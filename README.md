
- [$css和html](#css和html)
  - [Doctype作用？标准模式和兼容模式区别](#Doctype作用？标准模式和兼容模式区别)
  - [行内元素有哪些？块级元素有哪些？](#行内元素有哪些？块级元素有哪些？)
  - [引入样式link和import区别](#引入样式link和import区别)
  - [HTML5有哪些新特性？如何区分html和html5](#HTML5有哪些新特性？如何区分html和html5)
  - [html语义化理解](#html语义化理解)
  - [不使用borer新建一个1像素的横线](#不使用borer新建一个1像素的横线)
  - [两个盒子用一个css属性实现让一个盒子在左边一个盒子在右边并且在一行](#两个盒子用一个css属性实现让一个盒子在左边一个盒子在右边并且在一行)
  - [css垂直和水平居中方法](#css垂直和水平居中方法)
  - [清除浮动](#清除浮动)
  - [介绍一下css盒模型](#介绍一下css盒模型)
  - [position有几个值](#position有几个值)
  - [css创建三角形](#css创建三角形)
  - [为什么要初始化css样式](#为什么要初始化css样式)
  - [css新增伪类元素](#css新增伪类元素)
  - [css新特性](#css新特性)
- [$javascript](#javascript)
  - [js基本类型](#js基本类型)
  - [js基本类型规范](#js基本类型规范)
  - [定义函数](#定义函数)
  - [原型链](#原型链)
  - [js继承](#js继承)
  - [js作用域链](#js作用域链)
  - [this指向](#this指向)
  - [null与undefined](#null与undefined)
  - [eval题](#eval)
  - [window对象和document对象](#window对象和document对象)
  - [什么是闭包？闭包特性](#什么是闭包？闭包特性)
  - [什么是js严格模式](#什么是js严格模式)
  - [如何创建ajax](#如何创建ajax)
  - [同步和异步区别](#同步和异步区别)
  - [操作dom节点](#操作dom节点题)
  - [数组的方法](#数组的方法)
  - [更改this指向](#更改this指向)
  - [jquery.extend 与 jquery.fn.extend的区别？](#jquery.extend 与 jquery.fn.extend的区别？)
  - [作用域](#作用域)
  - [同源策略](#同源策略)
  - [http状态码有那些？分别代表是什么意思？](#http状态码有那些？分别代表是什么意思？)
  - [$一个页面从输入 URL 到页面加载显示完成，这个过程中都发生了什么？（流程说的越详细越好）](#一个页面从输入 URL 到页面加载显示完成，这个过程中都发生了什么？（流程说的越详细越好）)
- [$vue](#vue)
  - [对于mvvm的理解](#对于mvvm的理解)
  - [Vue实现数据双向绑定的原理：Object.defineProperty（）](#Vue实现数据双向绑定的原理：Object.defineProperty（）)
  - [Vue组件间的参数传递](#Vue组件间的参数传递)
  - [Vue的路由实现:hash模式 和 history模式](#Vue的路由实现:hash模式 和 history模式)
  - [Vue与React的区别？](#Vue与React的区别？)
  - [vue路由的钩子函数](#vue路由的钩子函数)
  - [vuex是什么？怎么使用？哪种功能场景使用它？](#vuex是什么？怎么使用？哪种功能场景使用它？)
- [$微信小程序](#微信小程序)
  - [微信小程序有几个文件题](#微信小程序有几个文件)
  - [微信小程序组件封装](#微信小程序组件封装)
  - [微信小程序怎样跟事件传值](#微信小程序怎样跟事件传值)
  - [小程序的wxss和css有哪些不一样的地方？](#小程序的wxss和css有哪些不一样的地方？)
  - [小程序关联微信公众号如何确定用户的唯一性？](#小程序关联微信公众号如何确定用户的唯一性？)
  - [微信小程序怎样获取用户信息](#微信小程序怎样获取用户信息)
  - [微信小程序与vue区别](#微信小程序与vue区别)


## css和html
### Doctype作用？标准模式和兼容模式区别。

声明在HTML文档第一行，告诉浏览器用什么文档标准解析这个文档。DOCTYPE不存在或格式不正确会导致文档以兼容模式呈现。

### 标准模式的排版 和JS运作模式都是以该浏览器支持的最高标准运行。在兼容模式中，页面以宽松的向后兼容的方式显示,模拟老式浏览器的行为以防止站点无法工作。

### 行内元素有哪些？块级元素有哪些？

每个元素都有一个diaplay属性，确定该元素的类型，比如块级元素默认值就是block,行内元素就是none

行内元素：span a u i b img input slect。。。

块级元素：div p ul li ol h1 h2。。。

### 引入样式link和import区别

link属于html直接是在html中引入，import在css中引入只能引入css

link在直接引入页面的时候就就已经引入了，import需要在引入css的时候才引入，性能比较低。

import是CSS2.1 提出的，只在IE5以上才能被识别，而link是html标签，无兼容问题;

### HTML5有哪些新特性？如何区分html和html5

html5新增了好多东西比如：

一些语义化标签 nav header footer

绘图用到的canvas

用于媒体的video 和 audio 元素

本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失，sessionStorage 的数据在浏览器关闭后自动删除;

表单控件，calendar、date、time、email、url、search

区分html5和html：

可以按上文说的doctype区分也可以使用标签区分

### html语义化理解:

语义化是html结构更清晰，便于浏览器解析，利于SEO搜素，使代码更好理解，便于维护

### 不使用borer新建一个1像素的横线

```  
<div style="height: 1px;background:red;overflow:hidden;"></div>
```  
### 两个盒子用一个css属性实现让一个盒子在左边一个盒子在右边并且在一行


```
    <div style="width: 100px;height: 100px;background:red;float: right;"></div>
    <div style="width: 100px;height: 100px;background:blue;"></div>
```  
### css垂直和水平居中方法

使用position定位：好处不用管盒子大小，就是不固定宽高

```
{
    position: absolute;;
    top: 50%;
    left: 50%;
    margin-left: -50%;
    margin-top: -50%;
}
```
也可以使用calc计算出需要定位的值，需要知道宽高

还可以使用transform: translate(-50%, -50%); 不需要知道宽高

固定宽高的话也可以使用定位

```
{
    position: absolute;;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
}
```
也可以使用flex
```
{
    display: flex;
    justify-content: center;
    align-items: center;
}
```
或者使用最新的grid，父元素必须加grid属性

```
{
    align-self: center;
    justify-self: center;
}
```
还有一种使用table居中缺点也是父盒子宽高为100%必须加display:table;

```
{
    display: table-cell;
    text-align: center;
    vertical-align: middle;
}
```
8.清除浮动

清除浮动最好的方法就是使用:after

```
:after { 
clear:both;
content:'';
display:block;
width:0;
height:0;
}
```
也可以先新建一个空元素来清除浮动

```
.clear{ 
clear:both; 
height:0; 
line-height:0; 
font-size:0; 
}
```
还可以给父元素增加overflow属性


.over-flow{ overflow:auto; zoom:1;  }//zoom:1;是在处理兼容性问题
### 介绍一下css盒模型

分为两种：ie盒模型和w3c盒模型

盒模型：内容(content)、填充(padding)、边界(margin)、 边框(border)；

区别：IE的content部分把 border 和 padding计算了进去;

### position有几个值

absolute 生成绝对定位的元素，相对于值不为 static的第一个父元素进行定位。

fixed 绝对定位，相对于浏览器窗口定位

reactive 相对定位，对于正常元素定位

static 默认值，没有定位

inherit 从父元素继承position属性

###  css创建三角形

```
{
  width: 0;
  height: 0;
  border-width: 20px;
  border-style: solid;
  border-color: transparent transparent red transparent;
}
```
###  为什么要初始化css样式

因为浏览器的兼容问题，不同浏览器对有些标签的默认值是不同的，如果没对CSS初始化往往会出现浏览器之间的页面显示差异

最简单的初始化方法： * {padding: 0; margin: 0;} （强烈不建议）

###  css新增伪类元素

:nth-child :after :befor :checked :disable

###  css新特性

transform ：translate scale skew rotate； transtion ；animation ；shadow ；border-radius

## javascript
###  js基本类型

js有五种基本类型：boolean string number null undefined 一种特殊类型：object

新增了Symbol(创建后独一无二且不可变的数据类型 )

###  js基本规范

不在同一行声明多个变量 不用全局函数 switch必须有default

###  定义函数

函数声明 function name（）{}

函数表达式 var name = function（）{}

new实例化（不常用）

###  原型链

简单来说就是每个对象对会在内部初始化一个属性 prototype 如果这个对象不存在这个属性 会在prototype上找 这个prototype又会自己往上找 prototype

###  js继承

构造函数 

优点：实现多个继承，实现子类可以向父类传递参数 

缺点：无法实现复用影响性能，只能继承父类方法 不能继承原型上的 

原型链继承 

优点：实现简单，父类新增原型方法子类可访问 

缺点：无法实现多个继承 创造子类实例时无法向父类构造函数传参 

拷贝继承 

优点：支持多继承 

缺点：效率低 内存占用高 

 实例继承 

优点：不限制调用方式

缺点：不支持多继承 

组合继承  

优点：可传参，可复用，可以继承原型链上的东西 既是子类实例又是父类实例 

缺点：调用了两次父类构造函数 多耗费了一点内存 

寄生式组合继承 

优点：完美 

缺点：实现复杂

###  js作用域链

作用域链的作用是保证执行环境里有权访问的变量和函数是有序的，作用域链的变量只能向上访问，变量访问到window对象即被终止，作用域链向下访问变量是不被允许的。

21.this指向

this指向直接调用者 

this指向new出来的对象 

在事件中this指向这个事件的对象 IE中的attachEvent的this指向全局window

thi指的当前对象

###  null与undefined

null 表示一个对象被定义了，值为“空值”； 

undefined 表示不存在这个值。 

null==undefined true

### eval

解析字符串，应该避免使用eval，不安全，非常耗性能（2次，一次解析成js语句，一次执行），也可以把JSON字符串转换为JSON对象

### window对象和document对象

window对象是指浏览器打开的窗口。

document对象是Documentd对象（HTML 文档对象）的一个只读引用，window对象的一个属性

### 什么是闭包？闭包特性

闭包是指有权访问另一个函数作用域中变量的函数，创建闭包的最常见的方式就是在一个函数内创建另一个函数，通过另一个函数访问这个函数的局部变量,利用闭包可以突破作用链域，将函数内部的变量和方法传递到外部。 

特性：

函数内再嵌套函数

内部函数可以引用外层的参数和变量

参数和变量不会被垃圾回收机制回收

### 什么是js严格模式

严格模式就是在js代码前加 use strict 让 Javascript 在更严格的条件下运行,使JS编码更加规范化的模式,消除Javascript语法的一些不合理、不严谨之处，减少一些怪异行为。

### 如何创建ajax


```
/* 封装ajax函数
 * @param {string}opt.type http连接的方式，包括POST和GET两种方式
 * @param {string}opt.url 发送请求的url
 * @param {boolean}opt.async 是否为异步请求，true为异步的，false为同步的
 * @param {object}opt.data 发送的参数，格式为对象类型
 * @param {function}opt.success ajax发送并接收成功调用的回调函数
 */
    function ajax(opt) {
        opt = opt || {};
        opt.method = opt.method.toUpperCase() || 'POST';
        opt.url = opt.url || '';
        opt.async = opt.async || true;
        opt.data = opt.data || null;
        opt.success = opt.success || function () {};
        var xmlHttp = null;
        if (XMLHttpRequest) {
            xmlHttp = new XMLHttpRequest();
        }
        else {
            xmlHttp = new ActiveXObject('Microsoft.XMLHTTP');
        }var params = [];
        for (var key in opt.data){
            params.push(key + '=' + opt.data[key]);
        }
        var postData = params.join('&');
        if (opt.method.toUpperCase() === 'POST') {
            xmlHttp.open(opt.method, opt.url, opt.async);
            xmlHttp.setRequestHeader('Content-Type', 'application/x-www-form-urlencoded;charset=utf-8');
            xmlHttp.send(postData);
        }
        else if (opt.method.toUpperCase() === 'GET') {
            xmlHttp.open(opt.method, opt.url + '?' + postData, opt.async);
            xmlHttp.send(null);
        } 
        xmlHttp.onreadystatechange = function () {
            if (xmlHttp.readyState == 4 && xmlHttp.status == 200) {
                opt.success(xmlHttp.responseText);
            }
        };
    }
```   
### 同步和异步区别

同步：浏览器访问服务器请求，用户看得到页面刷新，重新发请求,等请求完，页面刷新，新内容出现，用户看到新内容,进行下一步操作

异步：浏览器访问服务器请求，用户正常操作，浏览器后端进行请求。等请求完，页面不刷新，新内容也会出现，用户看到新内容

### 操作dom节点

creatElement（）具体元素 

creatTextNode（）创建文本节点

appendChild（）添加 

removeChild（）删除 

replaceChild（）替换 

insertChild（）插入

### 数组的方法

push（）pop（）unshift（）shift（）splice（）indexOf（）sort（）concat（）jion（）slice（）reverse（） includes（）

### 更改this指向

.call() .apply() .bind()

### jquery.extend 与 jquery.fn.extend的区别？

jquery.extend 为jquery类添加类方法，可以理解为添加静态方法

jquery.fn.extend:源码中jquery.fn = jquery.prototype，所以对jquery.fn的扩展，就是为jquery类添加成员函数 使用：

jquery.extend扩展，需要通过jquery类来调用，而jquery.fn.extend扩展，所有jquery实例都可以直接调用

### 作用域

作用域 每个方法都是作用域最大的是window 

作用域的方法和属性只能在当前作用域使用 

查找作用域 是从当前查找 再去上一级查找

### 同源策略

同域名 同端口 同协议

### http状态码有那些？分别代表是什么意思？

100 Continue	继续，一般在发送post请求时，已发送了http header之后服务端将返回此信息，表示确认，之后发送具体参数信息

200 OK 正常返回信息

201 Created 请求成功并且服务器创建了新的资源

202 Accepted 服务器已接受请求，但尚未处理

301 Moved Permanently 请求的网页已永久移动到新位置。

302 Found 临时性重定向。

303 See Other 临时性重定向，且总是使用 GET 请求新的 URI。

304 Not Modified 自从上次请求后，请求的网页未修改过。

400 Bad Request 服务器无法理解请求的格式，客户端不应当尝试再次使用相同的内容发起请求。

401 Unauthorized 请求未授权。

403 Forbidden 禁止访问。

404 Not Found 找不到如何与 URI 相匹配的资源。

500 Internal Server Error 最常见的服务器端错误。

503 Service Unavailable 服务器端暂时无法处理请求（可能是过载或维护）

### 一个页面从输入 URL 到页面加载显示完成，这个过程中都发生了什么？（流程说的越详细越好）

1、浏览器会开启一个线程来处理这个请求，对 URL 分析判断如果是 http 协议就按照 Web 方式来处理;

2、调用浏览器内核中的对应方法，比如 WebView 中的 loadUrl 方法;

3、通过DNS解析获取网址的IP地址，设置 UA 等信息发出第二个GET请求;

4、进行HTTP协议会话，客户端发送报头(请求报头);

5、进入到web服务器上的 Web Server，如 Apache、Tomcat、Node.JS 等服务器;

6、进入部署好的后端应用，如 PHP、Java、JavaScript、Python 等，找到对应的请求处理;

7、处理结束回馈报头，此处如果浏览器访问过，缓存上有对应资源，会与服务器最后修改时间对比，一致则返回304;

8、浏览器开始下载html文档(响应报头，状态码200)，同时使用缓存;

9、文档树建立，根据标记请求所需指定MIME类型的文件（比如css、js）,同时设置了cookie;

10、页面开始渲染DOM，JS根据DOM API操作DOM,执行事件绑定等，页面显示完成。

## vue
### 对于mvvm的理解

MVVM 是 Model-View-ViewModel 的缩写。
Model代表数据模型，也可以在Model中定义数据修改和操作的业务逻辑。
View 代表UI 组件，它负责将数据模型转化成UI 展现出来。
ViewModel 监听模型数据的改变和控制视图行为、处理用户交互，简单理解就是一个同步View 和 Model的对象，连接Model和View。
在MVVM架构下，View 和 Model 之间并没有直接的联系，而是通过ViewModel进行交互，Model 和 ViewModel 之间的交互是双向的， 因此View 数据的变化会同步到Model中，而Model 数据的变化也会立即反应到View 上。
ViewModel 通过双向数据绑定把 View 层和 Model 层连接了起来，而View 和 Model 之间的同步工作完全是自动的，无需人为干涉，因此开发者只需关注业务逻辑，不需要手动操作DOM, 不需要关注数据状态的同步问题，复杂的数据状态维护完全由 MVVM 来统一管理。

### vue生命周期

beforeCreate（创建前） 在数据观测和初始化事件还未开始
created（创建后） 完成数据观测，属性和方法的运算，初始化事件，$el属性还没有显示出来
beforeMount（载入前） 在挂载开始之前被调用，相关的render函数首次被调用。实例已完成以下的配置：编译模板，把data里面的数据和模板生成html。注意此时还没有挂载html到页面上。
mounted（载入后） 在el 被新创建的 vm.$el 替换，并挂载到实例上去之后调用。实例已完成以下的配置：用上面编译好的html内容替换el属性指向的DOM对象。完成模板中的html渲染到html页面中。此过程中进行ajax交互。
beforeUpdate（更新前） 在数据更新之前调用，发生在虚拟DOM重新渲染和打补丁之前。可以在该钩子中进一步地更改状态，不会触发附加的重渲染过程。
updated（更新后） 在由于数据更改导致的虚拟DOM重新渲染和打补丁之后调用。调用时，组件DOM已经更新，所以可以执行依赖于DOM的操作。然而在大多数情况下，应该避免在此期间更改状态，因为这可能会导致更新无限循环。该钩子在服务器端渲染期间不被调用。
beforeDestroy（销毁前） 在实例销毁之前调用。实例仍然完全可用。
destroyed（销毁后） 在实例销毁之后调用。调用后，所有的事件监听器会被移除，所有的子实例也会被销毁。该钩子在服务器端渲染期间不被调用。

### Vue实现数据双向绑定的原理：Object.defineProperty（）

vue实现数据双向绑定主要是：采用数据劫持结合发布者-订阅者模式的方式，通过Object.defineProperty（）来劫持各个属性的setter，getter，在数据变动时发布消息给订阅者，触发相应监听回调。当把一个普通 Javascript 对象传给 Vue 实例来作为它的 data 选项时，Vue 将遍历它的属性，用 Object.defineProperty 将它们转为 getter/setter。用户看不到 getter/setter，但是在内部它们让 Vue 追踪依赖，在属性被访问和修改时通知变化。

vue的数据双向绑定 将MVVM作为数据绑定的入口，整合Observer，Compile和Watcher三者，通过Observer来监听自己的model的数据变化，通过Compile来解析编译模板指令（vue中是用来解析 {{}}），最终利用watcher搭起observer和Compile之间的通信桥梁，达到数据变化 —>视图更新；视图交互变化（input）—>数据model变更双向绑定效果。

### Vue组件间的参数传递

1.父组件与子组件传值
父组件传给子组件：子组件通过props方法接受数据;
子组件传给父组件：$emit方法传递参数
2.非父子组件间的数据传递，兄弟组件传值
eventBus，就是创建一个事件中心，相当于中转站，可以用它来传递事件和接收事件。项目比较小时，用这个比较合适。

使用vuex也可以

### Vue的路由实现：hash模式 和 history模式

hash模式：在浏览器中符号“#”，#以及#后面的字符称之为hash，用window.location.hash读取；
特点：hash虽然在URL中，但不被包括在HTTP请求中；用来指导浏览器动作，对服务端安全无用，hash不会重加载页面。

history模式：history采用HTML5的新特性；且提供了两个新方法：pushState（），replaceState（）可以对浏览器历史记录栈进行修改，以及popState事件的监听到状态变更。

### Vue与React的区别？

相同点：
React采用特殊的JSX语法，Vue.js在组件开发中也推崇编写.vue特殊文件格式，对文件内容都有一些约定，两者都需要编译后使用；中心思想相同：一切都是组件，组件实例之间可以嵌套；都提供合理的钩子函数，可以让开发者定制化地去处理需求；都不内置列数AJAX，Route等功能到核心包，而是以插件的方式加载；在组件开发中都支持mixins的特性。
不同点：
React采用的Virtual DOM会对渲染出来的结果做脏检查；Vue.js在模板中提供了指令，过滤器等，可以非常方便，快捷地操作Virtual DOM。

### vue路由的钩子函数

首页可以控制导航跳转，beforeEach，afterEach等，一般用于页面title的修改。一些需要登录才能调整页面的重定向功能。

beforeEach主要有3个参数to，from，next：

to：route即将进入的目标路由对象，

from：route当前导航正要离开的路由

next：function一定要调用该方法resolve这个钩子。执行效果依赖next方法的调用参数。可以控制网页的跳转。

### vuex是什么？怎么使用？哪种功能场景使用它？

只用来读取的状态集中放在store中； 改变状态的方式是提交mutations，这是个同步的事物； 异步逻辑应该封装在action中。
在main.js引入store，注入。新建了一个目录store，….. export 。
场景有：单页应用中，组件之间的状态、音乐播放、登录状态、加入购物车
![vuex](img/vue.jpg)

state
Vuex 使用单一状态树,即每个应用将仅仅包含一个store 实例，但单一状态树和模块化并不冲突。存放的数据状态，不可以直接修改里面的数据。
mutations
mutations定义的方法动态修改Vuex 的 store 中的状态或数据。
getters
类似vue的计算属性，主要用来过滤一些数据。
action 
actions可以理解为通过将mutations里面处里数据的方法变成可异步的处理数据的方法，简单的说就是异步操作数据。view 层通过 store.dispath 来分发 action。

## 微信小程序
### 微信小程序有几个文件

WXML （WeiXin Markup Language）是框架设计的一套标签语言，结合基础组件、事件系统，可以构建出页面的结构。内部主要是微信自己定义的一套组件。
WXSS (WeiXin Style Sheets)是一套样式语言，用于描述 WXML 的组件样式，
js 逻辑处理，网络请求
json 小程序设置，如页面注册，页面标题及tabBar。
app.json必须要有这个文件，如果没有这个文件，项目无法运行，因为微信框架把这个作为配置文件入口，整个小程序的全局配置。包括页面注册，网络设置，以及小程序的window背景色，配置导航条样式，配置默认标题。
app.js必须要有这个文件，没有也是会报错！但是这个文件创建一下就行 什么都不需要写以后我们可以在这个文件中监听并处理小程序的生命周期函数、声明全局变量。
app.wxss配置全局css

### 微信小程序组件封装

可以看我上篇文章微信小程序组件的封装：https://juejin.im/post/5afcee09518825670961

### 微信小程序怎样跟事件传值

给HTML元素添加data-*属性来传递我们需要的值，然后通过e.currentTarget.dataset或onload的param参数获取。但data-名称不能有大写字母和不可以存放对象

### 小程序的wxss和css有哪些不一样的地方？

wxss的图片引入需使用外链地址；

没有Body；样式可直接使用import导入

### 小程序关联微信公众号如何确定用户的唯一性？

使用wx.getUserInfo方法withCredentials为 true 时 可获取encryptedData，里面有 union_id。后端需要进行对称解密

### 微信小程序怎样获取用户信息

微信小程序获取用户信息需要用户授权，首先用户登陆微信小程序使用wx.login这个API，然后通过wx.getUserInfo这个API在拿到用户信息

### 微信小程序与vue区别

生命周期不一样，微信小程序生命周期比较简单

数据绑定也不同，微信小程序数据绑定需要使用{{}}，vue直接:就可以

显示与隐藏元素，vue中，使用v-if 和v-show控制元素的显示和隐藏，小程序中，使用wx-if和hidden控制元素的显示和隐藏

事件处理不同，小程序中，全用bindtap(bind+event)，或者catchtap(catch+event)绑定事件,vue：使用v-on:event绑定事件，或者使用@event绑定事件。

数据双向绑定也不也不一样在vue中,只需要再表单元素上加上v-model,然后再绑定data中对应的一个值，当表单元素内容发生变化时，data中对应的值也会相应改变，这是vue非常nice的一点。微信小程序必须获取到表单元素，改变的值，然后再把值赋给一个data中声明的变量。

取值也不一样，小程序中，通过this.data.reason取值，vue中，通过this.reason取值

父子组件间的通信也不同

