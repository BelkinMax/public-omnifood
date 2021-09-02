<template>
  <section class="container grid" :style="gridCols">
    <slot></slot>
  </section>
</template>

<script>
export default {
  props: {
    cols: {
      type: Number,
      required: true
    }
  },
  computed: {
    gridCols() {
      return `grid-template-columns: repeat(${this.cols}, 1fr);`;
    }
  }
};
</script>

<style lang="scss" scoped>
.container {
  margin: 0 auto;
  max-width: 120rem;
}

.grid {
  column-gap: 6.4rem;
  display: grid;
  row-gap: 9.6rem;
  padding: 0 3.2rem;
}
</style>
