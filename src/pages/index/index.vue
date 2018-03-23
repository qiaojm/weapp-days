<template>
  <div class="container"> 
   <div class="item item-left"><span><img :src=birthday><br/>生日</span></div>
   <div class="item"><span><img :src=love><br/>爱情</span></div>
   <div class="item"><span><img :src=marry><br/>结婚</span></div>
    <div class="item item-left"><span><img :src=holiday><br/>节假日</span></div>
   <div class="item"><span><img :src=baby><br/>宝宝</span></div>
   <div class="item"><span><img :src=count><br/>倒计时</span></div>
    <div class="item item-left"><span><img :src=work><br/>工作</span></div>
   <div class="item"><span><img :src=divide><br/>离别</span></div>
   <div class="item"><span><img :src=individual><br/>自定义</span></div>
   <div class="item item-left">
     <span>
       <!-- <a href="/pages/counter/counter">点击添加</a> -->
       <a href="/pages/list/list">点击添加</a>
       <img class="finally" :src=add>
       <br/>
      </span>
    </div>
  </div>
</template>

<script>
import birthday from './img/birthday.png'
import love from './img/love.png'
import marry from './img/marry.png'
import holiday from './img/holiday.png'
import baby from './img/baby.png'
import count from './img/count.png'
import work from './img/work.png'
import divide from './img/divide.png'
import individual from './img/individual.png'
import add from './img/add.png'

export default{
  name: 'indexPage',
  data () {
    return {
      birthday,
      love,
      marry,
      holiday,
      baby,
      count,
      work,
      divide,
      individual,
      add
    }
  }
}
</script>

<style>
html,body{
    overflow: hidden;
    height: 100%;
    width: 100%;
}
.container {
  display: flex;
  -webkit-display:flex;
  -moz-display:flex;  
  flex-direction: row;
  align-items: center;
  justify-content: center; 
  flex-wrap: wrap;
    overflow: hidden;
  /* padding-top: 2rem; */
}
.item{
  /* flex: 1; */
  /* margin-right: 0.5rem; */
  width: 20%;
  margin-right: 0.5rem;
  height: 2rem;
  margin-bottom: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
span{
  text-align: center;
  font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif
}
img{
  width: 0.8rem;
  height: 0.8rem;
  text-align: center;
}
.item-left{
  margin-left: 0.5rem;
}
.finally{
  margin-top: 0.5rem;
}
</style>
