<template>
  <div id="app">
    <student name="yzd" :age="13" gender="男"></student>
    <school name="十三中" address="北京昌平"></school>
  </div>
</template>

<script>
  import student from './components/Student.vue'
  import school from './components/School.vue'
export default {
  name:'App',
  components:{
    student,school
  }
}
</script>

<style>

</style>