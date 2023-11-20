<script>
  export let title, subtitle, description, image, link;
</script>
<!-- ============================================ -->
<!--                 Side By Side                 -->
<!-- ============================================ -->

<section id="sbs-578">
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

<style>
  /*-- -------------------------- -->
<---       Side By Side         -->
<--- -------------------------- -*/
  /* Mobile - 360px */
  @media only screen and (min-width: 0rem) {
    #sbs-578 .cs-container {
      width: 100%;
      max-width: 80rem;
      margin: auto;
      display: flex;
      flex-direction: column;
      align-items: center;
      /* 48px - 64px */
      gap: clamp(3rem, 7vw, 4rem);
    }
    #sbs-578 .cs-content {
      /* set text aling to left if content needs to be left aligned */
      text-align: left;
      width: 100%;
      max-width: 32.625rem;
      /* moved section padding to the .cs-content so we can have the cs-picture be full width on mobile without the padding preventing it from doing so */
      padding: var(--sectionPadding);
      padding-top: 0;
      /* prevents padding from affecting width and height */
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      /* centers content horizontally, set to flex-start to left align */
      align-items: flex-start;
    }
    #sbs-578 .cs-text {
      /* Override.  cs-topper cs-title and first cs-text should be removed and put into your global css sheet so it can control every instance of them on your site and is consistent. This selector is a section specific override that stays inside this stitch */
      margin-bottom: 1rem;
    }
    #sbs-578 .cs-text:last-of-type {
      margin-bottom: 2rem;
    }
    #sbs-578 .cs-picture {
      display: block;
      position: relative;
      width: 100%;
      height: 18.75rem;
    }
    #sbs-578 .cs-picture img {
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      object-fit: cover;
    }
  }
  /* Tablet - 768px */
  @media only screen and (min-width: 48rem) {
    #sbs-578 {
      padding: var(--sectionPadding);
    }
    #sbs-578 .cs-container {
      flex-direction: row;
      justify-content: flex-start;
      /* 60px - 128px */
      gap: clamp(3.75rem, 10vw, 8rem);
    }
    #sbs-578 .cs-content {
      width: 53%;
      /* reset the padding, add the section padding back to the section container */
      padding: 0;
    }
    #sbs-578 .cs-picture {
      width: 47vw;
      max-width: 30.875rem;
      /* 518px - 700px */
      height: clamp(32.375rem, 63vw, 43.75rem);
      /* 16px - 28px, added margin left and bottom to cs-picture so it pushes away by the same amount the yellow box element overlaps it left and bottom. This maintains consistent spacing left and bottom */
      margin: 0 0 clamp(1rem, 2.4vw, 1.75rem) clamp(1rem, 2.4vw, 1.75rem);
      position: relative;
    }
    #sbs-578 .cs-picture:before {
      /* yellow box */
      content: "";
      width: 50%;
      height: 60%;
      background: var(--secondary);
      opacity: 1;
      display: block;
      position: absolute;
      /* 16px - 28px, wrapped in calc function to multiple by negative 1 and get a negative clamp value */
      bottom: calc(clamp(1rem, 2.4vw, 1.75rem) * -1);
      left: calc(clamp(1rem, 2.4vw, 1.75rem) * -1);
    }
  }
</style>
