<script>
  export let title, subtitle, description, cards, button, socialIcon;
</script>
<!-- ============================================ -->
<!--                 Meet The Team                -->
<!-- ============================================ -->

<section id="meet-team-221">
  <div class="cs-container">
    <div class="cs-content">
      <span class="cs-topper">{title}</span>
      <h2 class="cs-title">{subtitle}</h2>
      <p class="cs-text">
        {description}
      </p>
    </div>
    <ul class="cs-card-group">
      {#each cards as card}
      <li class="cs-item">
        <picture class="cs-picture">
          <img
            aria-hidden="true"
            loading="lazy"
            decoding="async"
            src="{card.image.url}"
            alt="{card.image.alt}"
            width="275"
            height="132"
          />
        </picture>
        <span class="cs-name">{card.name}</span>
        <span class="cs-job-title">{card.title}</span>
        <p class="cs-item-text">
          {card.blurb}
        </p>
        <!-- Social Flexbox -->
        <div class="cs-social">
          <a
            href="{card.socials.x}"
            class="cs-link"
            aria-label="Twitter"
            target="_blank"
            rel="noopener"
          >
            <img
              class="cs-icon"
              aria-hidden="true"
              loading="lazy"
              decoding="async"
              src="{socialIcon.x}"
              alt="twitter"
              width="15"
              height="13"
            />
          </a>
          <a
            href="{card.socials.linkedin}"
            class="cs-link"
            aria-label="Linked in"
            target="_blank"
            rel="noopener"
          >
            <img
              class="cs-icon"
              aria-hidden="true"
              loading="lazy"
              decoding="async"
              src="{socialIcon.linkedin}"
              alt="linkedin"
              width="17"
              height="16"
            />
          </a>
        </div>
      </li>
      {/each}
    </ul>
    <a href="{button.url}" class="cs-button-solid">{button.title}</a>
  </div>
</section>
