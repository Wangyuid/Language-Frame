<template>
  <div id="main">
    <button @click="down">-</button>
    <div class="center">{{ count }}</div>
    <button @click="up">+</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    up() {
      if (this.count < 10) {
        this.count++;
      } else {
        alert("不能再加了!");
      }
    },
    down() {
      if (this.count > 1) {
        this.count--;
      } else {
        alert("不能再减了!");
      }
    },
  },
};
</script>

<style>
#main {
  float: left;
}
button {
  display: inline-block;
  width: 50px;
  height: 30px;
  background-color: #c7c7c7;
}
.center {
  display: inline-block;
  width: 50px;
  height: 30px;
  text-align: center;
  line-height: 30px;
}
</style>