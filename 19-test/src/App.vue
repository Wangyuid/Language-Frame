<template>
  <div>
    <div class="demo">欢迎你</div>
    <school />
    <student />
  </div>
</template>

<script>
import school from "./components/school.vue";
import student from "./components/student.vue";
export default {
  name: "App",
  components: {
    school,
    student,
  },
};
</script>

<style scoped>
/* scope只对子文件起作用,对App.vue不起作用 */
.demo {
  color: red;
}
</style>