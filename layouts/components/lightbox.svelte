<script>
    export let image;
  </script>
  
  <!-- ============================================ -->
  <!--            Lightbox Gallery                  -->
  <!-- ============================================ -->
  
  <section id="lightbox-gallery">
    <div class="cs-container">
      <div class="cs-content">
        <span class="cs-topper">GALLERY</span>
        <h2 class="cs-title">View a selection of our recent creations</h2>
        <p class="cs-text">
          Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet
          sint. Velit officia consequat duis enim velit mollit. Amet minim mollit
          non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia
          consequat duis enim velit mollit.
        </p>
      </div>
      <div class="gallery">
        <div class="gallery-item">
          <a href={image.url} data-lightbox="gallery" data-image-alt="Image 1">
            <img loading="lazy" decoding="async" src={image.url} alt="Alt Text" />
          </a>
        </div>
        <div class="gallery-item">
          <a href={image.url} data-lightbox="gallery" data-image-alt="Image 2">
            <img loading="lazy" decoding="async" src={image.url} alt="Alt Text" />
          </a>
        </div>
        <div class="gallery-item">
          <a href={image.url} data-lightbox="gallery" data-image-alt="Image 3">
            <img loading="lazy" decoding="async" src={image.url} alt="Alt Text" />
          </a>
        </div>
        <div class="gallery-item">
          <a href={image.url} data-lightbox="gallery" data-image-alt="Image 4">
            <img loading="lazy" decoding="async" src={image.url} alt="Alt Text" />
          </a>
        </div>
      </div>
    </div>
  </section>