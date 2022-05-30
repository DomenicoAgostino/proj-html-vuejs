<template>
  <main>
    <CardComp />
    <SectionComp />
    <SectionSecond />
    <ReviewSection />
  </main>
</template>

<script>
import CardComp from './CardComp.vue';
import SectionComp from './SectionComp.vue';
import SectionSecond from './SectionSecond.vue';
import ReviewSection from './ReviewSection.vue';

export default {
    name: "MainComp",
    components: { CardComp, SectionComp, SectionSecond, ReviewSection }
}
</script>

<style lang="scss" scoped>

</style>