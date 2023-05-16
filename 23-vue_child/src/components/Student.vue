<template>
 <div>
        <h1>student子组件</h1> 
        <p>{{ count }}</p>
    </div>
</template>
<script>
//组件的交互，数据和方法
export default {
    name:'Student',
     data() {
        return{
           
        };
     },
    props:['count'],
    };
</script>

<style scoped>

</style>