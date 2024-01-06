<script>
  import { onMount } from "svelte";
  import Login from "./login.svelte";
  import Head from "./head.svelte";
  import Header from "./header.svelte";
  import Footer from "./footer.svelte";

  export let content, layout, allContent, allLayouts, user, env;
  let hash;
  onMount(async () => {
    hash = window.location.hash;
  });

</script>

<html lang="en">
  <Head title={content.filename} {env} />
  <body>
    <!--Screen reader skip main nav-->
    <a class="skip" aria-label="skip to main content" href="#main"
      >Click To Skip To Main Content</a
    >
    {#if user && $user.isAuthenticated}
      <svelte:component this={$user.menu} {user} bind:content />
    {/if}
    <Login bind:hash {user} />
    <Header />
    <main id="main">
      <svelte:component
        this={layout}
        {...content.fields}
        {allContent}
        {allLayouts}
        {content}
      />
      <Footer />
    </main>
  </body>
</html>
