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

6.条件渲染
v-if  v-show

7.样式绑定

通过style对样式进行绑定
1）.对象绑定  style="styleObj"
    数组绑定  style="[styleObj,{fontSize:20px}]"

2).class样式绑定

	对象绑定  v-bind:class={"actived":"isActivied"}
	数组绑定  v-class="[activied,activiedOne,activiedTwo]"


8.组件深入
1） <tr is="row"></tr>  row为自定的组件   页面元素是tr但是实际渲染的是component组件
2） ref dom元素引用  this.$refs.conterRefOne.number是vue实例下conterRefOne组件的number值
    this.$emit（'change'）子组件触发父组件的自定义事件
```


