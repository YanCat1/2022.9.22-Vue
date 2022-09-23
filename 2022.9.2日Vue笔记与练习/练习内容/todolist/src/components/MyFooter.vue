<template>
  <div class="todo-footer">
    <label for="">
        <input type="checkbox">
    </label>
    <span>
        <span>已完成0</span>/全部2
    </span>
    <button class="btn btn-danger">清除已完成</button>
  </div>
</template>

<script>
export default {
    name:'MyFooter'
}
</script >

<style scoped>
    .todo-footer{
        height:40px;
        line-height:40px;
        padding-left:6px;
        margin-top:5px;
    }
    .todo-footer label{
        display:inline-block;
        margin-right:20px;
        cursor:pointer;
    }
    .todo-footer label input{
        position:relative;
        top:-1px;
        vertical-align:middle;
        margin-right:5px;
    }
    li button{
        float:right;
        display:none;
        margin-top:3px;
    }
    li:before{
        content:initial;
    }
    li:last-child{
        border-bottom:none;
    }

</style>