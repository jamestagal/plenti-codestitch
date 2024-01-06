<script>
  export let title, subtitle, description, reviews, icon;
</script>
<!-- ============================================ -->
<!--                   Reviews                    -->
<!-- ============================================ -->

<section id="reviews-607">
  <div class="cs-container">
    <div class="cs-content">
      <span class="cs-topper">{title}</span>
      <h2 class="cs-title">{subtitle}</h2>
      <p class="cs-text">
        {description}
      </p>
    </div>
    <ul class="cs-card-group">
      {#each reviews as review}
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
        <h3 class="cs-h3">{review.title}</h3>
        <p class="cs-item-text">
          {review.quote}
        </p>
        <span class="cs-name">{review.name}</span>
      </li>
      {/each}
    </ul>
  </div>
</section>

<style>

</style>