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
    /*-- -------------------------- -->
<---       Why Choose Us        -->
<--- -------------------------- -*/
/* Mobile - 360px */
@media only screen and (min-width: 0rem) {
  #why-choose-12 {
    padding: var(--sectionPadding);
    background-color: #f7f7f7;
  }
  #why-choose-12 .cs-container {
    width: 100%;
    max-width: 80rem;
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    /* 48px - 64px */
    gap: clamp(3rem, 6vw, 4rem);
  }
  #why-choose-12 .cs-content {
    /* set text align to left if content needs to be left aligned */
    text-align: center;
    width: 100%;
    display: flex;
    flex-direction: column;
    /* centers content horizontally, set to flex-start to left align */
    align-items: center;
  }
  #why-choose-12 .cs-card-group {
    width: 100%;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 3.75rem;
  }
  #why-choose-12 .cs-item {
    text-align: center;
    list-style: none;
    width: 100%;
    max-width: 22.5rem;
    margin: 0;
    padding: 0;
  }
  #why-choose-12 .cs-picture {
    /* 68px - 88px */
    width: clamp(4.25rem, 7vw, 5.5rem);
    height: clamp(4.25rem, 7vw, 5.5rem);
    margin: auto;
    margin-bottom: 2rem;
    border-radius: 50%;
    background-color: var(--primary);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  #why-choose-12 .cs-picture img {
    width: auto;
    height: 2.625rem;
    display: block;
  }
  #why-choose-12 .cs-h3 {
    font-size: 1.25rem;
    line-height: 1.2em;
    text-align: inherit;
    font-weight: 700;
    text-transform: uppercase;
    margin: 0;
    margin-bottom: 0.5rem;
    color: var(--headerColor);
  }
  #why-choose-12 .cs-item-text {
    font-size: 1rem;
    text-align: inherit;
    line-height: 1.5em;
    margin: 0;
    color: var(--bodyTextColor);
  }
}
/* Tablet - 768px */
@media only screen and (min-width: 48rem) {
  #why-choose-12 .cs-card-group {
    flex-direction: row;
    justify-content: space-between;
  }
}
/* Dark Mode */
@media only screen and (min-width: 0rem) {
  body.dark-mode #why-choose-12 {
    background-color: rgba(0, 0, 0, 0.2);
  }
  body.dark-mode #why-choose-12 .cs-title,
  body.dark-mode #why-choose-12 .cs-h3,
  body.dark-mode #why-choose-12 .cs-item-text,
  body.dark-mode #why-choose-12 .cs-text {
    color: var(--bodyTextColorWhite);
  }
  body.dark-mode #why-choose-12 .cs-picture {
    background: var(--primary);
  }
}
</style>