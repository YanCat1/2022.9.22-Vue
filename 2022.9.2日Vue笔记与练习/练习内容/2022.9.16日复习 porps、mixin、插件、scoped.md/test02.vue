<template>
  <div class="box">
    <h1 @click="change">学生姓名:{{name}}</h1>
    <h1>学生性别:{{sex}}</h1>
    <h1>学生年龄：{{age}}</h1>
  </div>
</template>

<script>
    import {Append} from '../mixin'

export default {
    name:'test01',
    data() {
        return {
            
        }
    },
    props:{
        name:{
            type:String,
            default:'xxx'
        },
        age:{
            type:Number,
            default:99
        },
        sex:{

        }
    },
    mixins:[Append]
}
</script>

<style scoped>
    .box{
        background-color: skyblue;
    }
</style>