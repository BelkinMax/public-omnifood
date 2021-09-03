<template>
  <section class="section-meals">
    <div class="container center-text">
      <span class="subheading">Meals</span>
      <h2 class="heading-secondary">
        Omnifood AI chooses from 5,000+ recipes
      </h2>
    </div>

    <grid-layout :cols="3" class="margin-bottom-md">
      <div class="meal">
        <img
          src="/resources/meal-1.jpg"
          alt="Japanese Gyozas"
          class="meal-img"
        />
        <div class="meal-content">
          <div class="meal-tags">
            <span class="tag tag--vegetarian">Vegetarian</span>
          </div>
          <p class="meal-title">Japanese Gyozas</p>
          <ul class="meal-attributes">
            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z"
                />
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9.879 16.121A3 3 0 1012.015 11L11 14H9c0 .768.293 1.536.879 2.121z"
                />
              </svg>
              <span><strong>650</strong> Calories</span>
            </li>

            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M13 10V3L4 14h7v7l9-11h-7z"
                />
              </svg>
              <span>NutriScore &reg; <strong>74</strong></span>
            </li>
            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"
                />
              </svg>
              <span><strong>4.9</strong> Rating (537)</span>
            </li>
          </ul>
        </div>
      </div>

      <div class="meal">
        <img src="/resources/meal-2.jpg" alt="Avocado Salad" class="meal-img" />
        <div class="meal-content">
          <div class="meal-tags">
            <span class="tag tag--vegan">Vegan</span>
            <span class="tag tag--paleo">Paleo</span>
          </div>
          <p class="meal-title">Avocado Salad</p>
          <ul class="meal-attributes">
            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z"
                />
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9.879 16.121A3 3 0 1012.015 11L11 14H9c0 .768.293 1.536.879 2.121z"
                />
              </svg>
              <span><strong>400</strong> Calories</span>
            </li>

            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M13 10V3L4 14h7v7l9-11h-7z"
                />
              </svg>
              <span>NutriScore &reg; <strong>92</strong></span>
            </li>
            <li class="meal-attribute">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="meal-icon"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"
                />
              </svg>
              <span><strong>4.8</strong> Rating (441)</span>
            </li>
          </ul>
        </div>
      </div>

      <div class="diets">
        <h3 class="heading-tertiary">Works with any diet</h3>
        <ul class="list">
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Vegetarian </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Vegan </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Pescatarian </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Gluten-free </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Lactose-free </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Keto </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Paleo </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Low FODMAP </span>
          </li>
          <li class="list-item">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="list-icon"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 13l4 4L19 7"
              />
            </svg>
            <span> Kid-friendly </span>
          </li>
        </ul>
      </div>
    </grid-layout>

    <div class="container all-recipes">
      <a href="#" class="link">See all recipes &rarr;</a>
    </div>
  </section>
</template>

<script>
import GridLayout from "@/components/elements/GridLayout.vue";
export default {
  components: { GridLayout }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/colors.scss";

.container {
  margin: 0 auto;
  max-width: 120rem;
  padding: 0 3.2rem;
}

.section-meals {
  padding: 9.6rem 0;
}

.meal {
  border-radius: 11px;
  box-shadow: 0 2.4rem 4.8rem rgba(0, 0, 0, 0.075);
  overflow: hidden;
  transition: all 0.4s;

  &:hover {
    box-shadow: 0 3.2rem 6.4rem rgba(0, 0, 0, 0.06);
    transform: translateY(-1.2rem);
  }
}

.meal-content {
  padding: 3.2rem 4.8rem 4.8rem 4.8rem;
}

.meal-tags {
  display: flex;
  gap: 0.4rem;
  margin-bottom: 1.2rem;
}

.tag {
  border-radius: 100px;
  color: $gray-700;
  display: inline-block;
  font-size: 1.2rem;
  padding: 0.4rem 0.8rem;
  text-transform: uppercase;
}

.tag--vegetarian {
  background-color: $green;
}

.tag--vegan {
  background-color: $lime;
}

.tag--paleo {
  background-color: $yellow;
}

.meal-title {
  color: $gray-700;
  font-size: 2.4rem;
  font-weight: 600;
  margin-bottom: 3.2rem;
}

.meal-attributes {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  list-style: none;
}

.meal-attribute {
  align-items: center;
  display: flex;
  font-size: 1.8rem;
  gap: 1.6rem;
}

.meal-icon {
  height: 2.4rem;
  stroke: $brand-color;
  width: 2.4rem;
}

.meal-img {
  width: 100%;
}

.list {
  display: flex;
  flex-direction: column;
  gap: 1.6rem;
  list-style: none;

  &-item {
    align-items: center;
    display: flex;
    font-size: 1.8rem;
    gap: 1.6rem;
  }

  &-icon {
    height: 3rem;
    stroke: $brand-color;
    width: 3rem;
  }
}

.all-recipes {
  font-size: 1.8rem;
  text-align: center;
}

.margin-bottom-md {
  margin-bottom: 4.8rem !important;
}
</style>
