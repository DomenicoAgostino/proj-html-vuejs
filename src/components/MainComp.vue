<template>
  <main>
    <CardComp />
    <SectionComp />
    <SectionSecond />
    <ReviewSection />
    <PossibilitiesSection />
    <SubscriptionContainer />
    <SponsorComp />
    
  </main>
</template>

<script>
import CardComp from './CardComp.vue';
import SectionComp from './SectionComp.vue';
import SectionSecond from './SectionSecond.vue';
import ReviewSection from './ReviewSection.vue';
import PossibilitiesSection from './PossibilitiesSection.vue';
import SubscriptionContainer from './SubscriptionContainer.vue';
import SponsorComp from './SponsorComp.vue';




export default {
    name: "MainComp",
    components: { CardComp, SectionComp, SectionSecond, ReviewSection, PossibilitiesSection, SubscriptionContainer, SponsorComp, }
}
</script>

<style lang="scss" scoped>

</style>