<template>
  <div class="box">
    <h1 @click="change">学校名称:{{name}}</h1>
    <h1>学校地址:{{address}}</h1>
  </div>
</template>

<script>
    import {Append} from '../mixin'
export default {
    name:'test01',
    data(){
        return{
            name:'十三中',
            address:'北京昌平'
        }
    },
    mixins:[Append]
}
</script>

<style scoped>
    .box{
        background-color:orange;
    }
</style>