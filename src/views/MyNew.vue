<template>
  <div class="title">
    <h2>新品上市 <span class="titke_icon"></span><span>SELLING</span></h2>
    <span class="title_words">WELCOME TO SHOP</span>
  </div>
  <ul class="news">
    <li v-for="item in news" :key="item.id">
      <a href="#">
        <img :src="require('../../src/images/new_0'+item.id+'.png')">
      </a>
      <div class="news_right">
        <h3>{{item.title}}</h3>
        <p>日式镂空桌面收纳蓝塑料收筐厨房零食收纳盒化...</p>
        <div>
          <span>￥39.0</span>
          <a href="#">立即购买 &gt;</a>
        </div>
      </div>
    </li>
  </ul>
  <div class="accept">
    <div class="accept_title">
      <h3>收纳整理<span></span><span>SELLING</span><a href="#">查看更多 &gt;</a></h3>
    </div>
    <ul>
      <li v-for="item in accept" :key="item.id">
        <a href="#">
          <img :src="require('../../src/images/aceept_0'+item.id+'.png')">
          <h4>宝贝标题宝贝...</h4>
          <span>￥23.8</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MyNew",
  data() {
    return {
      news:[
        { id: 1, title: '桌面收纳篮' },
        { id: 2, title: '素色抽屉盒' },
        { id: 3, title: '厨房去污刷' },
      ],
      accept: [
        { id: 1 },
        { id: 2 },
        { id: 3 },
        { id: 4 },
        { id: 5 },
        { id: 6 },
        { id: 7 },
        { id: 8 },
      ],
    };
  },
}
</script>

<style scoped>
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
  list-style: none;
  padding: 0 10px;
}
.news li{
  overflow: hidden;
  margin: 10px 0;
  padding-bottom: 10px;
  border-bottom: 1px solid #f0f0f0;
}
.news li a{
  display: inline-block;
  float: left;
  width: 48%;
  margin-right: 15px;
}
.news li img{
  width: 100%;
}
.news li .news_right{
  padding-top: 20px;
  float: left;
  width: 45%;
}
.news li .news_right h3{
  font-size: 15px;
}
.news li .news_right p{
  font-size: 12px;
  color: #8a8a8a;
}
.news li .news_right div{
  width: 100%;
  padding-right: 10%;
  background: url("../../src/images/new_icon.png") no-repeat;
  background-size: 30px;
  overflow: hidden;
}
.news li .news_right div span{
  display: block;
  text-align: right;
  color: #3c3c3c;
  padding-right: 20px;
}
.news li .news_right div a{
  display: block;
  width: auto;
  padding: 0 5px;
  float: right;
  margin-right: 0;
  text-decoration: none;
  color: #8a8a8a;
  font-size: 12px;
  border: 1px solid #8a8a8a;
  border-radius: 20px;
}
.accept{
  background: #e1ebec;
  padding-bottom: 10px;
}
.accept .accept_title{
  background: #c3d1d2;
  padding: 10px;
  color: white;
}
.accept .accept_title h3{
  margin-bottom: 0;
  font-size: 18px;
}
.accept .accept_title h3 span:first-child{
  width: 5px;
  height: 5px;
  background: white;
  display: inline-block;
  margin: 0 5px;
  margin-bottom: 5px;
  border-radius: 50%;
}
.accept .accept_title h3 span:nth-child(2){
  font-weight: 200;
}
.accept .accept_title h3 a{
  text-decoration: none;
  color: white;
  font-size: 12px;
  font-weight: 200;
  float: right;
  display: inline-block;
  border: 1px solid white;
  border-radius: 20px;
  padding: 0 8px;
  line-height: 20px;
}
.accept ul{
  background: #f8f6f9;
  border: 5px solid #f8f6f9;
  margin: 10px;
  padding: 0;
  overflow: hidden;
  margin-bottom: 0;
}
.accept ul li{
  float: left;
  width: 24%;
  margin-right: 1.3%;
  background: white;
}
.accept ul li:nth-child(4){
  margin-right: 0;
}
.accept ul li:nth-child(8){
  margin-right: 0;
}
.accept ul li a{
  display: inline-block;
  color: #3c3c3c;
  text-decoration: none;
  text-align: center;
}
.accept ul li a img{
  width: 100%;
}
.accept ul li a h4{
  font-size: 12px;
  margin-bottom: 0;
}
.accept ul li a span{
  font-size: 13px;
}
</style>