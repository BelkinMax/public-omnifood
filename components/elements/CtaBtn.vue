<template>
  <a :href="to" class="btn" :class="btnType">{{ content }}</a>
</template>

<script>
export default {
  props: {
    type: {
      type: String,
      required: false,
      default: "main"
    },
    content: {
      type: String,
      required: true
    },
    to: {
      type: String,
      required: false,
      default: "#"
    }
  },
  computed: {
    btnType() {
      return `cta-${this.type}-btn`;
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.btn {
  transition: background-color 0.3s;
  font-weight: 600;

  &:link,
  &:visited {
    display: inline-block;
    font-size: 2rem;
    border-radius: 9px;
    text-decoration: none;

    padding: 1.6rem 3.2rem;
  }
}

.cta-primary-btn {
  &:link,
  &:visited {
    background-color: $brand-color;
    color: white;
  }
  &:hover,
  &:active {
    background-color: $brand-color-dark;
  }
}

.cta-secondary-btn {
  &:link,
  &:visited {
    background-color: white;
    color: $link-text-color;
    box-shadow: inset 0 0 0 3px white;
  }
  &:hover,
  &:active {
    background-color: transparent;
  }
}
</style>
