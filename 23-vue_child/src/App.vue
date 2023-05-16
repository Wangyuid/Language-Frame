<template>
  <div>
    <h1>欢迎你</h1>
    <p>子元素要传递的数值是：{{ message }}</p>
    <School @change="getVal"></School>
    <Student :count="message"></Student>
    
  </div>
</template>

<script>
import School from './components/School.vue';
import Student from './components/Student.vue';
export default {
name:'App',
data(){
   return{
    message:'',
   };
},
  components:{
    School,
    Student,
  },
  methods:{
    getVal(val){
      this.message = val;
    },
  },
};
</script>

<style scoped>
.demo{
  color: red;
}
</style>