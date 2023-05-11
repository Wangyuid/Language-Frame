  <!-- 组件结构 -->
<template>
  <div class="demo">
    <h4 @click="show">学校:{{ name }}</h4>
    <h4>地址:{{ address }}</h4>
  </div>
</template>
<script>
import { hunru, hunru2 } from "../aaa";
// 组建的交互数据和方法
export default {
  name: "school",
  data() {
    return {
      name: "山东商务",
      address: "烟台",
      a: 8888,
    };
  },
  methods: {
    show() {
      alert(this.name);
    },
  },
  mixins: [hunru, hunru2],
};
</script>
<style scoped>
/* 组件的样式 */
.demo {
  background-color: blue;
}
</style>
