<template>
  <div>
    <h1>props练习</h1>
    <h1 @click="change">学校名称:{{name}}</h1>
    <h1>学校地址:{{address}}</h1>
  </div>
</template>

<script>
    import {a} from '../change'
export default {
    name:'Student',
    data() {
        return {
            
        }
    },
    props:['name','address'],
    mixins:[a]
}
</script>

<style>

</style>