<script>
  export let title, subtitle, description, button, image, imageM;
</script>
<!-- ============================================ -->
<!--                     CTA                      -->
<!-- ============================================ -->

<section id="cta-51">
  <div class="cs-container">
    <div class="cs-content">
      <span class="cs-topper">{title}</span>
      <h2 class="cs-title">{subtitle}</h2>
      <p class="cs-text">
        {description}
      </p>
      <a href="{button.url}" class="cs-button-solid">{button.title}</a>
    </div>
  </div>
  <!-- Background Image-->
  <picture class="cs-picture">
    <source
      media="(max-width: 600px)"
      srcset="{imageM.url}"
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
      width="1920"
      height="1280"
      aria-hidden="true"
    />
  </picture>
</section>
