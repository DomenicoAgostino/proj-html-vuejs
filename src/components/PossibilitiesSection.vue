<template>
    <section>
      <div class="container container-possibilities">
      <div class="container-left">
      <div class="left" v-for="(item, index) in itemsList" :key="index">
          <span>{{item.title}}</span>
      </div>
      </div>
      <div class="right">
        <h2>Learning Possibilities</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad sint totam cum ipsum alias dolorum quas quibusdam ullam asperiores nulla aliquid eius maiores perferendis eaque facere consectetur animi, tempore est ducimus voluptatem dolorem natus officia ratione? Ratione nisi optio in.</p>
        <ul>
          <li 
          v-for="(item, index) in itemsList" :key="index"
          >
            <i 
            v-show="item.icon"
            class="fas fa-check"></i> 
            <span class="text-pos" v-if="item.icon" >
              {{item.listPossibilities}}
            </span>
          </li>
        </ul>
      </div>

      <div class="container-img-possibilities">
        <img src="../assets/img/h12-tabs-icon-1.png" alt="">
      </div>

    </div>
    </section>
  

</template>

<script>
export default {
  name: 'PossibilitiesSection',
  data(){
    return{
      itemsList:[
        {
          title:'What We Do',
          listPossibilities: 'We enrich lives through learning',
          icon: true
        },
        {
          title: 'Degree Programme',
          listPossibilities: 'Maximing potential through individual attention',
          icon: true
        },
        {
          title: 'Career Archievements',
          listPossibilities: 'The trusted name for specialized training',
          icon: true
        },
        {
          title: 'Personal Managment',
          listPossibilities: 'People teach. People learn. This is where they connect',
          icon: true
        },
        {
          title:'Steps To Success',
          icon: false
        },
        {
          title: 'Knowledge Transfer',
          icon: false
        }
      
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';

.text-pos{
  margin: 10px;
}
.container-possibilities{
  display: flex;
  align-items: center;
  width: 900px;
  position: relative;
  margin-bottom: 80px;
  .container-left{
    
    .left{
      cursor: pointer;
      display: flex;
      align-items: center;
      height: 58px;
      width: 240px;
      border: 1px solid #ECECEC;
      margin-left: 5px;
      &:hover, &:active{
        background-color: #FCFCFC;
        border-left: 5px solid $primary-color;
        span{
          color: $primary-color;
          
        }
      }
      
      span{
        margin: 10px;
        font-size: 15px;
        color: $secondary-color;
      }
    }
    
  }
  .right{
    margin-left: 13px;
    h2{

      font-weight: bold;
      font-size: 35px;
      margin-top: 50px;
    }
    p{
      margin: 13px 0;
      color: $secondary-color;
    }
    ul{
      color: $secondary-color;
      padding: 0;
      list-style: none;
      margin: 30px 0;
      
      li{
        margin: 10px 0;
        i{
          color: $primary-color;
        }
        
        span{
          margin: 10px 0px;
        }
      }
      
    }
  }
  .container-img-possibilities{
    position: absolute;
    bottom: 0;
    right: 0;
    width: 100px;
    img{
      width: 100%;
    }
  }
}

</style>