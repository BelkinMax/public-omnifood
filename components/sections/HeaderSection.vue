<template>
  <header class="header">
    <img class="logo" src="/resources/omnifood-logo.png" alt="Omnifood logo" />
    <nav class="navigation">
      navigation
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.header {
  // TODO: Make it sticky
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 9.6rem;
  background-color: $hero-bg;
  padding: 0 4.8rem;

  .logo {
    height: 2.2rem;
  }

  .navigation {
  }
}
</style>
