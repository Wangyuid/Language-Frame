  <!-- 组件结构 -->
<template>
  <div>
    <h4 @click="show">学生:{{ name }}</h4>
    <h4>学校:{{ sex }}</h4>
  </div>
</template>
<script>
import { hunru } from "../aaa";
// 组件的交互数据和方法
export default {
  name: "student",
  data() {
    return {
      name: "张三",
      sex: 18,
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
