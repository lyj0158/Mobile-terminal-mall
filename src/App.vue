<template>
  <my-banner></my-banner>
  <MyMenu></MyMenu>
  <MyType></MyType>
  <MyRecommend></MyRecommend>
  <MyNew></MyNew>
  <MyFoot></MyFoot>
  <div style="width: 100%;height: 100px;text-align: center;color: #8a8a8a">没有更多了</div>
</template>

<script>
import MyBanner from "@/views/MyBanner";
import MyMenu from "@/views/MyMenu";
import MyType from "@/views/MyType";
import MyRecommend from "@/views/MyRecommend";
import MyNew from "@/views/MyNew";
import MyFoot from "@/views/MyFoot";

export default {
  components: {
    MyBanner,
    MyMenu,
    MyType,
    MyRecommend,
    MyNew,
    MyFoot,
  }
}
</script>

<style>

</style>
