<script>
  export let title, subtitle, row1, row2, row3;
</script>
<!-- ============================================ -->
<!--                   Gallery                    -->
<!-- ============================================ -->

<section id="gallery-48">
  <div class="cs-container">
    <div class="cs-content">
      <span class="cs-topper">{title}</span>
      <h2 class="cs-title">
        {subtitle}
      </h2>
    </div>
    <div class="cs-image-group">
      <div class="cs-row cs-row-1">
        <!-- Row 1-->
        <picture class="cs-picture cs-picture-1">
          <source
            media="(max-width: 600px)"
            srcset="{row1.picture1.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row1.picture1.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row1.picture1.image.url}"
            alt="{row1.picture1.image.alt}"
            width="420"
            height="567"
          />
        </picture>
        <picture class="cs-picture cs-picture-2">
          <source
            media="(max-width: 600px)"
            srcset="{row1.picture2.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row1.picture2.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row1.picture2.image.url}"
            alt="{row1.picture2.image.alt}"
            width="420"
            height="630"
          />
        </picture>
        <picture class="cs-picture cs-picture-3">
          <source
            media="(max-width: 600px)"
            srcset="{row1.picture3.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row1.picture3.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row1.picture3.image.url}"
            alt="{row1.picture3.image.alt}"
            width="420"
            height="512"
          />
        </picture>
        <!-- To add more images, copy and paste this row's picture tags here in order from cs-picture-1 to cs-picture-3 and they will maintain the same layout-->
      </div>
      <!-- Row 2 -->
      <div class="cs-row cs-row-2">
        <picture class="cs-picture cs-picture-1">
          <source
            media="(max-width: 600px)"
            srcset="{row2.picture1.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row2.picture1.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row2.picture1.image.url}"
            alt="{row2.picture1.image.alt}"
            width="420"
            height="492"
          />
        </picture>
        <picture class="cs-picture cs-picture-2">
          <source
            media="(max-width: 600px)"
            srcset="{row2.picture2.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row2.picture2.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row2.picture2.image.url}"
            alt="{row2.picture2.image.alt}"
            width="420"
            height="517"
          />
        </picture>
        <picture class="cs-picture cs-picture-3">
          <source
            media="(max-width: 600px)"
            srcset="{row2.picture3.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row2.picture3.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row2.picture3.image.url}"
            alt="{row2.picture3.image.alt}"
            width="420"
            height="629"
          />
        </picture>
        <!-- To add more images, copy and paste this row's picture tags here in order from cs-picture-1 to cs-picture-3 and they will maintain the same layout-->
      </div>
      <!-- Row 3 -->
      <div class="cs-row cs-row-3">
        <picture class="cs-picture cs-picture-1">
          <source
            media="(max-width: 600px)"
            srcset="{row3.picture1.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row3.picture1.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row3.picture1.image.url}"
            alt="{row3.picture1.image.alt}"
            width="420"
            height="625"
          />
        </picture>
        <picture class="cs-picture cs-picture-2">
          <source
            media="(max-width: 600px)"
            srcset="{row3.picture2.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row3.picture2.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row3.picture2.image.url}"
            alt="{row3.picture2.image.alt}"
            width="420"
            height="452"
          />
        </picture>
        <picture class="cs-picture cs-picture-3">
          <source
            media="(max-width: 600px)"
            srcset="{row3.picture3.imageM.url}"
          />
          <source
            media="(min-width: 601px)"
            srcset="{row3.picture3.image.url}"
          />
          <img
            loading="lazy"
            decoding="async"
            src="{row3.picture3.image.url}"
            alt="{row3.picture3.image.alt}"
            width="420"
            height="629"
          />
        </picture>
        <!-- To add more images, copy and paste this row's picture tags here in order from cs-picture-1 to cs-picture-3 and they will maintain the same layout-->
      </div>
    </div>
  </div>
</section>

<style>
   
</style>