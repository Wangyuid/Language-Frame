  <!-- 组件结构 -->
<template>
  <div class="demo">
    <h4>学校:{{ schoolName }}</h4>
    <h4>地址:{{ address }}</h4>
    <button @click="show">点我</button>
  </div>
</template>
<script>
// 组建的交互数据和方法
export default {
  name: "school",
  data() {
    return {
      schoolName: "山东商务",
      address: "烟台",
    };
  },
  methods: {
    show() {
      console.log("111");
    },
  },
};
// const school = Vue.extend({
//   data() {
//     return {
//       schoolName: "山东商务",
//       address: "烟台",
//     };
//   },
//   methods: {
//     show() {
//       console.log("111");
//     },
//   },
// });
</script>
<style>
/* 组件的样式 */
.demo {
  background-color: yellow;
}
</style>