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

4.模板语法
v-text,v-html
5.计算属性方法侦听器
解决计算属性的方式有三种：
        1：computed:具有缓存机制，性能最高，代码量少
        2：watch:性能较高，代码量复杂一点，优点可以实时监测数据变化
        3：methods：方法去计算属性，需要再插值表达式中添加括号表示方法的引用,性能最低

```


