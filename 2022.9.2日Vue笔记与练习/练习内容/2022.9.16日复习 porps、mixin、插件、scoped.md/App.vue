<template>
  <div id="app">
    <test01></test01>
    <test02  sex="男"></test02>
  </div>
</template>

<script>
  import test01 from './components/test01.vue'
  import test02 from './components/test02.vue'

export default {
  name:'App',
  components:{
    test01,test02
  }
}
</script>

<style>

</style>