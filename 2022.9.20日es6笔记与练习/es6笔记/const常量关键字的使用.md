我们想要声明一个 常量 需要使用 const关键字

它必须要进行赋值，不赋值会报错

```javascript
const NAME = 'YZD'
常量潜规则 变量名大写
```

常量的值不能进行修改，跟元素数据相似，修改就报错；

但是如果常量声明的是一个数组或者对象时 我们操作其进行元素增删

不会报错

```javascript
const TEAME = ['yzd','yzd1','yzd2']
TEAM.push('yzd3')
log(TEAM)			//yzd,yzd1,yzd2,yzd3
```



但是我们如果直接修改TEAM就会报错了

```javascript
const TEAM = ['yzd','yzd1','yzd2']
TEAM  = 'aaa'			//报错
```

所以 const适合声明数组和对象时使用 也会防止一些误操作

