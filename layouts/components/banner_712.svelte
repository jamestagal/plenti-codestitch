<script>
  export let title, image, imageM;
</script>
<!-- ============================================ -->
<!--                   Banner                     -->
<!-- ============================================ -->

<div id="banner-712">
  <div class="cs-container">
    <span class="cs-int-title">{title}</span>
  </div>
  <!--Background Image-->
  <picture class="cs-background">
    <!--Mobile Image-->
    <source
      media="(max-width: 600px)"
      srcset="{imageM.url}"
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
      width="1280"
      height="568"
      aria-hidden="true"
    />
  </picture>
</div>
