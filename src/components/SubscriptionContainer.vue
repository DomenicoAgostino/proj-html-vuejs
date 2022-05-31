<template> 
  <section> 
    <CourseSection />
    <PlansSection />
  </section>
</template>

<script>
import CourseSection from './CourseSection.vue'
import PlansSection from './PlansSection.vue'
export default {
  components: { CourseSection, PlansSection },
  name: 'SubscriptionContainer'
}
</script>

<style lang="scss" scoped>

section{
  background-image: url(../assets/img/page-background-img.png);
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  background-repeat: repeat;
  background-size: 190%;
  background-position: 75% 0%;
}
</style>