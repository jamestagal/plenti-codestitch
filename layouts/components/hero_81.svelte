<script>
  export let title, subtitle, link, image, image_m;
</script>
<!-- ============================================ -->
<!--                    Hero                      -->
<!-- ============================================ -->

<section id="hero-81">
  <div class="cs-container">
    <h1 class="cs-title">
      {title}
    </h1>
    <p class="cs-text">
      {subtitle}
    </p>
    <a href="{link.url}" class="cs-button-solid">{link.title}</a>
  </div>

  <!-- Background Image -->
  <picture class="cs-background">
    <source
      media="(max-width: 600px)"
      srcset="{image_m.url}"
    />
    <source
      media="(min-width: 601px)"
      srcset="{image.url}"
    />
    <img
      loading="lazy"
      decoding="async"
      src="{image.url}"
      alt="{image.alt}"
      width="2250"
      height="1500"
      aria-hidden="true"
    />
  </picture>
</section>
