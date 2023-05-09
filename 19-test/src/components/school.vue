  <!-- 组件结构 -->
<template>
  <div>
    <h4 @click="show">学校:{{ name }}</h4>
    <h4>地址:{{ address }}</h4>
  </div>
</template>
<script>
import { hunru } from "../aaa";
// 组建的交互数据和方法
export default {
  name: "school",
  data() {
    return {
      name: "山东商务",
      address: "烟台",
    };
  },
  methods: {
    show() {
      alert(this.name);
    },
  },
  mixins: [hunru],
};
</script>
<style>
/* 组件的样式 */
</style>
