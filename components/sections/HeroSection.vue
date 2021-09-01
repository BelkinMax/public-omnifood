<template>
  <section class="hero-wrapper">
    <div class="hero">
      <div class="hero-textbox">
        <h1 class="heading-primary">
          {{ heading }}
        </h1>
        <p class="hero-description">
          {{ description }}
        </p>
        <div class="cta-wrapper">
          <CtaBtn type="primary" content="Start eating well" />
          <CtaBtn type="secondary" content="Learn more" />
        </div>
        <div class="customers">
          <div class="faces">
            <img
              v-for="(customer, idx) in customers"
              :key="idx"
              class="customer-photo"
              :src="customer.src"
              :alt="customer.alt"
            />
          </div>
          <p class="delivered">
            <span>{{ delivered[0] }}</span> {{ delivered[1] }}
          </p>
        </div>
      </div>
      <div class="hero-imgbox">
        <img
          class="hero-thumb"
          src="/resources/hero.webp"
          alt="Food delivery"
        />
      </div>
    </div>
  </section>
</template>

<script>
import CtaBtn from "@/components/elements/CtaBtn.vue";

export default {
  components: {
    CtaBtn
  },
  data() {
    return {
      heading: "A healthy meal delivered to your door, every single day",
      description:
        "The smart 365-days-per-year food subscription that will make you eat healthy again. Tailored to your personal tastes and nutritional needs.",
      delivered: ["250,000+", "meals delivered last year!"],
      customers: [
        { src: "/resources/customer-1.jpg", alt: "Customer photo" },
        { src: "/resources/customer-2.jpg", alt: "Customer photo" },
        { src: "/resources/customer-3.jpg", alt: "Customer photo" },
        { src: "/resources/customer-4.jpg", alt: "Customer photo" },
        { src: "/resources/customer-5.jpg", alt: "Customer photo" },
        { src: "/resources/customer-6.jpg", alt: "Customer photo" }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.hero-wrapper {
  background-color: $hero-bg;
  padding: 4.8rem 0 0.6rem 0;

  .hero {
    max-width: 130rem;
    margin: 0 auto;
    padding: 0 3.2rem;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 9.6rem;

    &-textbox {
      .heading-primary {
        font-size: 5.2rem;
        font-weight: 700;
        line-height: 1.05;
        color: $text-color;
        letter-spacing: -0.5px;

        margin-bottom: 3.2rem;
      }

      .hero-description {
        font-size: 2rem;
        line-height: 1.6;

        margin-bottom: 4.8rem;
      }

      .cta-wrapper {
        margin-bottom: 8rem;

        *:not(:last-child) {
          margin-right: 1.6rem;
        }
      }

      .customers {
        display: flex;
        align-items: center;
        gap: 1.6rem;

        .faces {
          display: flex;

          .customer-photo {
            height: 4.8rem;
            aspect-ratio: 1;
            border-radius: 50%;
            border: 3px solid $hero-bg;

            &:not(:first-child) {
              margin-left: -1.6rem;
            }
          }
        }

        .delivered {
          font-size: 1.8rem;
          font-weight: 600;

          span {
            color: $brand-color-dark;
          }
        }
      }
    }

    &-imgbox {
      .hero-thumb {
        width: 100%;
        font-weight: 700;
      }
    }
  }
}
</style>
