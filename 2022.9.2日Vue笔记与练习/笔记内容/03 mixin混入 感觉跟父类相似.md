相当于我们新建了 一个父文件，子文件使用父文件中的内容

过程 是 我们新建一个xx.js 以mixin.js为例 



##### 局部混入~~mixin.js~~

```vue
export const mixin = {
	methods:{
		showName(){
			alert(this.name)
		}
	},
	mounted(){
		console.log('挂载元素')
	}
}
```

以上 我们已经设置好了共有内容，需要在组件中进行引入使用

**Student.vue**

```vue
<script>
	import {mixin,xxx,xxx,xxx} from '../mixin'
	export default{
		
	}
</script>
```

我们可以在引入语句中 引入多个混合文件

**~~全局混入~~**

我们还是先新建一个混合文件 mixin.js

之后在 main.js 中 进行引入

```vue
import {hunhe1,hunhe2,xxxx} from './mixin'
```

引入后进行使用

```vue
Vue.mixin(hunhe1)
Vue.mixin(hunhe2)
Vue.mixin(xxx)
Vue.mixin(xxx)
```

这个就需要分别混合了，而不是多个一起单独混合，

这样我们混合使用后 所有的组件 都会有我们混合文件的内容

包括 App组件















