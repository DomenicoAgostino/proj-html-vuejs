<template>
  <header>
    <div class="container">

      <a href="#">
        <img src="../assets/img/logo-light.png" alt="logo">
      </a>

      <nav>
        <ul>
          <li v-for="(link,index) in links" :key="index">
            <a href="#">{{link}}</a>
          </li>
        </ul>
      </nav>

    </div>

    <JumbotronComp />
  </header>
</template>

<script>
import JumbotronComp from './JumbotronComp.vue'
export default {
    name: "HeaderComp",
    data() {
        return {
            links: [
                "Home",
                "Courses",
                "Instructors",
                "Events",
                "Pages",
                "Elements"
            ]
        };
    },
    components: { JumbotronComp }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';



header{
  background: rgba(0, 0, 0, .3) url(../assets/img/course-9-f-img.jpg);  
  background-blend-mode: darken;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
    .container{
      display: flex;
      justify-content: center;
      align-items: center;
      padding-top: 30px;
      i{
        cursor: pointer;
        filter: opacity(1); 
        font-size: 20px;
        margin: 0 20px;
        color: white;
        &:first-child {
          transform: rotate(90deg);
        }
        &:hover, &:active{
          transition: all 0.3s;
          color: $primary-color;
        }
      }
      img{
          width: 250px;
        }
        ul{ 
          display: flex;
          margin: 0;
          li{
            text-transform: uppercase;
            list-style: none;
            margin: 0 20px ;
            a{
              text-decoration: none;
              color: white;
              font-size: 18px;
              &:hover{
                transition: all 0.3s;
                color: $primary-color;
              }
            }
          }
        }
    }

  
}

</style>