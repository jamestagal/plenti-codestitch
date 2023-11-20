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
    /*-- -------------------------- -->
<---          Reviews           -->
<--- -------------------------- -*/
/* Mobile - 360px */
@media only screen and (min-width: 0rem) {
  #reviews-607 {
    padding: var(--sectionPadding);
  }
  #reviews-607 .cs-container {
    width: 100%;
    /* changes to 1280px at tablet */
    max-width: 34.375rem;
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    /* 48px - 64px */
    gap: clamp(3rem, 6vw, 4rem);
  }
  #reviews-607 .cs-content {
    /* set text align to left if content needs to be left aligned */
    text-align: center;
    width: 100%;
    display: flex;
    flex-direction: column;
    /* centers content horizontally, set to flex-start to left align */
    align-items: center;
  }
  #reviews-607 .cs-card-group {
    width: 100%;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.25rem;
  }
  #reviews-607 .cs-item {
    list-style: none;
    width: 100%;
    margin: 0;
    /* 32px - 48px top & bottom */
    /* 16px - 32px left & right */
    padding: clamp(2rem, 7vw, 3rem) clamp(1rem, 4vw, 2rem);
    /* makes padding not affect height and width */
    box-sizing: border-box;
    background-color: #F0F0F0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  #reviews-607 .cs-icon {
    /* 30px - 40px */
    width: clamp(1.875rem, 4vw, 2.5rem);
    height: auto;
    margin: 0 0 2rem 0;
    display: block;
  }
  #reviews-607 .cs-h3 {
    /* 20px - 25px */
    font-size: clamp(1.25rem, 4vw, 1.5625rem);
    line-height: 1.2em;
    font-weight: 700;
    margin: 0 0 1.5rem 0;
    color: var(--headerColor);
  }
  #reviews-607 .cs-item-text {
    /* 14px - 16px */
    font-size: clamp(0.875rem, 4vw, 1rem);
    line-height: 1.5em;
    max-width: 24.25rem;
    margin: 0 0 3rem 0;
    color: var(--bodyTextColor);
  }
  #reviews-607 .cs-name {
    font-size: 1.25rem;
    line-height: 1.2em;
    font-weight: 500;
    margin: auto 0 0 0;
    color: var(--headerColor);
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 0.5rem;
    position: relative;
  }
  #reviews-607 .cs-name:before {
    content: '';
    width: 0.5rem;
    height: 1px;
    background: currentColor;
    display: block;
    position: relative;
  }
}
/* Tablet - 768px */
@media only screen and (min-width: 48rem) {
  #reviews-607 .cs-container {
    max-width: 80rem;
  }
  #reviews-607 .cs-card-group {
    /* we went grid on tablet so that we can have an even spaced section with this design. Flexbox has a hard time making this type of design work with even gaps. */
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
  #reviews-607 .cs-item {
    grid-column: span 1;
    grid-row: span 1;
  }
}
/* Small Desktop - 1024px */
@media only screen and (min-width: 64rem) {
  #reviews-607 .cs-card-group {
    /* went back to flexbox for an easier transition to this horizontal layout. We don't have to re-target each cs-item to reset its grid positioning, we can just revert to flexbox and make the layout in less code and hassle */
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: stretch;
    justify-content: center;
  }
  #reviews-607 .cs-item {
    width: clamp(31.5%, 30.93vw, 32.29%);
  }
}
/* Dark Mode */
@media only screen and (min-width: 0rem) {
  body.dark-mode #reviews-607 .cs-title,
  body.dark-mode #reviews-607 .cs-text,
  body.dark-mode #reviews-607 .cs-h3,
  body.dark-mode #reviews-607 .cs-name,
  body.dark-mode #reviews-607 .cs-item-text {
    color: var(--bodyTextColorWhite);
  }
  body.dark-mode #reviews-607 .cs-text,
  body.dark-mode #reviews-607 .cs-item-text {
    opacity: .8;
  }
  body.dark-mode #reviews-607 .cs-item {
    background-color: rgba(0, 0, 0, 0.2);
  }
}
</style>