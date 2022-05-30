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
              <span>User Stories</span>
            </div>
            <div>
              <span class="number">347</span>
              <span>Events</span>
            </div>
          </div>
          
        </div>

        <div class="top ">
          
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

section{
  position: relative;
}
.container-row{
  display: flex;
  margin: 80px 0 40px 0;
  
  .left-flex{
    width: 500px;
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
    }
  }
 
}


</style>