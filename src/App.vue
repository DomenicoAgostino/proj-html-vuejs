<template>
  <div id="app">
    <HeaderComp />
    <CardComp />
  </div>
</template>
<script>
import HeaderComp from './components/HeaderComp.vue';
import CardComp from './components/CardComp.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    CardComp
}
}
</script>

<style lang="scss">
@import './assets/style/general'

</style>
