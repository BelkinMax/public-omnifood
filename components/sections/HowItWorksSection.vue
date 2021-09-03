<template>
  <section class="how-section">
    <div class="container">
      <span class="subheading">How it works</span>
      <h2 class="heading-secondary">
        Your daily dose of health in 3 simple steps
      </h2>
    </div>

    <grid-layout :cols="2">
      <!-- STEP 01 -->
      <div>
        <p class="step-number">01</p>
        <h3 class="heading-tertiary">
          Tell us what you like (and what not)
        </h3>
        <p class="step-description">
          Never again waste time thinking about what to eat! Omnifood AI will
          create a 100% personalized weekly meal plan just for you. It makes
          sure you get all the nutrients and vitamins you need, no matter what
          diet you follow!
        </p>
      </div>
      <div class="step-img-box">
        <img
          src="/resources/app-screen-1.png"
          class="step-img"
          alt="iPhone app
            preferences selection screen"
        />
      </div>

      <!-- STEP 02 -->
      <div class="step-img-box">
        <img
          src="/resources/app-screen-2.png"
          class="step-img"
          alt="iPhone app
            meal approving plan screen"
        />
      </div>
      <div>
        <p class="step-number">02</p>
        <h3 class="heading-tertiary">Approve your weekly meal plan</h3>
        <p class="step-description">
          Once per week, approve the meal plan generated for you by Omnifood AI.
          You can change ingredients, swap entire meals, or even add your own
          recipes.
        </p>
      </div>

      <!-- STEP 03 -->
      <div>
        <p class="step-number">03</p>
        <h3 class="heading-tertiary">Receive meals at convenient time</h3>
        <p class="step-description">
          Best chefs in town will cook your selected meal every day, and we will
          deliver it to your door whenever works best for you. You can change
          delivery schedule and address daily!
        </p>
      </div>
      <div class="step-img-box">
        <img
          src="/resources/app-screen-3.png"
          class="step-img"
          alt="iPhone app
            delivery screen"
        />
      </div>
    </grid-layout>
  </section>
</template>

<script>
import GridLayout from "@/components/elements/GridLayout.vue";

export default {
  components: {
    GridLayout
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.how-section {
  padding: 9.6rem 0;

  .container {
    margin: 0 auto;
    max-width: 120rem;
    padding: 0 3.2rem;
  }

  .step-img-box {
    align-items: center;
    display: flex;
    justify-content: center;
    position: relative;

    &::before,
    &::after {
      border-radius: 50%;
      content: "";
      display: block;
      left: 50%;
      position: absolute;
      top: 50%;
      transform: translate(-50%, -50%);
    }

    &::before {
      background-color: $tint-light;
      padding-bottom: 60%;
      width: 60%;
    }

    &::after {
      background-color: $tint-dark;
      padding-bottom: 45%;
      width: 45%;
    }

    .step-img {
      position: relative;
      width: 35%;
      z-index: 10;
    }
  }

  .step-number {
    color: #ddd;
    font-size: 9.8rem;
    font-weight: 600;
    margin-bottom: 1.2rem;
  }

  .step-description {
    font-size: 1.8rem;
    line-height: 1.8;
  }
}
</style>
