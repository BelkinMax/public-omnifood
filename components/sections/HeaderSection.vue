<template>
  <header class="header">
    <img class="logo" src="/resources/omnifood-logo.png" alt="Omnifood logo" />
    <nav class="navigation">
      <ul class="nav-list">
        <li
          v-for="(item, idx) in navigationItems"
          :key="idx"
          class="nav-list-item"
        >
          <a :href="item.to">{{ item.title }}</a>
        </li>
        <CtaBtn type="primary" size="md" content="Try for free" to="#" />
      </ul>
    </nav>
  </header>
</template>

<script>
import CtaBtn from "@/components/elements/CtaBtn.vue";

export default {
  components: {
    CtaBtn
  },
  data() {
    return {
      navigationItems: [
        {
          title: "Section 1",
          to: "#"
        },
        {
          title: "Section 2",
          to: "#"
        },
        {
          title: "Section 3",
          to: "#"
        },
        {
          title: "Section 4",
          to: "#"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.header {
  // TODO: Make it sticky
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 9.6rem;
  background-color: $bg-colr-hero;
  padding: 0 4.8rem;

  .logo {
    height: 2.2rem;
  }

  .navigation {
    .nav-list {
      display: flex;
      align-items: center;
      list-style: none;
      gap: 3.2rem;

      &-item a {
        transition: all 0.3s;

        &:link,
        &:visited {
          text-decoration: none;
          color: $text-color-main;
          font-weight: 500;
          font-size: 1.8rem;
        }
        &:hover,
        &:active {
          color: $brand-color-dark;
        }
      }
    }
  }
}
</style>
