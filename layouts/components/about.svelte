<script>
  export let title, subtitle, description, image, link;
</script>
<!-- ============================================ -->
<!--                   About Us                   -->
<!-- ============================================ -->

<section id="RPsbs-580">
  <div class="cs-container">
    <picture class="cs-picture">
      <!--Mobile Image-->
      <source
        media="(max-width: 600px)"
        srcset="{image.url}"
      />
      <!--Tablet and above Image-->
      <source
        media="(min-width: 601px)"
        srcset="{image.url}"
      />
      <img
        loading="lazy"
        decoding="async"
        src="{image.url}"
        alt="{image.alt}"
        width="494"
        height="700"
      />
    </picture>
    <div class="cs-content">
      <span class="cs-topper">{subtitle}</span>
      <h2 class="cs-title">{title}</h2>
      {#each description as d}
      <p class="cs-text">
        {@html d.paragraph}
      </p>
      {/each}
      <a href="{link.url}" class="cs-button-solid">{link.title}</a>
    </div>
  </div>
</section>
