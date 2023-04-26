<template>
  <div>
    <h1 v-text="msg" ref="title"></h1>
    <button ref="btn" @click="show">展示DOM</button>
    <School></School>
    <Student></Student>
    <Student studentName="李四" age="20"></Student>
  </div>
</template>

<script>
import School from "./components/Shool.vue";
import Student from "./components/Student.vue";
export default {
  name: "App",
  components: {
    School,
    Student,
  },
  data() {
    return {
      msg: "你好",
    };
  },
  methods: {
    show() {
      console.log(this.$refs);
    },
  },
};
</script>

<style>
</style>