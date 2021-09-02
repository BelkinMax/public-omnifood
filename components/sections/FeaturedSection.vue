<template>
  <section class="section-featured">
    <div class="container">
      <h2 class="heading-featured-in">As featured in</h2>
      <div class="logos">
        <img
          v-for="(logo, idx) in logos"
          :key="idx"
          :src="logo.src"
          :alt="logo.alt"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      logos: [
        { src: "/resources/techcrunch.png", alt: "Techcrunch logo" },
        {
          src: "/resources/business-insider.png",
          alt: "Business Insider logo"
        },
        {
          src: "/resources/the-new-york-times.png",
          alt: "The New York Times logo"
        },
        { src: "/resources/forbes.png", alt: "Forbes logo" },
        { src: "/resources/usa-today.png", alt: "USA Today logo" }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.container {
  margin: 0 auto;
  max-width: 120rem;
  padding: 0 3.2rem;
}

.section-featured {
  padding: 4.8rem 0 3.2rem 0;

  .heading-featured-in {
    color: #888;
    font-size: 1.4rem;
    font-weight: 500;
    letter-spacing: 0.75px;
    margin-bottom: 2.4rem;
    text-align: center;
    text-transform: uppercase;
  }

  .logos {
    display: flex;
    justify-content: space-around;

    img {
      filter: brightness(0);
      height: 3.2rem;
      opacity: 50%;
    }
  }
}
</style>
