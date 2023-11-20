<script>
  import { scale, fade } from "svelte/transition";
  export let title, subtitle, gallery1, gallery2, gallery3;
  let selectedCategory = 'one';
</script>

<!-- ============================================ -->
<!--                   Gallery                    -->
<!-- ============================================ -->

<section id="gallery-453">
  <div class="cs-container">
    <div class="cs-content">
      <div class="cs-flex">
        <span class="cs-topper">{title}</span>
        <h2 class="cs-title">{subtitle}</h2>
      </div>
      <div class="cs-button-group">
        <!--When adding extra galleries, copy and paste the button and make data-filter equal to four, then five, etc. Do the same for the corresponding gallery and it's data attribute-->
        <button
          on:click={() => (selectedCategory = "one")}
          class="cs-button {selectedCategory === 'one' ? 'cs-active' : ''}"
          data-filter="one"
        >
          Renovations
        </button>
        <button
          on:click={() => (selectedCategory = "two")}
          class="cs-button {selectedCategory === 'two' ? 'cs-active' : ''}"
          data-filter="two"
        >
          Sod
        </button>
        <button
          on:click={() => (selectedCategory = "three")}
          class="cs-button {selectedCategory === 'three' ? 'cs-active' : ''}"
          data-filter="three"
        >
          Fencing
        </button>
      </div>
    </div>
    {#key selectedCategory}
      <!--Gallery 1-->
      {#if selectedCategory === "one"}
        <div
          transition:fade={{ duration: 400 }}
          class="cs-gallery"
          data-category="one"
        >
          <!--Picture 1-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery1.image1.url} />
            <source media="(min-width: 601px)" srcset={gallery1.image1.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery1.image1.url}
              alt={gallery1.image1.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 2-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery1.image2.url} />
            <source media="(min-width: 601px)" srcset={gallery1.image2.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery1.image2.url}
              alt={gallery1.image2.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 3-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery1.image3.url} />
            <source media="(min-width: 601px)" srcset={gallery1.image3.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery1.image3.url}
              alt={gallery1.image3.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 4-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery1.image4.url} />
            <source media="(min-width: 601px)" srcset={gallery1.image4.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery1.image4.url}
              alt={gallery1.image4.alt}
              width="305"
              height="400"
            />
          </picture>
        </div>
      {/if}
      <!--Gallery 2-->
      {#if selectedCategory === "two"}
        <div
          transition:fade={{ duration: 400 }}
          class="cs-gallery"
          data-category="two"
        >
          <!--Picture 1-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery2.image1.url} />
            <source media="(min-width: 601px)" srcset={gallery2.image1.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery2.image1.url}
              alt={gallery2.image1.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 2-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery2.image2.url} />
            <source media="(min-width: 601px)" srcset={gallery2.image2.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery2.image2.url}
              alt={gallery2.image2.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 3-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery2.image3.url} />
            <source media="(min-width: 601px)" srcset={gallery2.image3.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery2.image3.url}
              alt={gallery2.image3.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 4-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery2.image4.url} />
            <source media="(min-width: 601px)" srcset={gallery2.image4.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery2.image4.url}
              alt={gallery2.image4.alt}
              width="305"
              height="400"
            />
          </picture>
        </div>
      {/if}
      <!--Gallery 3-->
      {#if selectedCategory === "three"}
        <div
          transition:fade={{ duration: 400 }}
          class="cs-gallery"
          data-category="three"
        >
          <!--Picture 1-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery3.image1.url} />
            <source media="(min-width: 601px)" srcset={gallery3.image1.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery3.image1.url}
              alt={gallery3.image1.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 2-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery3.image2.url} />
            <source media="(min-width: 601px)" srcset={gallery3.image2.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery3.image2.url}
              alt={gallery3.image2.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 3-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery3.image3.url} />
            <source media="(min-width: 601px)" srcset={gallery3.image3.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery3.image3.url}
              alt={gallery3.image3.alt}
              width="305"
              height="400"
            />
          </picture>
          <!--Picture 4-->
          <picture class="cs-image">
            <source media="(max-width: 600px)" srcset={gallery3.image4.url} />
            <source media="(min-width: 601px)" srcset={gallery3.image4.url} />
            <img
              loading="lazy"
              decoding="async"
              src={gallery3.image4.url}
              alt={gallery3.image4.alt}
              width="305"
              height="400"
            />
          </picture>
        </div>
      {/if}
    {/key}
  </div>
</section>
