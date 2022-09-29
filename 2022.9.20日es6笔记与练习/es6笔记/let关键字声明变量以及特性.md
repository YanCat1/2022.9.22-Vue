在es6语法中 我们可以使用 let关键字 声明某个变量,也可以声明多个变量

```javascript
let a = 13
let b,c,d;
let e = 100;
let f = 521,g = 'i love you',h=[]
```

~~let 变量的特性:~~

​		不能声明多个变量名相同的变量

```javascript
let start = 'aaa'
let start = 'bbb'
会报错，防止重名 全局污染
```



~~块级作用域~~：

```javascript
{
	let boy = 'yzd'
}
log(boy)			//会报错
```

if while for中的 { }我们也看作是块级作用域

在其中定义变量是局部的 

虽然是块级作用域 但是不会影响作用域链比如:

```javascript
{
	let name = 'yzd'
	function fn(){
		log(name)		//输出  yzd
	}
}
```

我们刚才说了 函数的{ } 也是一个块级作用域，我们的name变量 定义在作用域以外

是通过作用域链找到上一级的元素 进行使用的；

案例:	

```javascript
<h2>点击切换颜色</h2>
<div id="box">
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
</div>

<script>
    let item = document.querySelectorAll('.item')
    for(let i=0;i<item.length;i++){
        item[i].onclick=function(){
            for(j=0;j<item.length;j++){
                item[j].style.background=''
            }
            item[i].style.background='pink'
        }
    }
</script>
```

其中的for循环 如果我们不写let  直接用var

下面的 item[i]我们是找不到的，得用this，但是如果我们使用了let

那么可以在当前作用域中 找到现在的i是几，从而完成点击变色效果；



