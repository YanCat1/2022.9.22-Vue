<template>
  <div>
    <h1>props练习</h1>
    <h1>学校名称:{{name}}</h1>
    <h1>学校地址:{{address}}</h1>
  </div>
</template>

<script>
export default {
    name:'Student',
    data() {
        return {
            
        }
    },
    props:['name','address']
}
</script>

<style>

</style>