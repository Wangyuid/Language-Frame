<template>
 <div> 
    <h1>school子组件</h1>
        <button @click="fn">点击传递</button>
    </div>
</template>
<script>
//组件的交互，数据和方法
export default {
    name:'School',
     data() {
        return{
            cMsg:'子组件要传递当代信息',
        };
     },
     methods:{
        fn(){
           this.$emit("change",this.cMsg);
        },
     }
     
    };
</script>

<style>

</style>