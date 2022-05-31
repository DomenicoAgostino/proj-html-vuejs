<template>
   <section>
      <div class="container container-row">

      

        <div class="left-flex">
          <img src="../assets/img/h1-img-8.jpg" alt="">
        </div>

        <div class="right-flex">
          <h2>
            Empowering Children to Reach Their Potential.
          </h2>
          <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat quasi tempore ut reiciendis reprehenderit ea odit quibusdam dicta eaque iusto adipisci a atque eligendi aut cupiditate iure, excepturi possimus ad?</p>

          <div class="container-number">
            <div>
              <span class="number">168</span>
              <span class="text-span">User Stories</span>
            </div>
            <div>
              <span class="number">347</span>
              <span class="text-span">Events</span>
            </div>
          </div>
          
        </div>

    <div class="top top-botton">
      <a href="#">
        <i class="fas fa-chevron-up"></i>
        <span>TOP</span>
      </a>
      
    </div>


    </div>
  </section>
    
</template>

<script>
export default {
  name: 'SectionSecond'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';

  .top-botton{
        position: absolute;
        right: 0;
        bottom: 0;
      }
  
.top{
    i{
      display: block;
      font-size: 15px;
    }
    display: flex;
    align-items: center;
    cursor: pointer;
    color: white;
    font-size: 15px;
    width: 50px;
    height: 50px;
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

section{
  position: relative;
}

p{
  margin-top: 16px;
  font-size: 18px;
  color: black;
  opacity: 0.5;
}

h2{
    font-weight: bold;
    font-family: $title-font;
    font-size: 41px;
}
.container-row{
  display: flex;
  margin: 80px 0 40px 0;
  
  .left-flex{
    width: 400px;
    margin-top: 30px;
    img{
      width: 100%;
    }
  }
  .right-flex{
    margin-left: 80px;
    width: 450px;
  
  }
  .container-number{
    display: flex;
    color: $primary-color;
    div{
      width: 50%;
      padding: 40px 0;
    }
    .number{
      margin: 10px 0;
      font-size: 50px;
      display: block;
      font-weight: bold;
      font-family: $title-font;
    }

    .text-span{
      font-size: 20px;
      display: block;
      font-weight: bold;
      font-family: $title-font;
    }
  }
 
}


</style>