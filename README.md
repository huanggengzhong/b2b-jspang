## 学习笔记
### 一.首页布局
1.创建一个ShoppingMall组件,并设置对应的路由

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190514133424274.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3hpYW9kaTUyMDUyMA==,size_16,color_FFFFFF,t_70)
tips:安装一个插件Vue VSCode Snippets,比如使用v-base可以快速创建基本html.
同时增加简单的移动端适配
```js
  // 移动端适配
  let htmlWidth= document.documentElement.clientWidth || document.body.clientWidth;
  let htmlDom=document.getElementsByTagName('html')[0];
  htmlDom.style.fontSize=htmlWidth/20+'px';
```
2.布局
a.安装vant组件;
```js
cnpm i vant -S
```
b.配置(vant官网有介绍);
安装
```js
cnpm i babel-plugin-import -D
```
c.设置
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190514141304557.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3hpYW9kaTUyMDUyMA==,size_16,color_FFFFFF,t_70)
d.main.js按需引入

```js
import {Button,Row,Col} from 'vant'
Vue.use(Button).use(Row).use(Col);
```
测试效果
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190514141757771.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3hpYW9kaTUyMDUyMA==,size_16,color_FFFFFF,t_70)
如上,就成功了.

