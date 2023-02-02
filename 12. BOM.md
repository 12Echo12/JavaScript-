##### BOM

> `BOM` (Browser Object Model) 浏览器对象模型 。JavaScript的核心，提供了浏览器功能对象！！！

##### 一. Window 对象

> Window对象，表示为浏览器的实例

- 是 ES 中 `Global` 对象的代理

- 是浏览器的 JS 接口

**注意：**

因为 Window对象的属性在全局作用域中有效，所以很多浏览器的操作 API 和构造函数都以 Window对象的属性暴露出来，以供使用！！

**因为：**

Window对象被当作 Global 对象的代理，所以在全局作用域下用 var 声明的所有函数和变量都会成为 Window 对象的属性。

- 可以用 window 对象来查询某一变量是否声明！！

                 window.age
                 - 如果 age 声明了，返回存储的值
                 - 没有声明 age ，返回 undefined

###### Window对象的相关属性如下：

**<1> 窗口关系（几个窗口指针）**

- top ------ >  浏览器窗口本身（最上层/最外层窗口）

- parent  ------ > 当前窗口的父窗口

- self -------> 就是当前窗口 window

**<2> 窗口位置**

- moveTo()

- moveBy()

**<3> 窗口大小**

- innerWidth 、innerHeight 、outerWidth 、outerHeight

**<4> 视口位置**

**<5> 导航与打开新窗口**

- window.open()

              - 接收四个参数 要加载的 URL 、目标窗口 、特性字符串 、新打开的窗口在
              浏览器历史记录中是否替代当前窗口(布尔值)
              - 第二个参数如果是某个窗口名，那么会在该指定的窗口中打开新窗口，如果不是，就会
              重新在一个新窗口中打开！！！
              - 第四个参数可以用来设置新窗口的大小、位置....

**注意：**

由于弹窗泛滥，现在各个浏览器对弹窗都有了一定的限制，所以某些浏览器可能会对 window.open() 的使用报错！！！所以要用 try() 、catch() 块将 window.open()引用起来。防止出错！！！

**<6> 系统对话框**

- alter() 只能 ok 确认

- confirm() 有两个选项 OK or Cancel 
  
                - 有返回值
                      - true 表示点击了 OK
                      - false 表示点击了 Cancel

- prompt() 提示用户输入有两个选项 OK or Cancel

          - 有返回值
          - OK ，返回文本框中用户输入的内容
          - Cancel ，返回 null   

##### 二. location 对象

> `location对象` 包含了当前窗口中加载文档的信息，既是 Window 的属性 ，也是 document 的属性。(服务器、端口号、URL.....)

**<1> 查询字符串**

> `location.search` 返回了URL中从问号"?" 到结尾的所有查询字符串！！！但不太好对其进行使用，就可以使用 `URLSearchParams对象`

**URLSearchParams：**

> 其提供了一系列操作查询字符串的方法

- 需要创建该对象的实例，并且构造函数的参数为查询字符串，然后就可以在实例上调用一系列API [ get() 、 has() 、delete() ....]



**<2> 操作地址**     导航到新的地址

`共四种方法：`

- location.assign( v ) 

- location.href = v     最常见

- window.location = v

- **locatin.replace() **  会替代当前页面，即不能再回退到当前页面

**重载 reload()**  ---- 重新加载显示当前页面(如果不想从缓存中加载当前页面的话)！！！



##### 三. navigator 对象

> 其属性通常用于来确定浏览器的类型！！！

- 浏览器的版本、名字.....

- 可以用来进行浏览器的插件检测

##### 四. screen 对象

> 其属性储存客户端显示器的信息

- 屏幕像素高度....

##### 五. history 对象        导航

> 其属性和方法可以用来进行页面的前进和回退！！！

- history.go()

- history.back()




