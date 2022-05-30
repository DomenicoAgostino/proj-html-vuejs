<template>
<div class="container">
  <div class="row d-flex">
      <div class="col text-center"
      v-for="(subject,index) in subjects" :key="index">
      <img class="d-block" :src ="require ('../assets/img/'+ subject.img)"
      :alt="subject.title">
      <span>{{subject.title}}</span>
      </div>
  </div>

</div>
</template>

<script>
export default {
  name: 'CardComp',
  data() {
    return {
      subjects:[
      {
        title: 'Languages',
        img: 'h5-custom-icon-1.png'
      },
      {
        title: 'Software',
        img: 'h5-custom-icon-2.png'
      },
      {
        title: 'Business',
        img: 'h5-custom-icon-3.png'
      },
      {
        title: 'Chemistry',
        img: 'h5-custom-icon-4.png'
      },
      {
        title: 'Science',
        img: 'h5-custom-icon-5.png'
      },
      {
        title: 'DIY-Craft',
        img: 'h5-custom-icon-6.png'
      },
    ]
    }
  },
}
</script>

<style lang="scss" scoped>
@import '../assets/style/utilities';
@import '../assets/style/vars';

.row{
  margin: 60px 0;

}

.col{
  padding: 50px 0;
  margin: 20px;
  border: 1px solid lightgray;
  background-color: darken(#F2F8FC, 5%);
}


img {
  margin-bottom: 20px;
  
}


</style>