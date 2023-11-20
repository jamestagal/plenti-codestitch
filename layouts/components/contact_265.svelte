<script>
  export let title, subtitle, description, formFields, button, imageM, image, contactInfo;
</script>
<!-- ============================================ -->
<!--                Contact Form                  -->
<!-- ============================================ -->

<section id="cs-contact-265">
  <div class="cs-container">
    <div class="cs-left-section">
      <div class="cs-content">
        <span class="cs-topper">{title}</span>
        <h2 class="cs-title">{subtitle}</h2>
        <p class="cs-text">
          {description}
        </p>
      </div>
      <form id="cs-form-265" name="Contact Form" method="post">
        <label>
          {formFields.name}
          <input
            required
            type="text"
            id="name-265"
            name="name"
            placeholder="Name"
          />
        </label>
        <label>
          {formFields.email}
          <input
            required
            type="text"
            id="email-265"
            name="email"
            placeholder="Email"
          />
        </label>
        <label>
          {formFields.phone}
          <input
            required
            type="text"
            id="phone-265"
            name="phone"
            placeholder="Phone"
          />
        </label>
        <label>
          {formFields.reason}
          <input
            type="text"
            id="find-265"
            name="find-us"
            placeholder="How did you find us?"
          />
        </label>
        <label class="cs-label-message">
          {formFields.message}
          <textarea
            required
            name="Message"
            id="message-265"
            placeholder="Write message..."
          />
        </label>
        <button class="cs-button-solid cs-submit" type="submit"
          >{button.title}</button
        >
      </form>
    </div>
    <div class="cs-right-section">
      <!--Email-->
      <span class="cs-header">{contactInfo.email.title}</span>
      <a class="cs-link" href="mailto:{contactInfo.email.address}"
        >{contactInfo.email.address}</a
      >
      <!--Phone-->
      <span class="cs-header">{contactInfo.phone.title}</span>
      <a class="cs-link" href="tel:{contactInfo.phone.number}">{contactInfo.phone.number}</a>
      <!--Address-->
      <span class="cs-header">{contactInfo.address.title}</span>
      <a class="cs-link" href="."
        >{contactInfo.address.line1} <span class="cs-block">{contactInfo.address.line2}</span></a
      >

      <!-- Background Image-->
      <picture class="cs-bg-picture">
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
          width="542"
          height="662"
          aria-hidden="true"
        />
      </picture>
    </div>
  </div>
</section>

