<template>
  <div class="section">
  <div class="container container-column">
    
    <h2>The Trusted Name <br> for In-Home Tutoring.</h2>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt quo impedit excepturi inventore id exercitationem voluptates omnis, consectetur dicta fuga. Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa, sed. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Rerum, voluptatibus?</p>
    <a class="link-blue" href="#">Learn more</a>

    
    <img src="../assets/img/h5-img-1.jpg" alt="img">

      
      
    </div>



    
  </div>
  
</template>



<script>
export default {
  name: 'SectionComp'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixinis.scss';
@import '../assets/style/utilities';



.container-column{
  
  
  h2{
    
    margin-bottom: 20px;
    font-weight: bold;
    font-family: $title-font;
  }
  p{
    font-size: 20px;
    color: black;
    opacity: 0.5;
  }
  .link-blue{
    margin: 25px 0;
    display: block;
    text-transform: uppercase;
    font-weight: bold;
    text-decoration: none;
    color: $primary-color ;
    &:hover{
      color: darken($primary-color, 20% );
    }
  }
  .top-sectionColumn{
        position: absolute;
        right: 0;
        top: 70%;
      }
  
}
.top{
    i{
      display: block;
      font-size: 30px;
    }
    @include center (both);
    cursor: pointer;
    color: white;
    font-size: 20px;
    width: 80px;
    height: 80px;
    background-color: $primary-color;
    
    &:hover{
      color: darken($primary-color, 20% );
    }
    a{
      text-decoration: none;
      text-align: center;
      color:white;
      &:hover{
      color: darken($primary-color, 20% );
      transition: all 0.3s;
      font-weight: bold;
      font-family: $title-font;
    }
    }
  
  }

</style>