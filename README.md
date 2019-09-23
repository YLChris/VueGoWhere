VueGoWhere
# vue1基本讲解 
```
1.组件  
Vue.component('item',{
	props:['aaacontent']
	template:'<h1>abc</h1>'
})
此时则可以使用item进行在页面使用该组件了（<item></item>）

子组件传值到父组件：v-bind:aaacontent='aaa',则在组件中需要使用props注册一个aaacontent属性

2.实例
每一个组件都是一个实例


3.监听
v-on:click可以简写为@click
```


