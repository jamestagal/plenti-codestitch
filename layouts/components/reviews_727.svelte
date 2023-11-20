<script>
  export let title, subtitle, description, review1, review2, icon;
</script>
<!-- ============================================ -->
<!--                   Reviews                    -->
<!-- ============================================ -->

<section id="reviews-727">
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
        <img
          class="cs-icon"
          src="{icon.url}"
          alt="{icon.alt}"
          aria-hidden="true"
          width="40"
          height="38"
          loading="lazy"
          decoding="async"
        />
        <h3 class="cs-h3">{review1.title}</h3>
        <p class="cs-item-text">
          {review1.quote}
        </p>
        <span class="cs-name">{review1.name}</span>
      </li>
      <li class="cs-item">
        <img
          class="cs-icon"
          src="{icon.url}"
          alt="{icon.alt}"
          aria-hidden="true"
          width="40"
          height="38"
          loading="lazy"
          decoding="async"
        />
        <h3 class="cs-h3">{review2.title}</h3>
        <p class="cs-item-text">
          {review2.quote}
        </p>
        <span class="cs-name">{review2.name}</span>
      </li>
    </ul>
  </div>
</section>
