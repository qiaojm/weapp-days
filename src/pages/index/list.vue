<template>
 <div class="container">
<div class="item"> <div class=" item-left"><img :src=birthday></div><div class="item-right"><strong>哈哈</strong><br/><span>2018-3-22</span></div></div>
 <hr/>
<div class="item"> <div class=" item-left"><img :src=love></div><div class="item-right"><strong>哈哈</strong><br/><span>2018-3-22</span></div></div>
 <hr/>
<div class="item"> <div class=" item-left"><img :src=marry></div><div class="item-right"><strong>哈哈</strong><br/><span>2018-3-22</span></div></div>
 <hr/>
 <div class="item"> <div class=" item-left"><img :src=birthday></div><div class="item-right"><strong>哈哈</strong><br/><span>2018-3-22</span></div></div>
 <hr/>
 <div class="item"> <div class=" item-left"><img :src=birthday></div><div class="item-right"><strong>哈哈</strong><br/><span>2018-3-22</span></div></div>
 <hr/>
  </div>
</template>
<script>
import birthday from './img/birthday.png'
import love from './img/love.png'
import marry from './img/marry.png'
export default {
  name: 'list',
  data () {
    return {
      birthday,
      love,
      marry
    }
  }

}
</script>

<style>
.html,body{
  width: 100%;
  height: 100%;
}
.container{
  display: flex;
  /* justify-content: flex-start; */
}
.item{
  display: flex;
  height: 20%;
  flex-direction: row;
  width: 100%;
  /* flex-wrap: wrap; */
}
.item-left{
width: 20%;
margin-left: 0.5rem;
}
.item-right{
width: 80%;
}
hr{
  border-bottom: 1px solid rgba(151, 149, 149, 0.726);
  width: 100%;
  margin-top: -0.8rem;
}
strong{
  font-weight: 600;
  font-family:Arial, Helvetica, sans-serif;
  color: rgba(24, 22, 22, 0.726);
}
span{
  color: silver;
  /* padding-top: 0.5rem;
  margin-top: 0.5rem; */
}

img{width: 0.75rem;height: 0.75rem}
</style>
