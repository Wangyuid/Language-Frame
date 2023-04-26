  <!-- 组件结构 -->
<template>
  <div>
    <h4>学生:{{ studentName }}</h4>
    <h4>学校:{{ age }}</h4>
  </div>
</template>
<script>
// 组建的交互数据和方法
export default {
  name: "Student",
  data() {
    return {
      studentName: "张三",
      age: 18,
    };
  },
};
</script>