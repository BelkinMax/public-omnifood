<template>
  <a :href="to" class="btn" :class="custom">{{ content }}</a>
</template>

<script>
export default {
  props: {
    type: {
      type: String,
      required: false,
      default: "main"
    },
    size: {
      type: String,
      required: false,
      default: "lg"
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
    custom() {
      return `cta-${this.type}-btn btn-${this.size}`;
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.btn {
  display: inline-block;
  font-size: 2rem;
  text-decoration: none;
  transition: background-color 0.3s;

  &-lg {
    padding: 1.6rem 3.2rem;
    font-weight: 600;
    border-radius: 9px;
  }

  &-md {
    padding: 1.2rem 2.4rem;
    font-weight: 500;
    border-radius: 7px;
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
