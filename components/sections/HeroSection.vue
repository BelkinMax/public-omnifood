<template>
  <section class="section-hero">
    <div class="hero">
      <div class="hero-textbox">
        <h1 class="heading-primary">
          A healthy meal delivered to your door, every single day
        </h1>
        <p class="hero-description">
          Hello, we’re Omnifood, your new premium food delivery service. We know
          you’re always busy. No time for cooking. So let us take care of that,
          we’re really good at it, we promise!
        </p>
        <a href="#" class="cta-main-btn">Start eating well</a>
        <a href="#" class="cta-secondary-btn">Learn more &darr;</a>
      </div>
      <div class="hero-imgbox">
        <img class="hero-thumb" src="/resources/hero.jpg" alt="Food delivery" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.section-hero {
  .hero {
    max-width: 130rem;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(2, 1fr);

    &-textbox {
      .heading-primary {
      }
      .hero-description {
      }
    }

    &-imgbox {
      .hero-thumb {
        width: 100%;
      }
    }
  }
}
</style>
