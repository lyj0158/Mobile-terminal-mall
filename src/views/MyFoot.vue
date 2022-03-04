<template>
  <ul>
    <li v-for="item in advantage" :key="item.id">
      <a href="#">
        <img :src="require('../../src/images/advantage_0'+item.id+'.png')">
        <span>{{item.text}}</span>
        <span>{{item.english}}</span>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "MyFoot",
  data() {
    return {
      advantage:[
        { id: 1, text: '专业售后', english: 'intimate' },
        { id: 2, text: '七天退换', english: '7 days return' },
        { id: 3, text: '品质保证', english: 'quality' },
        { id: 4, text: '实物拍摄', english: 'real shots' },
      ],
    };
  },
}
</script>

<style scoped>
ul{
  overflow: hidden;
  list-style: none;
  padding: 10px 30px;
  background: #f3f3f3;
}
ul li{
  float: left;
  width: 24%;
  text-align: center;
  margin-right: 1%;
}
ul li:last-child{
  margin-right: 0;
}
ul li a{
  text-decoration: none;
}
ul li img{
  width: 70%;
}
ul li a span:nth-child(2){
  color: #555555;
  font-weight: 600;
  font-size: 12px;
  display: block;
}
ul li a span:last-child{
  color: #818181;
  font-size: 12px;
  letter-spacing: 0px;
}
@media screen and (max-width:390px){
  ul{
    padding: 10px 9px;
  }
}
</style>