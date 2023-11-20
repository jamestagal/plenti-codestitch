<script>
  export let service1, service2, service3;
</script>
<!-- ============================================ -->
<!--                   Services                   -->
<!-- ============================================ -->

<section id="h-services-81">
  <ul class="cs-card-group">
    <li class="cs-item">
      <picture class="cs-icon">
        <img
          loading="lazy"
          decoding="async"
          src="{service1.icon.url}"
          alt="{service1.icon.alt}"
          width="52"
          height="52"
          aria-hidden="true"
        />
      </picture>
      <h2 class="cs-title">{service1.title}</h2>
      <p class="cs-text">
        {service1.subtitle}
      </p>
    </li>
    <li class="cs-item">
      <picture class="cs-icon">
        <img
          loading="lazy"
          decoding="async"
          src="{service2.icon.url}"
          alt="{service2.icon.alt}"
          width="52"
          height="52"
          aria-hidden="true"
        />
      </picture>
      <h2 class="cs-title">{service2.title}</h2>
      <p class="cs-text">
        {service2.subtitle}
      </p>
    </li>
    <li class="cs-item">
      <picture class="cs-icon">
        <img
          loading="lazy"
          decoding="async"
          src="{service3.icon.url}"
          alt="{service3.icon.alt}"
          width="52"
          height="52"
          aria-hidden="true"
        />
      </picture>
      <h2 class="cs-title">{service3.title}</h2>
      <p class="cs-text">
        {service3.subtitle}
      </p>
    </li>
  </ul>
</section>
