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

</style>
