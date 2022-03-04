<template>
  <div class="overflow">
    <ul class="menu left">
      <li v-for="item in menu" :key="item.id">
        <a href="#">
          {{item.type}}
        </a>
      </li>
    </ul>
    <div class="show left">
      <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img src="../.././src/images/show.png" class="d-block w-100" alt="...">
          </div>
          <div class="carousel-item">
            <img src="../.././src/images/show.png" class="d-block w-100" alt="...">
          </div>
          <div class="carousel-item">
            <img src="../.././src/images/show.png" class="d-block w-100" alt="...">
          </div>
        </div>
      </div>
      <div class="recommend">
        <div>
          <h4>压圈垃圾桶</h4>
          <span>多色可选简约设计</span>
          <a href="#">热卖款</a>
        </div>
        <div style="width: 5px; background: #f1f1f1;padding: 0"></div>
        <div>
          <h4>进口棉毛巾</h4>
          <span>纯棉质地 柔软舒适</span>
          <a href="#">热卖款</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Menu",
  data() {
    return {
      menu: [
        { id:1, type: '收纳专区' },
        { id:2, type: '厨房专区' },
        { id:3, type: '清洁用品' },
        { id:4, type: '卫浴专区' },
        { id:5, type: '居家日用' },
        { id:6, type: '个人洗护' },
      ],
    };
  },
}
</script>

<style scoped>
.overflow{
  overflow: hidden;
  background: #f1f1f1;
}
.left{
  float: left;
}
a{
  color: #696969;
  text-decoration: none;
}
.menu{
  width: 30%;
  list-style: none;
  padding: 0;
  margin: 0;
}
.menu li{
  background: white;
  margin: 5px;
  margin-left: 0;
  padding: 8px;
  padding-left: 0px;
}
.menu li a{
  display: inline-block;
  padding-left: 33px;
  background-position: 6% 50% !important;
  background-size: 30px !important;
}
.menu li:nth-child(1) a{
  background: url("../../src/images/menu_01.png") no-repeat;
}
.menu li:nth-child(2) a{
  background: url("../../src/images/menu_02.png") no-repeat;
}
.menu li:nth-child(3) a{
  background: url("../../src/images/menu_03.png") no-repeat;
}
.menu li:nth-child(4) a{
  background: url("../../src/images/menu_04.png") no-repeat;
}
.menu li:nth-child(5) a{
  background: url("../../src/images/menu_05.png") no-repeat;
}
.menu li:nth-child(6) a{
  background: url("../../src/images/menu_06.png") no-repeat;
}
.show{
  width: 70%;
  margin-top: 5px;
}
.show .slide .carousel-inner .carousel-item img{
  height: 175px;
}
.show .recommend{
  overflow: hidden;
  margin: 5px 0;
  background: white;
}
.show .recommend div{
  width: 49%;
  float: left;
  height: 85px;
  padding: 5px;
  background-position: right bottom !important;
  background-size: 70% 70% !important;
}
.show .recommend div h4{
  color: #535353;
  font-size: 14px;
  font-weight: 700;
  margin-bottom: 2px;
}
.show .recommend div span{
  color: #535353;
  font-size: 12px;
  display: block;
}
.show .recommend div a{
  display: inline-block;
  background: #fe5e3c;
  color: white;
  border-radius: 20px;
  font-size: 12px;
  padding: 0 8px;
  margin-top: 20px;
}
.show .recommend div:nth-child(1){
  background: url("../../src/images/hot_01.png") no-repeat;
}
.show .recommend div:nth-child(3){
  background: url("../../src/images/hot_02.png") no-repeat;
}
</style>