<style>
  /*-- -------------------------- -->
<---          Contact           -->
<--- -------------------------- -*/
  /* Mobile - 360px */
  @media only screen and (min-width: 0rem) {
    #cs-contact-265 {
      padding: var(--sectionPadding);
    }
    #cs-contact-265 .cs-container {
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
    #cs-contact-265 .cs-content {
      /* set text align to left if content needs to be left aligned */
      text-align: left;
      width: 100%;
      margin: 0 0 2rem 0;
      display: flex;
      flex-direction: column;
      /* centers content horizontally, set to flex-start to left align */
      align-items: flex-start;
    }
    #cs-contact-265 #cs-form-265 label {
      font-size: 1rem;
      line-height: 1.5em;
      font-weight: 700;
      /* 12px - 20px */
      margin-bottom: clamp(0.75rem, 1.3em, 1.25rem);
      color: var(--headerColor);
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-direction: column;
    }
    #cs-contact-265 #cs-form-265 .cs-label-message {
      /* 32px - 48px */
      margin-bottom: clamp(2rem, 6.3vw, 3rem);
    }
    #cs-contact-265 #cs-form-265 input,
    #cs-contact-265 #cs-form-265 textarea {
      font-size: 1rem;
      width: 100%;
      height: 4rem;
      margin-top: 0.25rem;
      padding-left: 1.25rem;
      border: 1px solid #b4b2c7;
      border-radius: 0.25rem;
      /* prevents border & padding from affecting height */
      box-sizing: border-box;
      transition: border 0.3s;
    }
    #cs-contact-265 #cs-form-265 input:hover,
    #cs-contact-265 #cs-form-265 textarea:hover {
      border: 1px solid var(--primary);
    }
    #cs-contact-265 #cs-form-265 textarea {
      font-family: inherit;
      padding-top: 1.25rem;
      min-height: 7.5rem;
    }
    #cs-contact-265 #cs-form-265 .cs-button-solid {
      width: 100%;
    }
    #cs-contact-265 .cs-submit {
      width: 100%;
      border: none;
    }
    #cs-contact-265 .cs-submit:hover {
      cursor: pointer;
    }
    #cs-contact-265 .cs-right-section {
      width: 100%;
      height: 20rem;
      /* 24px - 40px top & bottom */
      /* 20px - 40px left & right */
      padding: clamp(1.5rem, 3vw, 2.5rem) clamp(1.25rem, 3vw, 2.5rem);
      /* prevents padding from affecting height and width */
      box-sizing: border-box;
      border-radius: 0.25rem;
      /* cuts off corners on img tag */
      overflow: hidden;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-end;
      position: relative;
    }
    #cs-contact-265 .cs-header {
      /* 16px - 20px */
      font-size: clamp(1rem, 3vw, 1.25rem);
      line-height: 1.2em;
      font-weight: 700;
      margin-bottom: 0.5rem;
      color: var(--bodyTextColorWhite);
      display: block;
    }
    #cs-contact-265 .cs-link {
      /* 16px - 20px */
      font-size: clamp(1rem, 3vw, 1.25rem);
      line-height: 1.2em;
      text-decoration: none;
      margin-bottom: 1.25rem;
      color: var(--bodyTextColorWhite);
      display: block;
      position: relative;
    }
    #cs-contact-265 .cs-link:before {
      /* Animated underline */
      content: "";
      width: 0%;
      height: 2px;
      /* current color of the parent */
      background: currentColor;
      opacity: 1;
      position: absolute;
      display: block;
      bottom: -0.125rem;
      left: 0;
      transition: width 0.3s;
    }
    #cs-contact-265 .cs-link:hover:before {
      width: 100%;
    }
    #cs-contact-265 .cs-link:last-of-type {
      margin-bottom: 0;
    }
    #cs-contact-265 .cs-block {
      /* sends second address line to the bottom on its own line */
      display: block;
    }
    #cs-contact-265 .cs-bg-picture {
      width: 100%;
      height: 100%;
      display: block;
      position: absolute;
      top: 0;
      left: 0;
      z-index: -1;
      transition: transform 0.6s;
    }
    #cs-contact-265 .cs-bg-picture:before {
      /* background color overlay */
      content: "";
      position: absolute;
      display: block;
      height: 100%;
      width: 100%;
      background: linear-gradient(
        180deg,
        rgba(0, 0, 0, 0) 0%,
        rgba(0, 0, 0, 0.8) 100%
      );
      top: 0;
      left: 0;
      z-index: 1;
    }
    #cs-contact-265 .cs-bg-picture img {
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      /* Makes img tag act as a background image */
      object-fit: cover;
    }
  }
  /* Tablet - 700px */
  @media only screen and (min-width: 43.75rem) {
    #cs-contact-265 .cs-container {
      max-width: 80rem;
    }
    #cs-contact-265 #cs-form-265 {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      flex-wrap: wrap;
    }
    #cs-contact-265 #cs-form-265 label {
      width: 48%;
    }
    #cs-contact-265 #cs-form-265 .cs-label-message {
      width: 100%;
    }
  }
  /* Small Desktop - 1024px */
  @media only screen and (min-width: 64rem) {
    #cs-contact-265 .cs-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: flex-start;
      gap: 5rem;
    }
    #cs-contact-265 .cs-left-section {
      max-width: 39.375rem;
    }
    #cs-contact-265 #cs-form-265 label {
      width: 100%;
    }
    #cs-contact-265 .cs-right-section {
      /* changes to 578px at 1300px wide */
      height: 42.875rem;
      width: 40vw;
      max-width: 33.875rem;
      /* prevents flexbox from squishing it */
      flex: none;
    }
    #cs-contact-265 .cs-right-section:hover .cs-bg-picture {
      transform: scale(1.1);
    }
    #cs-contact-265 .cs-block {
      /* goes back to inline so it stays "in line" with the rest of the text */
      display: inline-block;
    }
  }
  /* Small Desktop - 1300px */
  @media only screen and (min-width: 81.25rem) {
    #cs-contact-265 #cs-form-265 {
      column-gap: 0rem;
    }
    #cs-contact-265 #cs-form-265 label {
      width: 48%;
      max-width: 19.0625rem;
    }
    #cs-contact-265 #cs-form-265 .cs-label-message {
      max-width: 100%;
    }
    #cs-contact-265 .cs-right-section {
      height: 36.125rem;
    }
  }
</style>
