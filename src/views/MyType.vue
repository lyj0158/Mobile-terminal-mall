<template>
  <ul>
    <li v-for="item in type" :key="item.id">
      <a href="#">{{item.name}}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "MyType",
  data() {
    return {
      type: [
        { id:1, name: '收纳整理' },
        { id:2, name: '厨房用品' },
        { id:3, name: '清洁卫生' },
        { id:4, name: '卫浴用品' },
        { id:5, name: '居家用品' },
        { id:6, name: '办公文具' },
        { id:7, name: '食品保鲜' },
        { id:8, name: '美容工具' },
      ],
    };
  },
}
</script>

<style scoped>
a{
  text-decoration: none;
  color: #919191;
}
ul{
  padding: 20px;
  overflow: hidden;
  list-style: none;
  padding-bottom: 0;
}
ul li{
  float: left;
  width: 25%;
  text-align: center;
}
ul li a{
  width: 100%;
  display: inline-block;
  font-size: 13px;
  padding-top: 80px;
  background-size: 70px !important;
  background-position: center top !important;
}
ul li:nth-child(1) a{
  background: url("../../src/images/type_01.png") no-repeat;
}
ul li:nth-child(2) a{
  background: url("../../src/images/type_02.png") no-repeat;
}
ul li:nth-child(3) a{
  background: url("../../src/images/type_03.png") no-repeat;
}
ul li:nth-child(4) a{
  background: url("../../src/images/type_04.png") no-repeat;
}
ul li:nth-child(5) a{
  background: url("../../src/images/type_05.png") no-repeat;
}
ul li:nth-child(6) a{
  background: url("../../src/images/type_06.png") no-repeat;
}
ul li:nth-child(7) a{
  background: url("../../src/images/type_07.png") no-repeat;
}
ul li:nth-child(8) a{
  background: url("../../src/images/type_08.png") no-repeat;
}
</style>