#### 1 . JavaScript

> 是一门用来与网页交互的脚本语言,包括`ECMAScript` 、`DOM` 、`BOM` 三个组成部分！！

> 最开始 JavaScript 问世时的主要用途是代替 `Perl` 等服务器语言处理输入验证

#### 2 . ECMAScript（提供核心功能）

(1)

> `ECMAScript：` 实现**ECMA-262**这个规范描述的所有方面的一门语言的称呼。

其并不局限于 Web 浏览器，`Web 浏览器`只是 `ECMAScript`实现可能存在的一种`宿主环境`。

- 宿主环境提供了 `ECMAScript` 的基准实现和与环境自身交互必须的扩展！！！
- 扩展（比如 DOM）使用 `ECMAScript` 核心类型和语法，提供特定于环境的额外功能。
- 其余宿主环境还有，例如`服务器端 JavaScript 平台Node.js`。

(2) **ECMA-262**定义规范了什么？

- 语法
- 类型
- 语句
- 关键字
- 保留字
- 操作符
- 全局对象

(3) 跟 `JavaScript` 的关系：

> javascript 实现了 ECMAScript !!!

#### 3 . DOM（提供与网页交互的方法和接口）

> `DOM` (Document Object Mudule) 文档对象模型(表示文档的树),是一个应用编程接口(API)!!!,用在 HTML 中使用扩展的 XML.

- DOM 将整个页面抽象为一组分层节点. DOM 通过创建表示文档的树,让开发者可以随心所欲地控制网页的内容和结构!!!

**注意:**

- 对于浏览器来说,DOM 就是通过 `ECMAScript` 实现的
- DOM 并非只能通过 JavaScript 访问!!!

#### 4 . BOM（提供与浏览器交互的方法和接口）

> `BOM`浏览器对象模型(表示文档的树),操作浏览器窗口!!

(1) BOM 主要范畴:

- 弹出新浏览器窗口
- navigator 对象,提供关于浏览器的详尽信息
- location 对象,提供浏览器加载页面的详尽信息
- screen 对象,提供关于用户屏幕分辨率的详尽信息
- 对 cookie 的支持
