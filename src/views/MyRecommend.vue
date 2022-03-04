<template>
  <div class="title">
    <h2>店主推荐 <span class="titke_icon"></span><span>SELLING</span></h2>
    <span class="title_words">WELCOME TO SHOP</span>
  </div>
  <ul>
    <li v-for="item in recommend" :key="item.id">
      <a href="#" class="recommend_title">
        <img :src="require('../../src/images/recommend_0'+item.id+'.png')">
        <h6>{{item.title}}</h6>
        <span>{{item.price}}</span>
        <a href="#">立即购买 &gt;</a>
      </a>
    </li>
  </ul>
  <div class="coupon">
    <a href="#" class="coupon_a">
      <h2><span>￥</span>10</h2>
      <span>满200元使用</span>
      <span>点击领取</span>
    </a>
    <a href="#" class="coupon_a">
      <h2><span>￥</span>20</h2>
      <span>满400元使用</span>
      <span>点击领取</span>
    </a>
    <a href="#" class="coupon_a">
      <h2><span>￥</span>30</h2>
      <span>满500元使用</span>
      <span>点击领取</span>
    </a>
  </div>
</template>

<script>
export default {
  name: "MyRecommend",
  data() {
    return {
      recommend: [
        { id: 1, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
        { id: 2, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
        { id: 3, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
        { id: 4, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
        { id: 5, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
        { id: 6, title: '棉麻和风纸巾套纸巾袋纸抽袋...', price: '￥19.6' },
      ],
    };
  },
}
</script>

<style scoped>
a{
  text-decoration: none;
  display: inline-block;
  color: white;
}
.title{
  text-align: center;
  margin-bottom: 10px;
}
.title h2{
  font-weight: 800;
  margin-bottom: 0;
}
.title h2 .titke_icon{
  width: 5px;
  height: 5px;
  background: black;
  border-radius: 50%;
  margin-bottom: 7px;
  margin-right: 3px;
  display: inline-block;
}
.title .title_words{
  font-size: 12px;
  display: inline-block;
  background: url("../../src/images/title_bg.png") no-repeat;
  background-position: center top;
  padding-top: 15px;
}
.title h2 span{
  font-weight: 200;
}
ul{
  overflow: hidden;
  list-style: none;
  padding: 12px;
  margin: 0;
}
ul li{
  width: 48%;
  float: left;
}
ul li:nth-child(odd){
  margin-right: 12px;
}
ul li .recommend_title{
  overflow: hidden;
  color: #696969;
}
ul li img{
  width: 100%;
}
ul li .recommend_title h6{
  font-size: 12px;
  margin-top: 10px;
}
ul li .recommend_title span{
  float: left;
  display: inline-block;
}
ul li .recommend_title a{
  float: right;
  font-size: 12px;
  border: 1px solid #696969;
  border-radius: 50px;
  padding: 0 5px;
  color: #696969;
}
.coupon{
  padding: 0 10px;
  overflow: hidden;
  margin-bottom: 10px;
}
.coupon .coupon_a{
  width: 31%;
  float: left;
  border-radius: 8px;
  text-align: center;
}
.coupon a:nth-child(1){
  background: #d0c9c3;
}
.coupon a:nth-child(2){
  background: #c3d1d2;
  margin: 0 12px;
}
.coupon a:nth-child(3){
  background: #bebebe;
}
.coupon .coupon_a{
  position: relative;
}
.coupon .coupon_a h2{
  margin-bottom: 0;
}
.coupon .coupon_a h2 span{
  font-size: 12px;
  position: absolute;
  top: 5px;
  left: 25%;
}
.coupon .coupon_a span{
  font-size: 13px;
  display: inline-block;
}
.coupon .coupon_a span:nth-child(3){
  border: 1px solid white;
  border-radius: 20px;
  font-size: 12px;
  padding: 0 5px;
  margin-bottom: 5px;
}
</style>