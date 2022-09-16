我们在写样式时  经常会遇到这种问题 就是样式的class名重复了

我们可以在style标签中添加 scoped 关键字

```vue
<style scoped>
	
</style>
```

它会给标签生成一个属性，然后根据属性选择器 给指定元素进行添加



其实style标签还有一个lang属性 用来写语言的

可以用less和sass，但是需要看下版本