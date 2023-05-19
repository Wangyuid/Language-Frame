<template>
  <input type="text" v-model="myMessage" @input="passData(myMessage)" />
</template>
<script>
export default {
  name: "childComponent",
  data() {
    return {
      myMessage: this.message,
    };
  },
  props: {
    message: String,
  },
  methods: {
    passData(val) {
      this.$emit("getChildData");
    },
  },
};
</script>