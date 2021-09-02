<template>
  <section>
    <HeaderSection />
    <HeroSection />
    <main>
      <Nuxt />
    </main>
  </section>
</template>

<script>
import HeroSection from "@/components/sections/HeroSection.vue";
import HeaderSection from "@/components/sections/HeaderSection.vue";

export default {
  components: {
    HeroSection,
    HeaderSection
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600;700&display=swap");
@import "@/assets/scss/colors.scss";

/* ---------------------------------- Basic --------------------------------- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
}

html,
body {
  background-color: #fff;
  color: #555;
  font-family: "Rubik", sans-serif;
  font-weight: 400;
  line-height: 1;
  text-rendering: optimizeLegibility;
  overflow-x: hidden;
}

.clearfix {
  zoom: 1;
}

.clearfix:after {
  content: ".";
  clear: both;
  display: block;
  height: 0;
  visibility: hidden;
}

.heading-primary,
.heading-secondary,
.heading-tertiary {
  color: #333;
  font-weight: 700;
  letter-spacing: -0.5px;
}

.heading-primary {
  font-size: 5.2rem;
  line-height: 1.05;
  margin-bottom: 3.2rem;
}

.heading-secondary {
  font-size: 4.4rem;
  line-height: 1.2;
  margin-bottom: 9.6rem;
}

.heading-tertiary {
  font-size: 3rem;
  line-height: 1.2;
  margin-bottom: 3.2rem;
}

.subheading {
  color: $brand-color-dark;
  display: block;
  font-size: 2rem;
  font-weight: 500;
  letter-spacing: 0.75px;
  margin-bottom: 1.6rem;
  text-transform: uppercase;
}
</style>
