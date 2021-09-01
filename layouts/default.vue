<template>
  <section>
    <HeroSection />
    <main>
      <Nuxt />
    </main>
  </section>
</template>

<script>
import HeroSection from "@/components/sections/HeroSection.vue";
export default {
  components: {
    HeroSection
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;600;700&display=swap");

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
</style>
