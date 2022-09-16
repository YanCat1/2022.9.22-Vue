<template>
    <div>
      <h1>props练习</h1>
      <h1 @click="change">学生名称:{{name}}</h1>
      <h1>学生年龄:{{age}}</h1>
      <h1>学生性别:{{gender}}</h1>
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
      props:['name','age','gender'],
      mixins:[a]
  }
  </script>
  
  <style>
  
  </style>