<template>
  <div>
    <FeaturedSection />
    <HowItWorksSection />
    <MealsSection />
  </div>
</template>

<script>
import FeaturedSection from "@/components/sections/FeaturedSection.vue";
import HowItWorksSection from "@/components/sections/HowItWorksSection.vue";
import MealsSection from "@/components/sections/MealsSection.vue";
export default {
  components: {
    FeaturedSection,
    HowItWorksSection,
    MealsSection
  }
};
</script>
