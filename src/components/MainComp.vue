<template>
  <main>
    <CardComp />
    <SectionComp />
    <SectionSecond />

  </main>
</template>

<script>
import CardComp from './CardComp.vue';
import SectionComp from './SectionComp.vue';
import SectionSecond from './SectionSecond.vue';

export default {
    name: "MainComp",
    components: { CardComp, SectionComp, SectionSecond }
}
</script>

<style lang="scss" scoped>

</style>