<template>
  <div>
    <p>父子组件通信，父组件msg值</p>
    <child-componet :message="msg" v-on:getChildData="getData"></child-componet>
  </div>
</template>
<script>
import childComponet from "./components/childComponents.vue";
export default {
  components: {
    childComponet,
  },
  data(){
    return{
        msg: "测试一下",
    };
  },
  methods:{
    getData(val){
        this.msg=val;
    },
  },
};
</script>