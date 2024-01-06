<script>
  export let title, subtitle, description, reason1, reason2, reason3, button;
</script>
<!-- ============================================ -->
<!--                 Why Choose                   -->
<!-- ============================================ -->

<section id="why-choose-12">
  <div class="cs-container">
    <div class="cs-content">
      <span class="cs-topper">{title}</span>
      <h2 class="cs-title">{subtitle}</h2>
      <p class="cs-text">
        {description}
      </p>
    </div>
    <ul class="cs-card-group">
      <li class="cs-item">
        <picture class="cs-picture">
          <img
            loading="lazy"
            decoding="async"
            src="{reason1.icon.url}"
            alt="{reason1.icon.alt}"
            width="42"
            height="42"
            aria-hidden="true"
          />
        </picture>
        <h3 class="cs-h3">{reason1.title}</h3>
        <p class="cs-item-text">
          {reason1.subtitle}
        </p>
      </li>
      <li class="cs-item">
        <picture class="cs-picture">
          <img
            loading="lazy"
            decoding="async"
            src="{reason2.icon.url}"
            alt="{reason2.icon.alt}"
            width="42"
            height="42"
            aria-hidden="true"
          />
        </picture>
        <h3 class="cs-h3">{reason2.title}</h3>
        <p class="cs-item-text">
          {reason2.subtitle}
        </p>
      </li>
      <li class="cs-item">
        <picture class="cs-picture">
          <img
            loading="lazy"
            decoding="async"
            src="{reason3.icon.url}"
            alt="{reason3.icon.alt}"
            width="32"
            height="42"
            aria-hidden="true"
          />
        </picture>
        <h3 class="cs-h3">{reason3.title}</h3>
        <p class="cs-item-text">
          {reason3.subtitle}
        </p>
      </li>
    </ul>
    <a href="{button.url}" class="cs-button-solid">{button.title}</a>
  </div>
</section>

<style>

</style>