<template>
  <div class="jumbotron">
    <h1>Contemporary Ideas</h1>
    <div class="subtitle">
      <p>Lorem Ipsn gravida nibh vel velit auctor aliquetnean sollicitudin, lorem quis bibendum auci elit consequat ipsutis sem nibh id elited odio sit amet nibcursus a sit amet mauris.

      </p> 
    </div>

    <button>Register Now</button>

    <div class="icon">
      <i class="fas fa-circle"></i>
      <i class="fas fa-circle"></i>
      <i class="far fa-dot-circle active"></i>
    </div>


  </div>
</template>

<script>
export default {
  name: 'JumbotronComp'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';

.jumbotron{
  display: flex;
  flex-direction: column;
}
h1{
  font-size: 60px;
  color: white;
  text-align: center;
  margin-top: 120px;
  font-weight: bold;
  font-family: $title-font;
}
.subtitle{
  font-size: 18px;
  width: 850px;
  text-align: center;
  margin: 30px auto;
  color: white;
}
button{
  background-color: $primary-color;
  border: none;
  padding: 15px 25px;
  color: white;
  font-weight: bold;
  font-size: 13px;
  text-transform: uppercase;
  width: 200px;
  margin: 30px auto;
  margin-bottom: 120px;
  &:hover{
    background-color: darken($primary-color, 30%);
    transition: all 0.3s;
  }
}
.icon{
  text-align: center;
  padding: 30px;
  .active{
    filter: none;
  }
  i{
    cursor: pointer;
    color: white;
    margin: 0 10px;
    font-size: 30px;
    filter: opacity(.5); 
    &:hover{
      filter: none;
      transition: all 0.3s;
    }

  }
} 

</style>