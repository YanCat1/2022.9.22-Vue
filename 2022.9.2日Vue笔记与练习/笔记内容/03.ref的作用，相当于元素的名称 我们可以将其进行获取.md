在脚手架中，进行元素的获取

一个元素

```vue
<template>
	<h1 @click='showDom' $refs='title'>{{msg}}</h1>
	<button ref='btn'></button>
</template>

methods:{
	showDom(){
		log(this.$refs.title)
		log(this.$refs.btn)
	}
}
这样会输出该元素
<h1 @click='showDom' $refs='title'>{{msg}}</h1>
<button ref='btn'></button>
```

ref就相当于id或者class

而 this.$refs.title 就是找到ref为title的元素

我们可以通过这种方式 进行元素的获取



在之后组件之间的通信会有作用