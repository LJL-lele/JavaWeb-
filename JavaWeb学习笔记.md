
![JavaWeb学习笔记](https://i-blog.csdnimg.cn/direct/dbb9cba4efce4fd5a2ecd9937737d7a8.png)


---
大家好，这个是我个人的JavaWeb学习笔记，基于B站上面的各总视频教程学习的，结合视频类容深度思考整理后写下的笔记，类容比较详细，适合刚入门想学习JavaWeb的小伙伴，里面记录了全程的学习过程，各自资料的收集总结，代码实操，运行截图，遇到的问题，解决方案等，笔记将持续更新，直至javaweb学习完毕，欢迎大家一起来讨论交流，一起学习，希望可以帮助到大家。

**笔记使用方法：** 聚焦于知识点的总结和实现，知识点是分开的，笔记中是学一点就实操一下，便于理解记忆和快速入门。
**相关链接：** [1.黑马JavaWeb在线笔记](https://heuqqdmbyk.feishu.cn/wiki/QPxOw66KlikKhKk1TOlcqxHXnDd?from=from_copylink)
**学习视频：** [2.黑马JavaWeb学习视频](https://www.bilibili.com/video/BV1yGydYEE3H?t=7.5)
## 🌱学前配置
### VsCode插件安装
VS Code提供了非常丰富的插件功能，根据你的需要，安装对应的插件可以大大提高开发效率。

完成前端开发，常见插件介绍：
 Chinese (Simplified) Language Pack
适用于 VS Code 的中文（简体）语言包
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2403adf51a3c40aca581f8d0ef7cc35e.png)

安装完毕之后，点击右下角的 "Change Language and Restart" 按钮，重新启动服务。

 HTML CSS Support
在编写样式表的时候，自动补全功能大大缩减了编写时间。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/359252524cc143e6bf9a291a1736ef5f.png)


 JavaScript (ES6) code snippets
支持ES6语法提示
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9efb8bc6167d4c479cd4949500161ddc.png)

 
 Mithril Emmet
一个能大幅度提高前端开发效率的一个工具，用于补全代码
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/379f1b7ced754c1b95012ad79bea1638.png)


 Path Intellisense
路径提示插件
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/74e7ad27d2044971929f3aa8afd4347b.png)


 
Vue 3 Snippets
在 Vue 2 或者 Vue 3 开发中提供代码片段，语法高亮和格式化的 VS Code 插件，能极大提高你的开发效率。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/daa516fd5ef54b3a8abb99aba3ebd64a.png)


 Auto Close Tag
自动闭合HTML/XML标签
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c74932c5071e412f88c272d857f07839.png)

 

 Auto Rename Tag
自动完成另一侧标签的同步修改
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/36ce37491c124762aac366c67c187d0a.png)


open in browser
vscode不像IDE一样能够直接在浏览器中打开html，而该插件支持快捷键与鼠标右键快速在浏览器中打开html文件，支持自定义打开指定的浏览器，包括：Firefox，Chrome，Opera，IE以及Safari
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5441d9ab396b49ff87de54ab150b5231.png)


Live Server
一个具有实时加载功能的小型服务器，也就是说我们可以在项目中实时用live-server作为一个实时服务器实时查看开发的网页或项目效果。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/78a7cd7901d6409a80d6d2cc4ecbdaf6.png)


 Vue - Official
一个专门为 Vue 3 构建的语言支持插件。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/22d449ba28d240bda3b52e32577b3086.png)


File Utils
File Utils插件,可以方便快捷的来创建、复制、移动、重命名文件和目录。 
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/07868c4981e9442d8b05faff1975429a.png)



IntelliJ IDEA Keybindings
安装VSCode的插件 IntelliJ IDEA Keybindings 即可在VSCode中使用IDEA的快捷键。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8c9678864396492faf5b667accb0e3c8.png)



MarsCode AI
MarsCode 是字节跳动豆包旗下的智能编程助手，提供以智能代码补全为代表的核心能力，支持主流编程语言及 IDE，能在编码过程中提供单行或整个函数的建议，同时支持在用户编码过程中提供代码解释、单测生成、问题修复、技术问答等辅助功能，提升编码效率与质量。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8d908e12f5184db885e0a73817182055.png)

AI助手账号注册：[trea](https://www.marscode.cn/home?utm_source=mkt&utm_medium=cpaitcast&utm_campaign=hmcxy)


TONGYI Lingma
通义灵码，是一款基于通义大模型的智能编码辅助工具，提供行级/函数级实时续写、自然语言生成代码、单元测试生成、代码注释生成、代码解释、研发智能问答、异常报错排查等能力，并针对阿里云 SDK/API 的使用场景调优，为开发者带来高效、流畅的编码体验。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6e8b6668500140948a6afb2eb9aa0ed5.png)

AI助手账号注册：[通义灵码](https://account.aliyun.com/register/qr_register.htm?spm=5176.29741907.J_4VYgf18xNlTAyFFbOuOQe.d_register_1.e939154ab73d0j&oauth_callback=https://www.aliyun.com/)
## 🌱 前端学习路线
前端部分不是学习的重点，大家大概了解一下，可以看懂代码就行，不会的文AI就行啦。
### **第一阶段：基础三剑客**

1. **HTML**（结构层）

   * 网页的骨架，负责“放东西”。
   * 你会学：`div`、`p`、`img`、`a`、`table` 等常见标签。
   * 目标：能写一个简单的静态页面。

2. **CSS**（表现层）

   * 网页的样式，负责“让东西好看”。
   * 你会学：颜色、字体、布局（`flex`、`grid`）、响应式。
   * 目标：能把页面美化，像一个真正的网站。

3. **JavaScript**（行为层）

   * 网页的逻辑，负责“让东西动起来”。
   * 你会学：变量、函数、DOM 操作（比如点击按钮弹出提示）。
   * 目标：能写交互逻辑，比如一个计算器。

---

### **第二阶段：进阶**

1. **前端工程化**

   * 包括 Node.js、npm、模块化思想。
   * 学会用工具管理项目。

2. **框架**

   * Vue / React / Angular 任选一个（推荐 Vue 或 React）。
   * 让你快速做出复杂应用。

3. **后端基础（可选）**

   * 学一点点 Node.js + Express，做个简单 API。
   * 就能做到全栈开发啦。

---

### **第三阶段：项目实战**

* 做几个小项目，比如：

  * 个人简历网页
  * 记事本应用
  * 天气查询小工具

---

## 🔑 我建议的学习顺序

1. 先从 **HTML + CSS** 开始 👉 我可以带你写一个小网页。
2. 再学 **JavaScript 基础** 👉 会了变量、函数、DOM 就能做交互。
3. 再去 **React / Vue** 👉 打开大门。

---


# 🚀Day 1
---
## 知识要点 📌
### **HTML 是什么？**

HTML，全称 **HyperText Markup Language（超文本标记语言）**。
👉 它不是编程语言，而是一种 **标记语言**，用来描述网页的结构。

就好比：

* **人类写作文**要有标题、段落、图片；
* **网页**也需要“标题”“段落”“图片”，这些东西就是通过 **HTML 标签** 来写的。

---

### **HTML 的作用**

1. **搭建网页的骨架**
   就像房子的框架一样，HTML 是网页的结构。

2. **告诉浏览器内容是什么**

   * `<h1>` 表示标题
   * `<p>` 表示段落
   * `<img>` 表示图片

3. **配合 CSS 和 JavaScript 使用**

   * HTML：骨架
   * CSS：美化（加颜色、排版）
   * JS：让网页动起来

---

### **最简单的 HTML 例子**

```html
<!DOCTYPE html>
<html>
<head>
    <title>我的第一个网页</title>
</head>
<body>
    <h1>你好，世界！</h1>
    <p>这是我的第一个网页内容。</p>
    <img src="https://picsum.photos/200" alt="随机图片">
</body>
</html>
```

👉 打开方式：

1. 新建一个 `test.html` 文件
2. 把上面的代码复制进去
3. 双击打开，你就能在浏览器里看到网页啦 🎉

---





### 什么是 CSS？

**CSS** 全称 **Cascading Style Sheets**（层叠样式表），它的作用是 **给 HTML 页面加上样式**，比如颜色、字体、布局等。
👉 你可以理解为：**HTML 是骨架，CSS 是化妆和衣服**。

---

###  CSS 能做什么？

1. **改变文字样式**（颜色、大小、字体…）
2. **设置页面布局**（居中、分栏、网格布局…）
3. **美化背景**（背景颜色、背景图片…）
4. **增加动效**（过渡、动画、hover 效果…）

---

###  CSS 的写法

CSS 有 3 种使用方式：

1. **行内样式**（直接写在标签里）

```html
<p style="color: red; font-size: 20px;">这是一段红色文字</p>
```

2. **内部样式**（写在 `<style>` 标签中）

```html
<head>
  <style>
    p {
      color: blue;
      font-size: 18px;
    }
  </style>
</head>
<body>
  <p>这是蓝色的文字</p>
</body>
```

3. **外部样式**（单独写一个 `.css` 文件，然后引入）

```html
<!-- index.html -->
<link rel="stylesheet" href="style.css">
<p>这是带外部样式的文字</p>
```

```css
/* style.css */
p {
  color: green;
  font-size: 22px;
}
```

---

###  一个简单的例子

```html
<!DOCTYPE html>
<html>
<head>
  <title>CSS 示例</title>
  <style>
    body {
      background-color: lightyellow;
    }
    h1 {
      color: darkblue;
      text-align: center;
    }
    p {
      color: gray;
      font-size: 18px;
    }
  </style>
</head>
<body>
  <h1>这是标题</h1>
  <p>这是段落，带样式。</p>
</body>
</html>
```

打开网页，你会看到黄色背景、蓝色标题、灰色文字。✨

---

### 基本结构标签的讲解
你现在看到的就是一个最基本的 **HTML页面骨架**，我来逐行给你拆开解释，通俗易懂地理解它们的含义：

---

### 代码：

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

---

### 讲解：

1. **`<!DOCTYPE html>`**

   * 告诉浏览器：这是一个 **HTML5文档**。
   * 作用：让浏览器用最新的标准模式来渲染网页，而不是用旧的兼容模式。

---

2. **`<html lang="en"> ... </html>`**

   * 整个网页的根标签，所有内容都要写在 `<html>` 里面。
   * `lang="en"` 表示页面语言是 **英语**（如果写 `zh-CN`，就是中文）。

---

3. **`<head> ... </head>`**

   * 网页的“头部信息”，这里的内容不会直接显示在页面上。
   * 主要放：网页的配置、描述信息、CSS样式、JS脚本引入等。

   里面有几个常见的子标签：

   * **`<meta charset="UTF-8">`**

     * 指定网页的字符编码是 **UTF-8**。
     * 确保中文不会乱码。
   * **`<meta name="viewport" content="width=device-width, initial-scale=1.0">`**

     * 针对移动端优化的设置。
     * `width=device-width`：让网页宽度自适应设备屏幕宽度。
     * `initial-scale=1.0`：设置初始缩放比例为 1。
   * **`<title>Document</title>`**

     * 设置网页标题，会显示在浏览器标签页上。

---

4. **`<body> ... </body>`**

   * 网页的“身体部分”，真正展示给用户看的内容都放在这里。
   * 你平时看到的文字、图片、按钮、表格……都写在 `<body>` 里面。

---

📌 总结：

* `<!DOCTYPE html>` → 声明文档类型（HTML5）。
* `<html>` → 整个网页的根标签。
* `<head>` → 放配置信息（不直接显示）。
* `<body>` → 放页面内容（用户能看到的）。

---





### HTML 常见标签分类讲解

### 1. 文本标签

* `<h1> ~ <h6>`：标题标签，数字越小标题越大。相当于 Java 文档里的“章节标题”。
* `<p>`：段落标签，一般用来写正文。
* `<span>`：行内标签，用来给文字加样式，不会换行。

例子：

```html
<h1>我是大标题</h1>
<h3>我是小标题</h3>
<p>这里是一段文字。</p>
<span>这是高亮的文字</span>
```

---

### 2. 列表标签

* **无序列表**：`<ul><li>...</li></ul>`，前面有小圆点。
* **有序列表**：`<ol><li>...</li></ol>`，前面有数字。

例子：

```html
<ul>
  <li>苹果</li>
  <li>香蕉</li>
  <li>橘子</li>
</ul>

<ol>
  <li>第一步</li>
  <li>第二步</li>
</ol>
```

---

### 3. 链接和图片

* `<a href="url">文字</a>`：超链接。
* `<img src="url" alt="描述">`：图片。

例子：

```html
<a href="https://www.baidu.com">去百度</a>
<img src="cat.jpg" alt="一只可爱的猫">
```

---

### 4. 表格

* `<table>`：表格整体
* `<tr>`：一行（table row）
* `<td>`：单元格（table data）
* `<th>`：表头（加粗居中）

例子：

```html
<table border="1">
  <tr>
    <th>姓名</th>
    <th>年龄</th>
  </tr>
  <tr>
    <td>张三</td>
    <td>18</td>
  </tr>
</table>
```

---

### 5. 表单（重要，跟后端交互）

* `<form>`：表单容器
* `<input>`：输入框（text/password/checkbox/radio 等）
* `<button>` 或 `<input type="submit">`：提交按钮
* `<label>`：输入提示

例子：

```html
<form action="/login" method="post">
  <label>用户名：</label>
  <input type="text" name="username"><br>
  
  <label>密码：</label>
  <input type="password" name="password"><br>
  
  <button type="submit">登录</button>
</form>
```

（这里的 `action="/login"` 就会对应后端 Java 的接口，比如 Spring Boot 里的 `/login` API）

---

### 一个综合案例（前端 + 后端联动思维）

假设你有一个 **用户注册页面**，HTML 可以写成这样：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>用户注册</title>
</head>
<body>
  <h1>注册新用户</h1>
  <p>请填写以下信息：</p>

  <form action="/register" method="post">
    <label>用户名：</label>
    <input type="text" name="username"><br><br>

    <label>邮箱：</label>
    <input type="email" name="email"><br><br>

    <label>密码：</label>
    <input type="password" name="password"><br><br>

    <button type="submit">注册</button>
  </form>

  <h2>已有账号？</h2>
  <a href="/login">点此登录</a>
</body>
</html>
```

👉 运行逻辑：

* 用户在浏览器填写表单，点击“注册”。
* 浏览器会把数据（username/email/password）**POST 提交**到 `/register`。
* 你的 Java 后端（比如 Spring Boot Controller）就能接收到表单数据，处理后存入数据库。

---

### 总结（后端角度理解 HTML）

* HTML = **数据结构（页面结构）**
* CSS = **样式（相当于皮肤/美化）**
* JS = **行为（交互逻辑，像控制器）**


### 超链接标签
```java
<a href="https://news.sina.com.cn/o/2025-08-26/doc-infnismz9772640.shtml" target ="_blank"></a>
```

`<a>` 标签是超链接标签，而它的 `target` 属性就是**控制点击链接后页面在哪里打开**的参数。

---

### 常见的 `target` 取值及含义：

1. **`_self`** （默认值）

   * 在**当前窗口/标签页**中打开链接。
   * 示例：

     ```html
     <a href="https://www.baidu.com" target="_self">百度（当前页打开）</a>
     ```

2. **`_blank`**

   * 在**新窗口/新标签页**中打开链接。
   * 示例：

     ```html
     <a href="https://www.baidu.com" target="_blank">百度（新窗口打开）</a>
     ```

3. **`_parent`**

   * 在**父框架**中打开（主要用于 `<frame>` 或 `<iframe>` 场景）。
   * 示例：

     ```html
     <a href="page.html" target="_parent">在父框架中打开</a>
     ```

4. **`_top`**

   * 在**整个窗口**中打开，清除所有框架嵌套。
   * 示例：

     ```html
     <a href="page.html" target="_top">在整个窗口中打开</a>
     ```

5. **自定义名称（如 `myFrame`）**

   * 链接会在**指定的 iframe** 中打开。
   * 示例：

     ```html
     <iframe name="myFrame" width="400" height="200"></iframe>
     <a href="page.html" target="myFrame">在 iframe 中打开</a>
     ```

---

### 总结

* `target="_self"` → 当前页打开（默认）。
* `target="_blank"` → 新标签页打开，最常用。
* `target="_parent"`、`target="_top"` → 在框架结构里使用。
* `target="自定义名字"` → 指定的 iframe 里打开。

---


### CSS 样式主要有 **三种引入方式**：

---

### 1. **行内样式（Inline CSS）**

👉 直接在 HTML 标签的 `style` 属性里写样式。

### 写法：

```html
<p style="color: red; font-size: 18px;">这是红色的文字</p>
```

### 特点：

* 优点：方便，修改某个元素的样式时很快。
* 缺点：结构和样式混在一起，不利于维护，大项目很少用。

---

### 2. **内部样式（Internal CSS）**

👉 在 HTML 文件的 `<head>` 标签中，用 `<style>` 标签写样式。

### 写法：

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>内部样式示例</title>
  <style>
    p {
      color: blue;
      font-size: 20px;
    }
    .highlight {
      background-color: yellow;
    }
  </style>
</head>
<body>
  <p>这是蓝色的文字</p>
  <p class="highlight">这是高亮的文字</p>
</body>
</html>
```

### 特点：

* 优点：结构和样式分离一些，适合小型页面。
* 缺点：多个页面复用样式时麻烦。

---

### 3. **外部样式（External CSS）**

👉 把样式写到单独的 `.css` 文件里，在 HTML 中通过 `<link>` 引入。

### 写法：

**style.css**

```css
p {
  color: green;
  font-size: 22px;
}
```

**index.html**

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>外部样式示例</title>
  <!-- 外部样式文件引入 -->
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <p>这是绿色的文字</p>
</body>
</html>
```

### 特点：

* 优点：**前端开发最推荐**，样式和结构彻底分离，多个页面共享，方便维护。
* 缺点：必须额外加载一个 CSS 文件（但一般没问题）。

---

### 4. **优先级（重要概念）**

当三种方式冲突时，优先级是：

```
行内样式 > 内部样式 > 外部样式 > 浏览器默认样式
```

比如：

```html
<p style="color: red;">这段文字最终会是红色</p>
```

即使外部样式写了 `p { color: green; }`，也会被行内覆盖。

---
好的，我来用通俗的语言讲一下 **`<span>` 标签** 👇

---
### span标签
### 1. `span` 是什么？

* **`<span>` 标签是一个行内元素**，本身没有任何语义，也不会对内容的显示方式产生影响。
* 它的主要作用是：**在不改变内容结构的情况下，给文字或内容加样式**。

你可以把它理解成：
👉 “用来圈住一小段文字或内容，然后给它单独加点 CSS 样式”。

---

### 2. 使用场景

常见用法就是：

* 给一段文字设置 **颜色**、**字体**、**大小**。
* 给一小部分文字单独加 **背景色** 或 **下划线**。

---

### 3. 基本语法

```html
<p>我最喜欢的颜色是 <span style="color: red;">红色</span>。</p>
```

**效果：**
我最喜欢的颜色是 **红色**。

这里：

* 整段话是一个段落 `<p>`。
* 只有“红色”两个字被 `<span>` 包起来，并用 `style="color: red;"` 设置了颜色。

---

### 4. 为什么用 `span`？

如果你只想修改某几个字的样式，就不需要换标签（比如 `<p>` 会换行， `<div>` 会占一整行）。
👉 `span` 是 **行内元素**，不会影响整体排版，只针对被圈起来的内容加样式。

---

### 5. 示例练习

```html
<p>今天的天气 <span style="color: blue; font-weight: bold;">特别好</span>！</p>
<p>我在学习 <span style="background-color: yellow;">HTML 和 CSS</span>。</p>
```

**效果：**

* “特别好” → 蓝色加粗
* “HTML 和 CSS” → 黄色背景

---


### 🔨 实操演练（推荐练习）

1. 建一个 `index.html` 文件，写一段文字。
2. 先用 **行内样式** 改颜色。
3. 再用 **内部样式** 改字体大小。
4. 最后写一个 `style.css`，在里面加 `p { background-color: yellow; }`，看看效果。

---

### 我的代码例子
代码
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>人工智能新闻</title>
    <link rel="stylesheet" href="lele.css">
    <!-- 方式一：内部样式 -->
    <style>
        h1{
            color: red;
        }

    </style>
    <link rel="stylesheet" href="lele.css">
</head>
<body>
    <h1>方式一：内部样式</h1>
    <h1>人工智能新篇章</h1>

    <a href="https://news.sina.com.cn/o/2025-08-26/doc-infnismz9772640.shtml" target="_blank" rel="noopener">人工智能新闻</a>
    
    <span>
        时间：2025-08-26
        来源：新浪新闻
    </span>
    <!--方式二： 行内样式 -->
    <p style="color: aqua;">方式二：行内样式</p>

    <p style="color: aqua;">人工智能正在改变我们的世界，为我们带来了无限的可能性。</p>
    
    <!-- 方式三：外部样式 -->
    <h2>方式三：外部样式</h2>

    <h2>人工智能正在改变我们的世界，为我们带来了无限的可能性。</h2>
</body>

</html>
```
运行效果图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/165cdc8fa5f34a10a4f4d76aae42b9ea.png)
好的，我来详细讲一下 **CSS 的颜色表示方法**，通俗易懂，并结合你做笔记和实操的思路。

---

### CSS 颜色表示方法分类

### 1. **颜色名称（Color Name）**

直接用浏览器支持的标准颜色名称，比如：

```css
p {
  color: red;      /* 红色 */
  background-color: yellow; /* 黄色背景 */
}
```

常见颜色：

* red, green, blue, yellow, orange, pink, purple, black, white, gray

✅ 优点：简单易记
❌ 缺点：颜色数量有限，不能精确控制

---

### 2. **十六进制（Hex）**

用 `#RRGGBB` 表示颜色，每两位代表一个通道（红、绿、蓝）。

```css
p {
  color: #ff0000;   /* 红色 */
  color: #00ff00;   /* 绿色 */
  color: #0000ff;   /* 蓝色 */
}
```

* 前两位 RR → 红色值
* 中间 GG → 绿色值
* 后两位 BB → 蓝色值
* 范围：00 \~ FF（十六进制，0\~255）

✅ 优点：精确控制颜色
✅ 可以用 3 位缩写：`#f00` = `#ff0000`

---

### 3. **RGB 表示法**

使用 `rgb(R, G, B)`，每个通道取 0\~255。

```css
p {
  color: rgb(255, 0, 0);   /* 红色 */
  color: rgb(0, 255, 0);   /* 绿色 */
  color: rgb(0, 0, 255);   /* 蓝色 */
}
```

* `R` → 红色
* `G` → 绿色
* `B` → 蓝色

✅ 优点：直观易懂
✅ 可以加透明度（用 `rgba`）

```css
p {
  color: rgba(255, 0, 0, 0.5); /* 半透明红色 */
}
```

---

### 4. **HSL 表示法**

HSL = **色相（Hue）、饱和度（Saturation）、亮度（Lightness）**

```css
p {
  color: hsl(0, 100%, 50%);   /* 红色 */
  color: hsl(120, 100%, 50%); /* 绿色 */
  color: hsl(240, 100%, 50%); /* 蓝色 */
}
```

* **Hue** 色相：0\~360°，红色=0°，绿色=120°，蓝色=240°
* **Saturation** 饱和度：0\~100%
* **Lightness** 亮度：0\~100%

✅ 优点：调整颜色更自然，比如调亮度、饱和度

---

### 5. **透明关键字和关键字颜色**

* `transparent` → 完全透明
* `currentColor` → 使用当前文字颜色

```css
div {
  background-color: transparent;
  border-color: currentColor;
}
```

---

### 二、实操演练建议

1. 建一个 `index.html`，写一段文字。
2. 用 **颜色名称** 改字体颜色。
3. 用 **Hex** 改背景颜色。
4. 用 **RGB / RGBA** 改边框颜色或文字颜色。
5. 用 **HSL** 改另一段文字颜色。
6. 给每种颜色加上说明（写在 `<p>` 里），截图做笔记。

---

### CSS选择器
好嘞！CSS 选择器是前端最核心的知识之一，它决定了 **你要给哪些 HTML 元素添加样式**。我给你用 Java 后端思维类比讲解，通俗易懂，并按类别整理。

---

### CSS 选择器概念

* CSS 选择器就像 **SQL 的条件语句或者 Java 的对象引用**
* 它告诉浏览器：“我想给页面里哪些元素加样式”

例子：

```css
p {
  color: red;
}
```

* `p` → 选择器
* `{ color: red; }` → 样式
  意思是：把所有 `<p>` 标签文字变红。

---

### CSS 选择器分类讲解

### 1. **基础选择器**

| 选择器    | 说明                    | 示例                                   |
| ------ | --------------------- | ------------------------------------ |
| `*`    | 通配符，选择所有元素            | `* { margin: 0; }`                   |
| `元素`   | 标签选择器，选择所有该标签元素       | `p { color: red; }`                  |
| `.类名`  | 类选择器，选择所有拥有 class 的元素 | `.highlight { background: yellow; }` |
| `#id名` | ID 选择器，选择拥有指定 id 的元素  | `#title { font-size: 24px; }`        |

---

### 2. **组合选择器**

* **后代选择器**（空格）：

```css
div p {
  color: blue;
}
```

> 选择 div 内的所有 p 标签

* **子元素选择器**（`>`）：

```css
div > p {
  color: green;
}
```

> 选择 div 的直接子元素 p

* **并集选择器**（`,`）：

```css
h1, h2, h3 {
  font-weight: bold;
}
```

> 同时选择 h1、h2、h3 标签

---

### 3. **伪类选择器**

* 用来选择元素的**特定状态**

```css
a:hover {
  color: red; /* 鼠标悬停时变红 */
}
p:first-child {
  font-weight: bold; /* 父元素的第一个 p 标签加粗 */
}
```

常用伪类：

* `:hover` → 鼠标悬停
* `:first-child` → 第一个子元素
* `:last-child` → 最后一个子元素
* `:nth-child(n)` → 第 n 个子元素

---

### 4. **伪元素选择器**

* 选择元素的一部分，而不是整个元素

```css
p::first-letter {
  font-size: 30px; /* 段落首字母放大 */
}
p::before {
  content: "★ "; /* 在段落前添加内容 */
}
```

---

### 5. **属性选择器**

* 根据元素属性来选择

```css
input[type="text"] {
  border: 1px solid gray;
}
img[alt] {
  border: 1px solid red; /* 所有有 alt 属性的图片 */
}
```

---

### 6. **层级与优先级**

CSS 优先级计算方式（从高到低）：

1. 行内样式（`style=""`）
2. ID 选择器（`#id`）
3. 类、伪类、属性选择器（`.class`、`:hover`）
4. 标签选择器（`p`, `div`）
5. 通配符 `*`

> 后端类比：就像 Java 对象里字段覆盖顺序，最具体的规则优先级高。

---

### 实操演练建议

1. 写一个简单 HTML 页面：

```html
<div id="box" class="highlight">
  <p>段落 1</p>
  <p>段落 2</p>
  <a href="#">这是链接</a>
</div>
```

2. 用不同选择器设置样式：

```css
/* 基础选择器 */
p { color: blue; }

/* 类选择器 */
.highlight { background: yellow; }

/* ID 选择器 */
#box { border: 2px solid red; }

/* 后代选择器 */
div p { font-size: 18px; }

/* 伪类 */
a:hover { color: green; }

/* 伪元素 */
p::first-letter { font-size: 24px; color: red; }

/* 属性选择器 */
a[href] { text-decoration: underline; }
```

3. 打开浏览器查看效果。

---
好嘞，我来用通俗的方式给你讲解一下 **`<video>` 标签** 👇

---

### video标签
### 1.`<video>` 标签的作用

HTML5 提供的标签，用来在网页中 **嵌入视频**（比如 MP4、WebM、Ogg 格式的文件）。
以前需要用 Flash 插件，现在直接用 `<video>` 就能播放。

---

### 2. 基本语法

```html
<video src="movie.mp4" controls></video>
```

* `src` ：视频文件的路径
* `controls` ：显示控制条（播放、暂停、音量、全屏）

如果没有 `controls`，视频会加载但是用户没法操作。

---

### 3. 常见属性

| 属性                 | 作用                       |
| ------------------ | ------------------------ |
| `src`              | 指定视频文件路径                 |
| `controls`         | 显示控制条                    |
| `autoplay`         | 自动播放（⚠️很多浏览器需要静音才允许自动播放） |
| `loop`             | 循环播放                     |
| `muted`            | 静音                       |
| `poster="xxx.jpg"` | 视频未播放时显示的封面图片            |
| `width` / `height` | 设置视频的宽高                  |

---

### 4. 多格式兼容写法

不同浏览器支持的视频格式不一样，所以一般写多个 `<source>`：

```html
<video controls width="400">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  <source src="movie.ogg" type="video/ogg">
  您的浏览器不支持 video 标签。
</video>
```

浏览器会从上往下选择它能识别的格式。

---

### 5. 一个完整例子

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>视频演示</title>
</head>
<body>
  <h2>HTML5 视频演示</h2>
  
  <video controls width="500" poster="cover.jpg">
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.webm" type="video/webm">
    您的浏览器不支持 video 标签。
  </video>

</body>
</html>
```

---

### 6. 小总结

* `<video>` 用来播放视频
* 最常见属性：`controls autoplay loop muted poster`
* 为了兼容性，最好写多个 `<source>`
* 不支持视频的浏览器会显示标签内的文字（备用提示）

---

好的，我来给你详细讲解一下 **`<img>` 标签**，这是 HTML 中最常用的标签之一，用于在网页中插入图片。

---
### < img >标签
### 1. 基本语法

```html
<img src="图片路径" alt="替代文字">
```

特点：

* **`<img>` 是自闭合标签**（没有 `</img>`）。
* 必须指定 `src` 属性来加载图片。

---

### 2. 常用属性

#### (1) **src（source，图片路径）**

指定图片的地址，可以是：

* **相对路径**：`src="images/photo.jpg"`
* **绝对路径**：`src="https://example.com/photo.jpg"`

---

#### (2) **alt（alternative text，替代文本）**

当图片加载失败时显示的文字，同时也用于无障碍（盲人读屏器会读取）。

```html
<img src="logo.png" alt="网站LOGO">
```

---

#### (3) **width / height（宽度和高度）**

控制图片显示的大小：

```html
<img src="cat.jpg" width="200" height="150">
```

注意：如果只写一个（比如 `width`），浏览器会按比例缩放另一边。

---

#### (4) **title**

鼠标悬停时显示的提示文字：

```html
<img src="dog.jpg" alt="小狗" title="这是一只小狗">
```

---

#### (5) **loading（懒加载）**

* `loading="lazy"` 表示只有当用户快要滚动到图片时才加载，提升性能。
* `loading="eager"` 表示立即加载（默认）。

```html
<img src="big-image.jpg" alt="大图" loading="lazy">
```

---

#### (6) **其他常见属性**

* `style`：可以写 CSS 样式（不推荐，最好写在 CSS 文件里）。
* `class` / `id`：用于 CSS 或 JavaScript 操作。

---

### 3. 图片格式

常见的图片文件类型：

* **JPEG (.jpg / .jpeg)**：适合照片，有损压缩，文件小。
* **PNG (.png)**：支持透明，适合图标、LOGO。
* **GIF (.gif)**：支持简单动画。
* **SVG (.svg)**：矢量图，放大不失真。
* **WebP (.webp)**：谷歌推出的格式，压缩率高，支持透明。

---

### 4. 使用示例

### 基本用法

```html
<img src="cat.jpg" alt="可爱的小猫">
```

### 设置大小

```html
<img src="cat.jpg" alt="小猫" width="300">
```

### 带提示信息

```html
<img src="dog.jpg" alt="小狗" title="萌萌的小狗">
```

### 懒加载

```html
<img src="big-photo.jpg" alt="风景图" loading="lazy">
```

---

### 5. 注意事项

1. `alt` 很重要，对 SEO 和无障碍体验都很有用。
2. 不要用大图直接缩小显示（会浪费带宽），应该上传合适大小的图片。
3. 想让图片响应式（在不同屏幕自适应），常用 CSS：

   ```css
   img {
     max-width: 100%;
     height: auto;
   }
   ```

---

好的，我们把 **`<br>`、`<strong>`、`<b>`** 标签逐个讲解一下，带你快速理解它们的区别和用法：

---

###  `<br>` 换行标签

* **作用**：在文本中插入一个**换行**。
* **特点**：

  * 它是**空标签**（没有结束标签）。
  * 用于需要在文字中**强制换行**的时候。
  * 不会产生额外的段落间距（不同于 `<p>` 标签）。

✅ 示例：

```html
<p>第一行<br>第二行<br>第三行</p>
```

📌 显示效果：
第一行
第二行
第三行

---

### `<strong>` 标签

* **作用**：表示一段文字的重要性、强调。
* **特点**：

  * 语义化标签（强调“语义”而不仅仅是样式）。
  * 默认样式是 **加粗**（和 `<b>` 看起来一样），但在屏幕阅读器（盲人用的阅读设备）里会读作“重点”。

✅ 示例：

```html
<p>今天的任务<strong>必须完成</strong>！</p>
```

📌 显示效果：
今天的任务 **必须完成**！

（这里“必须完成”不仅加粗，还带有“很重要”的语义信息）

---

### `<b>` 标签

* **作用**：让文字加粗。
* **特点**：

  * **非语义化标签**，只是单纯改变样式。
  * 不强调重要性，只是让文字看起来醒目。

✅ 示例：

```html
<p>这本书的名字是 <b>HTML入门</b>。</p>
```

📌 显示效果：
这本书的名字是 **HTML入门**。

---

### 📌 总结区别

| 标签         | 主要作用      | 是否语义化  | 默认效果 |
| ---------- | --------- | ------ | ---- |
| `<br>`     | 强制换行      | 无      | 换行   |
| `<strong>` | 强调内容，表示重要 | ✅ 语义化  | 加粗   |
| `<b>`      | 文字加粗（仅样式） | ❌ 非语义化 | 加粗   |

👉 所以：

* 想要**换行** → 用 `<br>`。
* 想要**加粗并表达重要性** → 用 `<strong>`。
* 想要**只是加粗外观** → 用 `<b>`。

---


好问题 👍，你提到的 `<u> <ins> <i> <em> <s> <del>` 这些 HTML 标签，看似都是“样式标签”，但实际上有 **表现形式**（外观效果）和 **语义意义**（被浏览器、搜索引擎、读屏软件理解的含义）两个层面。我们来逐个讲解：

---

### 下划线相关

### `<u>`

* **表现**：给文本加下划线。
* **语义**：⚠️ 没有特别的语义，纯粹是样式标签。
* **问题**：容易和超链接 `<a>` 混淆，所以现代开发中少用它，推荐用 CSS `text-decoration: underline;`。

```html
<p>这是<u>下划线</u>效果。</p>
```

### `<ins>`

* **表现**：默认也是下划线。
* **语义**：表示“插入的文本”（inserted text）。
* **应用场景**：比如在文章修订中，标注新增的内容。
* **推荐使用**：因为它有实际语义（区别于纯样式的 `<u>`）。

```html
<p>这是<ins>新增</ins>的文字。</p>
```

---

### 倾斜相关

### `<i>`

* **表现**：让文字变斜体。
* **语义**：本身没有“强调”语义，只是单纯地表现样式。
* **常见用法**：用来表示外来词、专业名词、图标字体等。
* **不推荐用于强调**。

```html
<p>我会说<i>English</i>。</p>
```

### `<em>`

* **表现**：默认也是斜体。
* **语义**：有“强调”作用（emphasis）。
* **层级语义**：嵌套 `<em>` 可以表示更强的强调。
* **推荐使用**：因为不仅视觉上强调，读屏软件也会加重语气。

```html
<p>这是<em>重点</em>。</p>
<p>这是<em><em>非常重要</em></em>的部分。</p>
```

---

### 删除线相关

### `<s>`

* **表现**：给文字加删除线。
* **语义**：表示“不再准确、不再相关”的内容。
* **示例**：表示过期价格、废弃信息。

```html
<p>原价：<s>￥199</s>，现价：￥99。</p>
```

### `<del>`

* **表现**：默认也是删除线。
* **语义**：表示“被删除的文本”（deleted text）。
* **应用场景**：文档修订时标记被删除的部分。
* **推荐使用**：因为它比 `<s>` 更语义化。

```html
<p>修订：<del>错误的内容</del> → 正确的内容</p>
```

---

### 📝 总结对比表

| 标签      | 样式  | 语义      | 推荐情况             |
| ------- | --- | ------- | ---------------- |
| `<u>`   | 下划线 | 无语义     | ❌ 不推荐，改用 CSS     |
| `<ins>` | 下划线 | 插入内容    | ✅ 推荐             |
| `<i>`   | 斜体  | 无语义     | ⚠️ 少用，适合外来语/专有名词 |
| `<em>`  | 斜体  | 强调      | ✅ 推荐             |
| `<s>`   | 删除线 | 过期、不再相关 | ⚠️ 场景有限          |
| `<del>` | 删除线 | 被删除的内容  | ✅ 推荐             |

---

👉 所以一句话总结：

* **强调**用 `<em>`（不要用 `<i>`）。
* **新增内容**用 `<ins>`（不要用 `<u>`）。
* **删除内容**用 `<del>`（比 `<s>` 更有语义）。

### 几个标签

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a0fe8734be5a42638e3fd01fcef0f98b.png)

### 盒子模型
 **CSS 盒子模型（Box Model）**。这是前端布局的核心概念之一。你可以把网页里的每一个元素（比如一个按钮、一个段落、一个 div）都想象成一个 **盒子**。

---

### 📦 盒子模型的四层结构

一个盒子由 **从里到外** 四个部分组成：

1. **content（内容区域）**

   * 存放文字、图片等实际内容的地方。
   * 可以通过 `width` 和 `height` 来控制大小。

2. **padding（内边距）**

   * 内容和边框之间的空隙。
   * 设置 `padding` 会让内容区域“往里缩”，但是会撑大整个盒子。

3. **border（边框）**

   * 围绕在 `padding` 外面的一层边框。
   * 可以设置粗细（`border-width`）、样式（`solid`、`dashed`）、颜色。

4. **margin（外边距）**

   * 盒子与盒子之间的距离。
   * 透明的，不会有背景色。

---

### 🔎 直观结构图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/374c8b01e39d45c9af0444102e4dea43.png)




### 📐 盒子总宽度 / 高度计算公式

* **标准盒子模型（content-box，默认值）**

  ```
  总宽度 = content 宽度 + padding + border + margin
  总高度 = content 高度 + padding + border + margin
  ```

* **IE盒子模型（border-box，需要手动设置：box-sizing: border-box）**

  * 在这种模式下，`width` 和 `height` 包含了 `content + padding + border`。
  * 好处：设置一个固定大小时，内部 padding 和 border 不会把盒子撑大。

---
### 边距参数的使用方法
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/92211c6d1dda46339a3aca8b432fdea7.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/bf87e7b491f74bc19d75910fe94e6fd7.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2be4393ef02c4787b8b1b5c385375da4.png)

### 🌰 举个例子

```html
<div class="box">Hello World</div>
```

```css
.box {
  width: 200px;           /* 内容宽度 */
  height: 100px;          /* 内容高度 */
  padding: 10px;          /* 内边距 */
  border: 5px solid red;  /* 边框 */
  margin: 20px;           /* 外边距 */
}
```

* 在 **标准盒子模型** 下：
  总宽度 = 200 + (10×2) + (5×2) + (20×2) = 270px
  总高度 = 100 + (10×2) + (5×2) + (20×2) = 170px

* 如果加上 `box-sizing: border-box;`：
  总宽度 = 200 + margin(20×2) = 240px
  总高度 = 100 + margin(20×2) = 140px

---
### div标签与span标签的区别


---

### 1. **基本概念**

* **`<div>`**：division（区块），是一个 **块级元素**。
* **`<span>`**：跨度（内联容器），是一个 **行内元素**。

---

### 2. **显示特点**

#### 📦 `<div>`（块级元素）

* 独占一行，默认会 **从上到下排列**。
* 宽度默认撑满父容器（可以设置宽高）。
* 常用于 **大块内容的布局**。
* 类比：像一块砖头，一块接一块往下摆。

```html
<div style="background: lightblue;">这是一个 div</div>
<div style="background: lightgreen;">这是另一个 div</div>
```

效果：每个 div 各占一行。

---

#### 📝 `<span>`（行内元素）

* 不会独占一行，**跟其他文字或标签在同一行显示**。
* 默认宽高由内容决定（不能直接设置宽高，除非转成块级/行内块）。
* 常用于 **标记或修饰文字**。
* 类比：像文字里的一个小标记，用荧光笔划出的几字。

```html
<p>我喜欢 <span style="color:red;">红色</span> 的文字。</p>
```

效果：整句话在一行，只有“红色”字变红。

---

### 3. **使用场景**

* **`div`**：布局、分块、页面结构。
  👉 例：头部（header）、内容区（content）、侧边栏（sidebar）、底部（footer）。
* **`span`**：修饰局部文本或小范围内容。
  👉 例：给某几个字加颜色、加粗。

---

### 4. **总结口诀**

* **div = 大盒子，块级布局用它。**
* **span = 小标记，修饰文字用它。**

---
### Flex弹性布局
好的，我来用通俗的方式给你讲解 **Flex 弹性布局**，并结合案例演示。

---

### 1. 什么是 Flex 布局？

Flex 全称是 **Flexible Box（弹性盒子布局）**，是 CSS3 新增的一种布局方式。
它主要解决的是：**如何在容器里灵活、方便地排列子元素**，尤其是应对不同屏幕大小时的自适应。

一句话总结：
👉 你把一个容器设为 `display: flex`，里面的子元素就会按“弹性规则”来排列。

---

### 2. Flex 的核心思想

* **容器（父元素）**：定义为 `display: flex`，相当于一个“弹性盒子”。
* **项目（子元素）**：容器里的每个元素就是一个“弹性子元素”，会按规则排列。

Flex 有两条轴：

* **主轴**（main axis）：子元素主要排列的方向（默认是横向从左到右）。
* **交叉轴**（cross axis）：垂直于主轴的方向（默认是纵向从上到下）。

---

### 3. 常用属性

### 1）父容器属性（常用）

* `display: flex;` → 开启弹性布局
* `flex-direction` → 设置主轴方向

  * `row`（默认，横向排列）
  * `column`（纵向排列）
* `justify-content` → 沿主轴对齐方式

  * `flex-start`（靠左/靠上）
  * `flex-end`（靠右/靠下）
  * `center`（居中）
  * `space-between`（两端对齐，元素均分间距）
  * `space-around`（每个元素两边都有间距）
* `align-items` → 沿交叉轴对齐方式

  * `flex-start`（顶部对齐）
  * `flex-end`（底部对齐）
  * `center`（垂直居中）
  * `stretch`（拉伸填满容器高度）

### 2）子元素属性（常用）

* `flex: 1` → 自动分配空间（相当于“平均分”）
* `order` → 改变排列顺序
* `align-self` → 单独设置某个子元素的交叉轴对齐方式

---

### 4. 使用案例

### 🌰 示例：制作一个水平居中、垂直居中的三栏布局

```html
<!DOCTYPE html>
<html lang="zh">
<head>
  <meta charset="UTF-8">
  <title>Flex布局示例</title>
  <style>
    .container {
      display: flex;                /* 开启Flex布局 */
      flex-direction: row;          /* 横向排列 */
      justify-content: center;      /* 主轴居中 */
      align-items: center;          /* 交叉轴居中 */
      height: 100vh;                /* 全屏高度 */
      background-color: #f0f0f0;
    }

    .box {
      width: 100px;
      height: 100px;
      margin: 10px;
      background-color: lightblue;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 20px;
      border-radius: 10px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="box">1</div>
    <div class="box">2</div>
    <div class="box">3</div>
  </div>
</body>
</html>
```

👉 页面效果：

* 三个方块在屏幕中央水平并排显示。
* 无论屏幕大小变化，都会保持居中。

---

### 5. 小总结

* **Flex 是专门用来做自适应、响应式布局的利器**。
* 关键点：`flex-direction`（主轴方向）、`justify-content`（主轴对齐）、`align-items`（交叉轴对齐）。
* 子元素还能用 `flex` 属性来自动伸缩。

---
好的，我来用**通俗易懂的方式**给你讲解一下 **HTML 表单标签（form 标签）**。

---
### 表单标签
### 1. 什么是表单标签？

表单（`<form>`）是用来**收集用户输入数据**的，比如：

* 登录页面（用户名 + 密码）
* 注册页面（邮箱 + 手机号 + 密码）
* 搜索框（输入关键字）
* 调查问卷

👉 可以理解为：**表单就是前端和后端之间的“桥梁”**，它把用户输入的内容发送到服务器。

---

### 2. 表单的基本语法

```html
<form action="提交地址" method="提交方式">
    <!-- 这里放表单元素 -->
</form>
```

* `action`：数据提交到哪里（一般是后台接口地址，比如 `/login`）。
* `method`：提交方式，常用有两个：

  * `GET`：数据会显示在 URL 上（适合搜索框）。
  * `POST`：数据放在请求体中，不会出现在 URL（适合登录、注册）。

---
好问题 👍。我们具体讲解一下 **`<form>` 标签的 `method` 属性**，它主要有两个常见取值：

---

#### 1. `GET` 方法

##### 特点：

* **数据拼接在 URL 后面**，以 `?` 开始，用 `&` 分隔参数。
  例如：

  ```
  https://example.com/search?name=Tom&age=18
  ```
* **数据长度有限制**（不同浏览器和服务器有不同限制，通常在 2KB～8KB 左右）。
* **数据明文显示**在地址栏，不安全。
* **可以被收藏、分享、保存历史记录**。

##### 适用场景：

* **查询类表单**：如搜索框、过滤条件、分页查询。
* 当你需要 **把表单数据保存到书签**，或者用户 **可能会分享链接** 的情况。

---

#### 2. `POST` 方法

##### 特点：

* **数据放在 HTTP 请求体里**，不会显示在 URL 上。
* **理论上没有大小限制**（取决于服务器配置，通常比 GET 大很多）。
* **数据相对安全**（虽然依然需要 HTTPS 才能真正加密）。
* **不能直接被收藏或分享**。

##### 适用场景：

* **需要提交敏感信息**：如密码、个人资料。
* **数据量较大**：如文章提交、文件上传。
* **会修改服务器数据的操作**：如注册、登录、发帖、购物车提交。

---

#### 3. 代码示例

##### 使用 `GET`

```html
<form action="/search" method="get">
  <label>关键字：<input type="text" name="keyword"></label>
  <button type="submit">搜索</button>
</form>
```

用户输入 `apple`，提交后浏览器跳转到：

```
/search?keyword=apple
```

---

##### 使用 `POST`

```html
<form action="/login" method="post">
  <label>用户名：<input type="text" name="username"></label>
  <label>密码：<input type="password" name="password"></label>
  <button type="submit">登录</button>
</form>
```

提交后数据在 **请求体**，不会显示在 URL 上。

---

✅ 总结一句话：

* **GET** → 查询、获取、书签/分享。
* **POST** → 提交、修改、敏感或大数据。

---



### 3. 表单常见的控件（表单元素）

表单中常用的标签有：

### （1）输入框 `<input>`

```html
<input type="text" name="username" placeholder="请输入用户名">
<input type="password" name="password" placeholder="请输入密码">
<input type="email" name="email" placeholder="请输入邮箱">
<input type="number" name="age" placeholder="请输入年龄">
<input type="checkbox" name="hobby" value="read"> 阅读
<input type="radio" name="gender" value="male"> 男
<input type="radio" name="gender" value="female"> 女
```

👉 `type` 决定输入框的样子
👉 `name` 是提交到后台的字段名（必须写）

---

### （2）下拉框 `<select>`

```html
<select name="city">
  <option value="bj">北京</option>
  <option value="sh">上海</option>
  <option value="gz">广州</option>
</select>
```

---

### （3）多行输入框 `<textarea>`

```html
<textarea name="comment" rows="5" cols="30"></textarea>
```

适合写留言、评论等。

---

### （4）按钮

```html
<input type="submit" value="提交">
<input type="reset" value="重置">
<button type="button">普通按钮</button>
```

* `submit`：提交表单
* `reset`：清空表单
* `button`：普通按钮（需要自己写功能）

---

### 4. 表单完整案例

👉 做一个登录表单

```html
<form action="/login" method="post">
  <label>用户名：</label>
  <input type="text" name="username" placeholder="请输入用户名"><br><br>

  <label>密码：</label>
  <input type="password" name="password" placeholder="请输入密码"><br><br>

  <label>性别：</label>
  <input type="radio" name="gender" value="male"> 男
  <input type="radio" name="gender" value="female"> 女<br><br>

  <label>城市：</label>
  <select name="city">
    <option value="bj">北京</option>
    <option value="sh">上海</option>
    <option value="gz">广州</option>
  </select><br><br>

  <label>个人简介：</label><br>
  <textarea name="intro" rows="4" cols="40"></textarea><br><br>

  <input type="submit" value="登录">
  <input type="reset" value="重置">
</form>
```

---

### 5. 总结

* `form` 是表单的容器
* `action` 指定提交地址，`method` 指定提交方式
* 表单里常见的控件有：`input`、`select`、`textarea`、`button`
* 提交时，`name` 对应后台接收的字段名

---
### 表单标签——表单项
好的 👍 我来给你系统归纳一下 **表单标签的表单项**，并整理成一个清晰的表格，方便你快速理解和对比。

---

### 表单项总结表格

| 表单项标签                     | 功能              | 常见属性                                     | 应用场景        |           |                 |
| ------------------------- | --------------- | ---------------------------------------- | ----------- | --------- | --------------- |
| `<input type="text">`     | 单行文本输入框         | `name`、`value`、`placeholder`、`maxlength` | 用户名、搜索框     |           |                 |
| `<input type="password">` | 密码输入框（内容不可见）    | `name`、`maxlength`、`placeholder`         | 登录密码        |           |                 |
| `<input type="radio">`    | 单选按钮（只能选一个）     | `name`（同组选项相同）、`value`、`checked`         | 性别选择、支付方式   |           |                 |
| `<input type="checkbox">` | 多选框（可选多个）       | `name`、`value`、`checked`                 | 兴趣爱好、权限选择   |           |                 |
| `<input type="submit">`   | 提交按钮            | `value`                                  | 提交表单到服务器    |           |                 |
| `<input type="reset">`    | 重置按钮            | `value`                                  | 清空表单内容      |           |                 |
| `<input type="button">`   | 普通按钮（无默认功能）     | `value`、`onclick`                        | JS交互按钮      |           |                 |
| `<input type="file">`     | 文件上传选择框         | `accept`（限制文件类型）、`multiple`（多选）          | 上传头像、文档     |           |                 |
| `<input type="hidden">`   | 隐藏字段（用户不可见）     | `name`、`value`                           | 传递后台参数（如ID） |           |                 |
| `<textarea>`              | 多行文本输入          | `rows`、`cols`、`placeholder`              | 留言、评论、文章输入  |           |                 |
| `<select>` + `<option>`   | 下拉选择框           | `selected`、`multiple`                    | 城市选择、分类选择   |           |                 |
| `<button>`                | 自定义按钮           | \`type="submit                           | reset       | button"\` | 代替 input 按钮，更灵活 |
| `<label>`                 | 标签文本，点击可聚焦对应表单项 | `for`（绑定id）                              | 提升可用性和无障碍体验 |           |                 |
| `<fieldset>`              | 表单分组            | -                                        | 把相关表单项分组显示  |           |                 |
| `<legend>`                | 分组标题            | -                                        | 表单分组的说明文字   |           |                 |

---

✅ **记忆技巧**

* **input万能选手**：大部分输入（文字、密码、单选、多选、按钮、文件等）都用 `<input>` 实现。
* **专用标签**：长文本用 `<textarea>`，下拉选项用 `<select>`，分组说明用 `<fieldset>` + `<legend>`。
* **辅助标签**：`<label>` 提升交互体验。

---


### 📌 完整的表单示例代码（HTML）

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>注册表单示例</title>
</head>
<body>
  <h2>用户注册表单</h2>
  <!-- form 表单开始 -->
  <form action="/submit_form" method="post">
    
    <!-- 文本输入框 -->
    <label for="username">用户名：</label>
    <input type="text" id="username" name="username" placeholder="请输入用户名" required>
    <br><br>

    <!-- 密码框 -->
    <label for="password">密码：</label>
    <input type="password" id="password" name="password" placeholder="请输入密码" required>
    <br><br>

    <!-- 单选按钮 -->
    性别：
    <input type="radio" id="male" name="gender" value="男" checked>
    <label for="male">男</label>
    <input type="radio" id="female" name="gender" value="女">
    <label for="female">女</label>
    <br><br>

    <!-- 复选框 -->
    爱好：
    <input type="checkbox" id="reading" name="hobby" value="阅读">
    <label for="reading">阅读</label>
    <input type="checkbox" id="sports" name="hobby" value="运动">
    <label for="sports">运动</label>
    <input type="checkbox" id="music" name="hobby" value="音乐">
    <label for="music">音乐</label>
    <br><br>

    <!-- 下拉列表 -->
    <label for="city">所在城市：</label>
    <select id="city" name="city">
      <option value="bj">北京</option>
      <option value="sh">上海</option>
      <option value="gz">广州</option>
      <option value="sz">深圳</option>
    </select>
    <br><br>

    <!-- 多行文本框 -->
    <label for="intro">个人简介：</label><br>
    <textarea id="intro" name="intro" rows="4" cols="40" placeholder="写点你的自我介绍..."></textarea>
    <br><br>

    <!-- 文件上传 -->
    <label for="avatar">上传头像：</label>
    <input type="file" id="avatar" name="avatar">
    <br><br>

    <!-- 提交和重置按钮 -->
    <input type="submit" value="提交注册">
    <input type="reset" value="重置表单">
    
  </form>
  <!-- form 表单结束 -->
</body>
</html>
```

---
运行效果图
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8f09e4796b5648ca93e1676fc489927d.png)

### 📌 表单包含的主要元素总结

| 表单项   | 标签/属性                     | 功能说明      |
| ----- | ------------------------- | --------- |
| 文本输入框 | `<input type="text">`     | 输入普通文本    |
| 密码输入框 | `<input type="password">` | 输入密码，内容隐藏 |
| 单选按钮  | `<input type="radio">`    | 多选一       |
| 复选框   | `<input type="checkbox">` | 多选多       |
| 下拉列表  | `<select><option>`        | 从下拉菜单选择   |
| 文本域   | `<textarea>`              | 多行输入文字    |
| 文件上传  | `<input type="file">`     | 上传本地文件    |
| 提交按钮  | `<input type="submit">`   | 提交表单      |
| 重置按钮  | `<input type="reset">`    | 清空表单内容    |

---

### 表格相关的标签

---

### 一、核心结构标签

* `<table>`：表格容器。
* `<tr>`（table row）：表格的一行。
* `<th>`（table header cell）：**表头单元格**，默认加粗、居中；建议配合 `scope`。
* `<td>`（table data cell）：普通数据单元格。

> 语义与可访问性：
>
> * 表头请用 `<th>`，并加 `scope`：`scope="col"`（列头）、`scope="row"`（行头），或 `scope="colgroup"`/`rowgroup`（分组头）。
> * 复杂表头可用 `id` + `headers` 关联：在 `<th id="h1">`，对应 `<td headers="h1">`。

---

### 二、结构分区

* `<thead>`：表头区域（通常放列标题）。
* `<tbody>`：数据主体（多行数据）。
* `<tfoot>`：表尾（小计/合计/备注）。

> 浏览器会自动把缺失的分区补齐；合理分区有助于可读性和无障碍工具理解表格结构。

---

### 三、标题与说明

* `<caption>`：表格标题/说明文本（默认在表格上方，`caption-side: bottom;` 可改到底部）。

---

### 四、列定义（按列批量设样式）

* `<colgroup>`：列分组容器。
* `<col>`：定义某一列（或多列）的通用样式，如宽度、背景色等。可用 `span` 一次性作用多列。

```html
<colgroup>
  <col class="col-name">
  <col span="2" class="col-num">
  <col class="col-total">
</colgroup>
```

---

### 五、单元格合并

* `rowspan="n"`：纵向合并 **n** 行。
* `colspan="n"`：横向合并 **n** 列。

> 合并时要删除被合并覆盖的多余 `<td>/<th>`，否则列数对不上。

---

### 六、常用样式与属性建议

* 用 **CSS** 控制样式：

  * `border-collapse: collapse;` 折叠边框。
  * `border-spacing: 8px;`（在非折叠模式下控制单元格间距）。
  * `table-layout: fixed;` + 设定列宽，能稳定布局并避免抖动。
  * 斑马纹：`tbody tr:nth-child(even){ background: #fafafa; }`
  * 宽表格容器横向滚动：外包一层 `overflow-x: auto;`
  * 粘性表头：`thead th { position: sticky; top: 0; }`
* **过时/不推荐**：`border`、`cellpadding`、`cellspacing`、`align` 等旧属性，改用 CSS。

---

### 七、完整可运行示例（含粘性表头、列宽、合计、合并单元格）

> 直接保存为 `table-demo.html` 打开即可查看效果。

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8" />
<title>表格综合示例</title>
<style>
  body { font-family: system-ui, -apple-system, "Segoe UI", Arial, sans-serif; margin: 24px; background:#f7f8fa; }
  .table-wrap { max-width: 900px; margin: 0 auto; background:#fff; border:1px solid #e5e7eb; border-radius:12px; box-shadow:0 4px 14px rgba(0,0,0,.06); }
  .table-scroll { overflow-x:auto; border-radius:12px; }
  table { width: 100%; border-collapse: collapse; table-layout: fixed; }
  caption { text-align:left; font-weight:700; padding:16px 16px 0; font-size:18px; }
  thead th { position: sticky; top: 0; background:#f3f4f6; z-index:1; }
  th, td { border:1px solid #e5e7eb; padding:10px 12px; text-align:center; word-wrap:break-word; }
  tbody tr:nth-child(even) { background:#fafafa; }
  tfoot th, tfoot td { background:#f9fafb; font-weight:600; }
  /* 按列样式（来自 <colgroup> 的类名） */
  .col-name { width: 160px; }
  .col-q1, .col-q2, .col-q3 { width: 140px; }
  .col-total { width: 160px; }
  /* 行头单元格（scope=row）可左对齐增强可读性 */
  tbody th[scope="row"] { text-align:left; }
</style>
</head>
<body>

<div class="table-wrap">
  <div class="table-scroll">
    <table>
      <caption>2025 年各地区季度销售统计（单位：万元）</caption>

      <colgroup>
        <col class="col-name">
        <col class="col-q1">
        <col class="col-q2">
        <col class="col-q3">
        <col class="col-total">
      </colgroup>

      <thead>
        <tr>
          <th scope="col">地区</th>
          <th scope="col">Q1</th>
          <th scope="col">Q2</th>
          <th scope="col">Q3</th>
          <th scope="col">合计</th>
        </tr>
      </thead>

      <tbody>
        <tr>
          <th scope="row">华北</th>
          <td>120</td>
          <td>135</td>
          <td>142</td>
          <td>397</td>
        </tr>
        <tr>
          <th scope="row">华东</th>
          <td>150</td>
          <td>158</td>
          <td>166</td>
          <td>474</td>
        </tr>
        <!-- 示例：合并行，把“西南”做成一个大类，包含重庆与四川两行 -->
        <tr>
          <th scope="row" rowspan="2">西南</th>
          <td>80</td>
          <td>86</td>
          <td>93</td>
          <td>259</td>
        </tr>
        <tr>
          <!-- 此处行头已由上一行 rowspan 占位，故不再写 -->
          <td>92</td>
          <td>99</td>
          <td>105</td>
          <td>296</td>
        </tr>
      </tbody>

      <tfoot>
        <tr>
          <th scope="row">总计</th>
          <!-- 演示 colspan：把 Q1~Q3 三列合并展示汇总说明 -->
          <td colspan="3">（Q1~Q3 汇总）</td>
          <td>1,426</td>
        </tr>
      </tfoot>
    </table>
  </div>
</div>

</body>
</html>
```

---

### 八、最佳实践与易错点

1. **语义化表头**：用 `<th>` 而不是 `<td>` 充当表头，并加 `scope`。
2. **不要用表格做页面布局**：布局用 Flex/Grid，表格只呈现结构化数据。
3. **合并单元格**：使用 `rowspan/colspan` 时，删掉被覆盖的单元格，保证每行列数一致。
4. **宽表格可滚动**：外层包 `overflow-x:auto;`，避免小屏溢出。
5. **粘性表头**：长表格阅读体验更好（`position: sticky; top: 0;`）。
6. **按列设置样式**：使用 `<colgroup>/<col>` 统一设置列宽、背景色等，比在每个单元格写样式可维护。
7. **数值列对齐**：金额/数量类常用 `text-align: right;` 或居中，保持列内一致。
8. **可访问性**：复杂表头时考虑 `id/headers`；提供明确 `<caption>`。

---
###  Day 1 总结
#### 1.标签总结
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e84db3892a90480bbbaeb25456f53802.png)
#### 2.CSS总结
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e5cdeba0af0849c7b75f2b212f04f3cc.png)

# 🚀Day 2
---
## 知识要点 📌


### JavaScript的引入方式


在 HTML 中，我们使用 **`<script>` 标签** 来引入 JavaScript。常见有 **三种方式**：

---

### 1. **行内 JavaScript（直接写在标签里）**

* 直接在 HTML 元素的事件属性（比如 `onclick`、`onmouseover`）里写 JS 代码。
* 适合写一些很简单的交互，但不推荐大规模使用（会让代码很乱）。

🔹 示例：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>行内JS示例</title>
</head>
<body>
  <button onclick="alert('按钮被点击了！')">点我</button>
</body>
</html>
```

👉 点击按钮就会弹出提示框。

---

### 2. **内嵌 JavaScript（写在 `<script>` 标签里）**

* 把 JS 代码直接写在 HTML 页面 `<script>` 标签内部。
* 一般放在 **`<head>`** 或 **`</body>` 之前**（推荐放在 `</body>` 前，保证 HTML 先加载完）。

🔹 示例：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>内嵌JS示例</title>
  <script>
    function showMessage() {
      alert("欢迎学习 JavaScript！");
    }
  </script>
</head>
<body>
  <button onclick="showMessage()">点我</button>
</body>
</html>
```

👉 这样代码逻辑更清晰。

---

### 3. **外部 JavaScript 文件**

* 把 JS 单独写在一个 `.js` 文件里，然后用 `<script src="xxx.js"></script>` 引入。
* **推荐做法**：HTML 负责结构，CSS 负责样式，JS 负责逻辑，分开管理更清晰。

🔹 示例：

`index.html`

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <title>外部JS示例</title>
  <!-- 引入外部JS文件 -->
  <script src="main.js"></script>
</head>
<body>
  <button onclick="showMessage()">点我</button>
</body>
</html>
```

`main.js`

```javascript
function showMessage() {
  alert("这是外部 JS 文件里的代码！");
}
```

👉 推荐使用这种方式，因为更好维护。

---

### ⚡ 总结：

1. **行内**： `<button onclick="alert('Hi')">点我</button>` （不推荐，代码和结构耦合）。
2. **内嵌**： `<script> ... </script>` （适合小页面临时用）。
3. **外部**： `<script src="xxx.js"></script>` （推荐，大型项目都用这个）。

---

### JavaScript 的变量和数据类型
### 一、什么是变量？

👉 **变量就是用来存储数据的“容器”**，你可以把它理解为一个带名字的盒子。
比如：

```javascript
let name = "Tom";
```

这里：

* `let`：表示定义一个变量
* `name`：变量的名字（盒子的标签）
* `"Tom"`：变量存储的内容（放进盒子的东西）

以后你就可以用 `name` 这个名字来访问 `"Tom"` 了。

---

### 二、变量的声明方式

JavaScript 有 **3 种**声明变量的方式：

1. **let**

   * 常用，推荐
   * 可以改变值

   ```javascript
   let age = 18;
   age = 20;  // 可以改
   ```

2. **const**

   * 常量，值不能改
   * 必须在声明时赋值

   ```javascript
   const PI = 3.14;
   // PI = 3.1415; ❌ 报错
   ```

3. **var**

   * 旧语法，现在一般不用
   * 作用域规则比较怪

---

### 三、JavaScript 的数据类型

JavaScript 有 **两大类数据类型**：

* **基本类型**（值类型）
* **引用类型**（复杂对象）

### 1. 基本数据类型（7种）

可以理解为存放在“盒子”里的简单值。

1. **Number**：数字（整数、小数）

   ```javascript
   let a = 10;
   let b = 3.14;
   ```

2. **String**：字符串（文本）

   * 用 `""` 或 `''` 或 `` `模板字符串` `` 包裹

   ```javascript
   let name = "Alice";
   let msg = 'Hello';
   let info = `My name is ${name}`;
   ```

3. **Boolean**：布尔值（true / false）

   ```javascript
   let isOk = true;
   let isDone = false;
   ```

4. **Undefined**：未定义（声明了但没赋值）

   ```javascript
   let x;
   console.log(x); // undefined
   ```

5. **Null**：空值，表示“没有对象”

   ```javascript
   let data = null;
   ```

6. **Symbol**（ES6 引入）：唯一标识符

   ```javascript
   let s1 = Symbol("id");
   let s2 = Symbol("id");
   console.log(s1 === s2); // false
   ```

7. **BigInt**（ES11 引入）：大整数

   ```javascript
   let big = 123456789012345678901234567890n;
   ```

---

### 2. 引用数据类型（复杂数据）

存储的是 **对象的引用地址**，常见有：

1. **Object**：对象

   ```javascript
   let person = {
       name: "Tom",
       age: 20
   };
   ```

2. **Array**：数组（多个数据的集合）

   ```javascript
   let numbers = [1, 2, 3, 4, 5];
   ```

3. **Function**：函数

   ```javascript
   function greet() {
       console.log("Hello!");
   }
   ```

---

### 四、检查数据类型

用 `typeof` 来判断数据类型：

```javascript
console.log(typeof 123);       // number
console.log(typeof "hello");   // string
console.log(typeof true);      // boolean
console.log(typeof undefined); // undefined
console.log(typeof null);      // object (特殊情况)
console.log(typeof {});        // object
console.log(typeof []);        // object
console.log(typeof function(){}); // function
```

---

### 五、总结口诀

* **let 常用，const 不变，var 少用**
* **基本类型 7 个：数字、字符串、布尔、undefined、null、symbol、bigint**
* **引用类型：对象、数组、函数等**

---

### JavaScript 的函数
### 1. 什么是函数？

👉 函数就是一段可以 **被重复使用** 的代码，它能接收输入（参数），执行一些操作，然后给你一个输出（返回值）。
好处就是：**避免写重复代码，提高代码可读性和可维护性**。

---

### 2. 函数的基本结构

```javascript
function 函数名(参数1, 参数2, ...) {
    // 函数体（要执行的代码）
    return 返回值; // 可选
}
```

🔎 解释：

* `function` —— 定义函数的关键字
* `函数名` —— 给函数起的名字（见名知意，方便调用）
* `参数` —— 输入的值（类似传进小机器的原材料）
* `return` —— 返回结果（小机器产出的东西）

---

### 3. 示例

### (1) 一个简单的函数

```javascript
function sayHello() {
    console.log("你好，JavaScript!");
}
sayHello(); // 调用函数
```

👉 输出结果：

```
你好，JavaScript!
```

### (2) 带参数的函数

```javascript
function greet(name) {
    console.log("你好，" + name + "!");
}
greet("小明"); // 你好，小明!
greet("翠花"); // 你好，翠花!
```

🔑 参数 `name` 就像一个变量，你在调用函数时给它赋值。

---

### (3) 带返回值的函数

```javascript
function add(a, b) {
    return a + b; // 返回两个数的和
}
let result = add(3, 5);
console.log(result); // 8
```

👉 有了 `return`，函数就可以像一个计算器，算出结果给你。

---

### 4. 函数的几种写法

### (1) 普通函数声明

```javascript
function sayHi() {
    console.log("Hi!");
}
```

### (2) 函数表达式

```javascript
let sayHi = function() {
    console.log("Hi!");
};
```

👉 把函数存进变量里，也能调用。

### (3) 箭头函数（ES6）

```javascript
let add = (a, b) => a + b;
console.log(add(2, 3)); // 5
```

👉 更简洁，常用于回调函数。

---

### 5. 函数的好处

✅ 让代码更清晰、结构化
✅ 避免重复写代码
✅ 方便调试和维护
✅ 提高代码复用率

---

### JavaScript 自定义对象
### 1. 什么是对象？

在 JavaScript 中，对象就是一个“容器”，里面存放的是 **属性（数据）** 和 **方法（行为）**。
可以理解为：对象 = 名词 + 动作。

比如描述一个人：

* **属性**：名字、年龄、性别
* **方法**：说话、走路

---

### 2. 创建对象的几种方式

### 方式一：对象字面量（最常用 ✅）

```javascript
let person = {
  name: "Tom",
  age: 20,
  gender: "male",
  sayHello: function() {
    console.log("Hello, my name is " + this.name);
  }
};

console.log(person.name);  // Tom
person.sayHello();         // Hello, my name is Tom
```

📌 解释：

* `name, age, gender` 是对象的 **属性**
* `sayHello` 是对象的 **方法**
* `this` 代表当前对象本身

---

### 方式二：使用 `new Object()`

```javascript
let car = new Object();
car.brand = "Tesla";
car.color = "red";
car.run = function() {
  console.log(this.brand + " is running!");
};

console.log(car.color);  // red
car.run();               // Tesla is running!
```

👉 这种写法比较老，现在更推荐 **字面量**。

---

### 方式三：工厂函数（适合创建多个对象）

```javascript
function createPerson(name, age) {
  return {
    name: name,
    age: age,
    sayHi: function() {
      console.log("Hi, I am " + this.name);
    }
  };
}

let p1 = createPerson("Alice", 18);
let p2 = createPerson("Bob", 22);

p1.sayHi(); // Hi, I am Alice
p2.sayHi(); // Hi, I am Bob
```

👉 像“工厂生产对象”一样。

---

### 方式四：构造函数（推荐，和类很像）

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
  this.sayHi = function() {
    console.log("Hi, my name is " + this.name);
  };
}

let p1 = new Person("Jack", 25);
let p2 = new Person("Lily", 30);

p1.sayHi(); // Hi, my name is Jack
```

📌 解释：

* `Person` 就像一个“类”，用来描述人
* `new Person()` 就是创建对象的过程

---

### 方式五：ES6 的 `class`（语法糖）

```javascript
class Animal {
  constructor(type, name) {
    this.type = type;
    this.name = name;
  }

  speak() {
    console.log(this.name + " the " + this.type + " is speaking!");
  }
}

let dog = new Animal("dog", "Lucky");
dog.speak();  // Lucky the dog is speaking!
```

---

### 3. 总结

JavaScript 创建对象有很多方式：

1. **字面量**（简单、常用）
2. **new Object()**（较少用）
3. **工厂函数**（适合批量）
4. **构造函数**（常用，类似类）
5. **class（ES6 语法糖）**（现代开发推荐 ✅）

---


### JSON
### 1. 什么是 JSON

* **JSON** 全称是 **JavaScript Object Notation**，即 **JavaScript 对象表示法**。
* 它是一种 **轻量级的数据交换格式**，常用于 **前后端传输数据**。
* 语法和 JavaScript 的对象非常像，但更严格。

👉 举个例子，一个学生的信息：

```json
{
  "name": "小明",
  "age": 18,
  "isStudent": true,
  "hobbies": ["篮球", "编程", "音乐"],
  "address": {
    "city": "北京",
    "zip": "100000"
  }
}
```

---

### 2. JSON 的语法规则

1. **数据以键值对形式存储**：`"key": value`
2. **键必须是双引号包裹的字符串**

   * ✅ 正确：`"name": "小明"`
   * ❌ 错误：`name: "小明"`
3. **值可以是以下类型**：

   * 字符串（必须用双引号 `""`）
   * 数字
   * 布尔值（`true` / `false`）
   * 数组（`[]`）
   * 对象（`{}`)
   * `null`
4. **不能写注释**（和 JavaScript 对象不同）

---

### 3. JSON 与 JavaScript 的区别

* JSON 是 **数据格式**（像字符串），JavaScript 对象是 **代码中的对象**。
* 在 JavaScript 中：

  * **对象**：

    ```js
    let student = { name: "小明", age: 18 };
    ```
  * **JSON（字符串）**：

    ```js
    let studentJSON = '{"name": "小明", "age": 18}';
    ```

---

### 4. JSON 与 JavaScript 的互相转换

JavaScript 提供了两个方法：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8fed920effec421f983103d5a0bb3da3.png)
1. **JSON 转对象**

   ```js
   let jsonStr = '{"name": "小明", "age": 18}';
   let obj = JSON.parse(jsonStr);
   console.log(obj.name); // 输出 "小明"
   ```

2. **对象转 JSON**

   ```js
   let obj = { name: "小明", age: 18 };
   let jsonStr = JSON.stringify(obj);
   console.log(jsonStr); // 输出 '{"name":"小明","age":18}'
   ```

---

### 5. JSON 的应用场景

* **前后端通信**：服务器返回数据给前端时，常用 JSON 格式。
* **配置文件**：如 `package.json`、`tsconfig.json`。
* **数据存储**：浏览器 `localStorage`、`sessionStorage` 中可以存 JSON 字符串。

---

✨ 总结一下：

* JSON 是一种 **数据格式**，看起来像 JavaScript 对象，但更严格。
* 常用于 **存储和传输数据**。
* JavaScript 用 `JSON.parse()` 和 `JSON.stringify()` 来解析和转换。

---


### DOM
### 1. DOM 是什么？

DOM 全称是 **Document Object Model**（文档对象模型）。
它是 **浏览器用来表示网页内容的一种模型**。

你可以把 DOM 想象成：
👉 网页 = 一个“树形结构”的文档对象。
👉 这棵树里的每个节点，都是网页里的一个部分，比如标签、属性、文本等。

---

### 2. 为什么要有 DOM？

因为网页本质上是 **HTML 文件**，浏览器需要一种方式把这堆标签解析出来，并且让 JavaScript 能操作它。

所以：

* 浏览器加载 HTML → 生成 DOM 树
* JavaScript 就可以用 DOM API 去访问、修改网页内容

---

### 3. DOM 的结构（树形）
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/454614741a57495da559b129c033207b.png)
举个例子：

```html
<!DOCTYPE html>
<html>
  <head>
    <title>我的网页</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>这是一个段落</p>
  </body>
</html>
```

转成 DOM 树长这样：

```
Document
 └── html
     ├── head
     │    └── title
     │          └── "我的网页"
     └── body
          ├── h1
          │    └── "Hello World"
          └── p
               └── "这是一个段落"
```

---

### 4. DOM 节点的类型

DOM 把网页里的东西分成 **节点 (Node)**，常见有：

* **元素节点 (Element)**：比如 `<h1>`、`<p>`
* **属性节点 (Attribute)**：比如 `<p id="test">` 里的 `id="test"`
* **文本节点 (Text)**：比如 `"Hello World"`

---

### 5. JavaScript 操作 DOM

我们可以用 JS 访问和修改 DOM：

### 获取元素

```js
let title = document.getElementById("myTitle");
let paragraphs = document.getElementsByTagName("p");
```

### 修改内容

```js
document.getElementById("myTitle").innerText = "新的标题";
```

### 修改样式

```js
document.getElementById("myTitle").style.color = "red";
```

### 创建元素

```js
let newP = document.createElement("p");
newP.innerText = "我是新段落";
document.body.appendChild(newP);
```

---

### 6. 总结（通俗记忆）

* DOM 就是 **浏览器把网页变成一棵树**
* JS 可以通过 DOM **查找、修改、删除、添加** 节点
* DOM 是 **HTML、CSS、JS 之间的桥梁**

---

### DOM操作
### 一、先说两个重要概念

* **DOM = 浏览器把 HTML 解析成的一棵节点树**，JavaScript 操作 DOM 就是增删改查这棵树的节点。
* **重排（reflow）/ 重绘（repaint）**：改 DOM 或样式会触发浏览器计算布局与绘制，频繁修改会很慢——后面会讲性能优化。

---

### 二、**查找 / 选择 元素**（Selector）

常用 API（从推荐到不推荐）：

```js
// 推荐（灵活，支持 CSS 选择器）
const el = document.querySelector('#id');        // 单个元素（第一个匹配）
const list = document.querySelectorAll('.cls');  // NodeList（静态，不是实时更新）

// 经典 API（返回实时集合或老式方法）
const elById = document.getElementById('id');   // 性能最好，专门选 id
const byClass = document.getElementsByClassName('cls'); // HTMLCollection（live）
const byTag = document.getElementsByTagName('div');     // HTMLCollection（live）
```

> **注意**：`getElementsByClassName`、`getElementsByTagName` 返回的集合是 **live（实时）**，DOM 改变会同步更新集合；而 `querySelectorAll` 返回的是**静态 NodeList**（不会自动更新）。

---

### 三、**遍历 DOM 节点**

常用属性和方法：

```js
el.parentElement       // 父元素
el.children            // 只包含元素节点（HTMLCollection）
el.childNodes          // 包含文本节点、注释等（NodeList）
el.firstElementChild
el.lastElementChild
el.previousElementSibling
el.nextElementSibling
```

---

### 四、**创建 / 插入 / 删除 / 替换 元素**

现代 DOM API 很丰富，常用方法：

```js
// 创建
const li = document.createElement('li');
li.textContent = '项 1';                // 推荐用 textContent 避免 XSS
li.className = 'item';
li.setAttribute('data-id', '123');

// 插入（多种）
parent.appendChild(li);                 // 最经典（只支持单个节点）
parent.append(li);                      // 现代：支持 Node 和 字符串，且可以多个参数
parent.prepend(newNode);                // 插入到开头
referenceNode.insertBefore(node, referenceNode.nextSibling); // 在指定位置前插入
node.after(otherNode);                   // 在当前元素之后插入（现代）
node.before(otherNode);                  // 在当前元素之前插入（现代)

// 批量插入（性能好）
const frag = document.createDocumentFragment();
for (...) frag.appendChild(item);
parent.appendChild(frag);

// 删除
node.remove();                          // 现代
parent.removeChild(child);              // 传统

// 替换
parent.replaceChild(newNode, oldNode);  // 传统
oldNode.replaceWith(newNode);           // 现代
```

**提示**：尽量优先用现代方法（`append` / `remove` / `replaceWith`），代码更简洁。

---

### 五、**属性与属性/属性 vs. 属性/属性值 (attributes vs properties)**

* HTML 属性（attribute）存在于标记中，比如 `<input id="a" value="x">`。
* DOM 属性（property）是 JS 对象的字段，比如 `input.value`、`input.id`。

常用：

```js
el.id = 'myId';
el.setAttribute('data-id', '123');
const v1 = el.getAttribute('data-id');
const v2 = el.dataset.id;    // data-* 的快捷访问
```

**注意差异**：

* `elem.href` 可能返回绝对 URL，而 `getAttribute('href')` 返回原始写在 HTML 的值。
* `checked`、`value` 等是 property（会反映当前状态），`getAttribute` 读的是初始属性。

---

### 六、**内容操作（文本/HTML）**

```js
el.textContent = '纯文本';    // 推荐：安全（会转义）
el.innerText = '显示文本';    // 会考虑 CSS，触发回流更频繁
el.innerHTML = '<b>加粗</b>'; // 插入 HTML（可能引起 XSS），慎用
el.outerHTML = '<div>替换整个元素</div>'; // 用于替换当前元素本身
```

* 如果插入用户提供的内容，**千万别用 innerHTML** 除非经过严格清洗。

---

### 七、**样式修改**

```js
// 直接设置内联样式
el.style.backgroundColor = 'lightblue';
el.style.cssText += 'padding: 10px; border-radius:5px;';

// 操作类名（推荐）
el.classList.add('active');
el.classList.remove('active');
el.classList.toggle('open');
el.classList.contains('open');

// 整体替换类名
el.className = 'foo bar';
```

优先用 `classList` + CSS 类来控制样式，而不是大量直接写 `style`。

---

### 八、**事件处理（重要）**

#### 添加 / 移除监听器

```js
function onClick(e) {
  console.log('clicked', e.target);
}
el.addEventListener('click', onClick);
el.removeEventListener('click', onClick);
```

* 可选第三个参数 `{ capture: false, once: false, passive: false }`（其中 `once:true` 只触发一次）。
* **不要**使用 `onclick = fn`（会覆盖其他监听器），推荐 `addEventListener`。

#### 事件对象（Event）

* `e.target`：事件发生的真实元素（可能是子元素）。
* `e.currentTarget`：被绑定监听器的元素。
* `e.preventDefault()`：阻止默认行为（如 a 链接跳转、表单提交）。
* `e.stopPropagation()`：阻止事件冒泡（通常少用）。

#### 事件委托（Event Delegation）

对动态列表尤其重要，**在父容器上绑定一次监听**，通过判断 `e.target` 处理子项，避免给每个子元素都绑监听，性能好、维护方便。

```js
list.addEventListener('click', e => {
  const btn = e.target.closest('.delete-btn');
  if (btn) {
    const li = btn.closest('li');
    li.remove();
  }
});
```

---

### 九、**表单与输入控件交互**

```js
const val = document.querySelector('#username').value;
document.querySelector('#checkbox').checked = true;
const sel = document.querySelector('#city').value; // select 的 value
```

* 使用 `FormData` 快速收集表单数据（支持文件上传）：

```js
const form = document.querySelector('form');
const data = new FormData(form);
fetch('/api', { method: 'POST', body: data });
```

---

### 十、**性能优化（避免回流/重绘）**

典型建议：

1. **批量 DOM 更新**：用 `DocumentFragment` 或先构造字符串再 `innerHTML`（谨慎）或批量 `append`。
2. **避免布局抖动（layout thrashing）**：不要在循环里交替读写会触发布局的属性（如 `offsetWidth`、`clientHeight`、`getComputedStyle`）。先读取所有需要的，再一次性写入。
3. **使用事件委托**，避免给大量子元素绑定事件。
4. **使用 `requestAnimationFrame`** 做与动画相关的 DOM 更新。
5. **缓存选择器**：不要在循环中多次调用 `document.querySelector` 去选同一个元素。

---

### 十一、**安全注意（XSS）**

* 尽量使用 `textContent` 而不是 `innerHTML` 去插入用户数据。
* 如果必须插入 HTML，使用可信库（DOMPurify）做清洗，或后端返回安全数据。
* 使用 `Content-Security-Policy` (CSP) 限制内联脚本/外域资源也很重要。

---

### 十二、**现代补充 API**

* `Element.matches(selector)`：判断元素是否匹配选择器。
* `Element.closest(selector)`：向上查找最近的匹配父元素。
* `Node.cloneNode(true|false)`：克隆节点（`true` 深度克隆）。
* `MutationObserver`：监听 DOM 变化（替代 `DOMNodeInserted` 等弃用事件）。

---

### 十三、**生命周期与脚本加载**

* 把脚本放在 `</body>` 前可保证 DOM 已经解析完再执行。
* 或用 `<script defer src="...">`，页面解析时会并行加载脚本，脚本会在 DOM 解析完成后执行。
* 或监听 `DOMContentLoaded`：

```js
document.addEventListener('DOMContentLoaded', () => {
  // DOM 已解析完毕
});
```

---

### 十四、实践示例：**Todo List（完整可运行）**

下面是一个小型 Todo 应用，演示常见 DOM 操作：选择、创建、插入、删除、事件委托、DocumentFragment、localStorage 持久化。

把下面代码保存为 `todo.html`，直接在浏览器打开即可运行。

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="utf-8" />
  <title>DOM 实战：Todo List</title>
  <style>
    body { font-family: Arial, sans-serif; padding:20px; background:#f6f8fb; }
    .wrap { max-width:640px; margin:0 auto; background:#fff; padding:20px; border-radius:8px; box-shadow:0 6px 18px rgba(0,0,0,.06); }
    h1 { margin-top:0; }
    form { display:flex; gap:8px; }
    input[type="text"] { flex:1; padding:8px 10px; border-radius:4px; border:1px solid #ddd; }
    button { padding:8px 14px; border:none; background:#2d8cf0; color:#fff; border-radius:4px; cursor:pointer; }
    ul { list-style:none; padding:0; margin-top:16px; }
    li { display:flex; justify-content:space-between; padding:10px; border-bottom:1px solid #f0f0f0; align-items:center; }
    li.completed .text { text-decoration:line-through; color:#999; }
    .controls button { margin-left:8px; background:#e74c3c; }
    .controls button.info { background:#999; }
  </style>
</head>
<body>
  <div class="wrap">
    <h1>Todo List</h1>
    <form id="todoForm">
      <input id="todoInput" type="text" placeholder="写下你的任务并回车或点击添加" required />
      <button type="submit">添加</button>
    </form>

    <div style="margin-top:12px;">
      <button id="clearDone" class="info">清除已完成</button>
      <button id="clearAll" style="background:#999;color:#fff;margin-left:8px;">清空所有</button>
    </div>

    <ul id="todoList" aria-live="polite"></ul>
  </div>

  <script>
    // 简单的 TODO 管理（本地 localStorage 持久化）
    const form = document.getElementById('todoForm');
    const input = document.getElementById('todoInput');
    const list = document.getElementById('todoList');
    const CLEAR_DONE = document.getElementById('clearDone');
    const CLEAR_ALL = document.getElementById('clearAll');

    // 从 localStorage 载入
    const STORAGE_KEY = 'demo_todos_v1';
    let todos = JSON.parse(localStorage.getItem(STORAGE_KEY) || '[]');

    // 渲染单个 todo 到页面
    function createTodoNode(todo) {
      const li = document.createElement('li');
      li.dataset.id = todo.id;
      if (todo.done) li.classList.add('completed');

      li.innerHTML = `
        <span class="text">${escapeHtml(todo.text)}</span>
        <div class="controls">
          <button class="toggle">${todo.done ? '未完成' : '完成'}</button>
          <button class="delete">删除</button>
        </div>
      `;
      return li;
    }

    // 渲染整个列表（使用 DocumentFragment 批量插入）
    function renderList() {
      list.innerHTML = ''; // 清空
      const frag = document.createDocumentFragment();
      for (const t of todos) {
        frag.appendChild(createTodoNode(t));
      }
      list.appendChild(frag);
    }

    // 保存到 localStorage
    function save() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(todos));
    }

    // 添加 todo
    form.addEventListener('submit', (e) => {
      e.preventDefault();
      const text = input.value.trim();
      if (!text) return;
      const todo = { id: Date.now().toString(), text, done: false };
      todos.push(todo);
      save();
      list.appendChild(createTodoNode(todo)); // 只插入新项，性能好
      input.value = '';
      input.focus();
    });

    // 事件委托：处理完成 & 删除（避免给每个按钮都绑定事件）
    list.addEventListener('click', (e) => {
      const btn = e.target;
      const li = btn.closest('li');
      if (!li) return;
      const id = li.dataset.id;
      if (btn.classList.contains('delete')) {
        // 删除
        todos = todos.filter(t => t.id !== id);
        save();
        li.remove();
      } else if (btn.classList.contains('toggle')) {
        // 切换完成状态
        const idx = todos.findIndex(t => t.id === id);
        if (idx >= 0) {
          todos[idx].done = !todos[idx].done;
          save();
          li.classList.toggle('completed', todos[idx].done);
          btn.textContent = todos[idx].done ? '未完成' : '完成';
        }
      }
    });

    // 批量操作
    CLEAR_DONE.addEventListener('click', () => {
      todos = todos.filter(t => !t.done);
      save();
      renderList();
    });
    CLEAR_ALL.addEventListener('click', () => {
      if (!confirm('确认清空所有吗？')) return;
      todos = [];
      save();
      renderList();
    });

    // 简单 XSS 避免：插入 text 时使用 textContent 或 escape
    function escapeHtml(str) {
      return String(str)
        .replace(/&/g, '&amp;')
        .replace(/</g, '&lt;')
        .replace(/>/g, '&gt;')
        .replace(/"/g, '&quot;')
        .replace(/'/g, '&#39;');
    }

    // 首次渲染
    renderList();
  </script>
</body>
</html>
```

**关键点说明：**

* 使用 `createElement` / `innerHTML`（但对用户文本我们先 `escapeHtml`）来构建节点。
* 使用 `DocumentFragment` 批量插入加速渲染。
* 使用事件委托（`list.addEventListener('click', ...)`）处理删除与切换，避免每个子项都新增监听器。
* 用 `dataset` 存放自定义 data-id（`li.dataset.id`）方便操作。
* 使用 `localStorage` 做简单持久化（演示用途）。

---

### 十五、常见坑与建议（小结）

* **不要滥用 `innerHTML`**（XSS 风险）。
* **避免在循环中频繁读写会触发布局的属性**（如 `offsetHeight`）。
* **优先用 `classList` 控制样式** 而非大量 `style` 直接写入。
* **事件委托** 对大量动态元素非常重要。
* **缓存 DOM 查询**（不要在循环中多次 `querySelector` 同一个节点）。
* **使用 `defer` 或把 script 放到 body 末尾**，以免 DOM 未加载而报错。
* **必要时用 MutationObserver** 监听复杂 DOM 变化，但要注意性能。

---
### 事件监听
### 1. 什么是事件监听？

事件监听（Event Listener）就是**在网页上“监听”某个事件的发生**，当事件触发时，执行你写好的代码。
👉 类似于你盯着一个按钮，一旦有人点它，你就会立刻做出反应。

常见事件：

* 鼠标事件：`click`（点击）、`mouseover`（鼠标移入）、`mouseout`（鼠标移出）
* 键盘事件：`keydown`（按下）、`keyup`（松开）
* 表单事件：`submit`、`change`、`input`
* 窗口事件：`load`（页面加载完）、`resize`（窗口大小变化）、`scroll`（页面滚动）

---

### 2. 添加事件监听的方式

### （1）HTML 内联方式（不推荐）

直接在 HTML 里写：

```html
<button onclick="alert('按钮被点击了！')">点我</button>
```

👉 缺点：结构和逻辑混在一起，不好维护。

---

### （2）JS 里的 DOM 属性方式

```html
<button id="btn">点我</button>
<script>
  const btn = document.getElementById("btn");
  btn.onclick = function () {
    alert("按钮被点击了！");
  };
</script>
```

👉 缺点：**一个事件只能绑定一个函数**，后写的会覆盖前面的。

---

### （3）推荐：`addEventListener`

```html
<button id="btn">点我</button>
<script>
  const btn = document.getElementById("btn");

  // 绑定多个事件处理函数
  btn.addEventListener("click", function () {
    alert("第一次反应！");
  });

  btn.addEventListener("click", function () {
    alert("第二次反应！");
  });
</script>
```

👉 优点：

* 同一个事件可以绑定多个监听器，互不覆盖。
* 更加灵活，可以用 `removeEventListener` 移除。

---

### 3. 事件对象（event）

当事件发生时，浏览器会自动生成一个事件对象 `event`，传递给回调函数。

```js
btn.addEventListener("click", function (event) {
  console.log(event); // 打印事件对象
  console.log("事件类型:", event.type); // click
  console.log("点击位置:", event.clientX, event.clientY);
});
```

---

### 4. 事件传播机制（冒泡 & 捕获）

DOM 事件有两种传播方式：

1. **捕获阶段**：从最外层（`document`）往下传递到目标元素。
2. **冒泡阶段**：从目标元素往上传递到 `document`。

默认是**冒泡**，也就是说如果你点击一个按钮，事件会从按钮触发，一直往上传给它的父元素、祖先元素。

例子：

```html
<div id="outer" style="padding:20px; background:lightblue">
  外层
  <button id="btn">点我</button>
</div>

<script>
  const outer = document.getElementById("outer");
  const btn = document.getElementById("btn");

  outer.addEventListener("click", () => {
    alert("外层 div 被触发（冒泡）");
  });

  btn.addEventListener("click", () => {
    alert("按钮被点击");
  });
</script>
```

👉 点击按钮时，先执行按钮的监听器，再执行外层的监听器（冒泡）。

如果要用捕获：

```js
outer.addEventListener("click", () => {
  alert("外层 div 捕获阶段触发");
}, true); // 第三个参数 true 表示捕获
```

---

### 5. 阻止事件传播 & 默认行为

* **阻止冒泡**

```js
btn.addEventListener("click", (event) => {
  event.stopPropagation(); // 阻止事件往上传
  alert("只执行按钮，不冒泡给外层");
});
```

* **阻止默认行为**（比如点击 `<a>` 会跳转，表单提交会刷新页面）

```js
document.querySelector("a").addEventListener("click", (event) => {
  event.preventDefault(); // 阻止跳转
  alert("阻止了默认行为");
});
```

---

### 6. 事件委托（重点技巧）

如果页面里有很多按钮，一个个绑定很麻烦，可以**把事件绑定在父元素上**，利用冒泡来统一处理。

```html
<ul id="list">
  <li>苹果</li>
  <li>香蕉</li>
  <li>橘子</li>
</ul>

<script>
  const list = document.getElementById("list");

  list.addEventListener("click", function (event) {
    if (event.target.tagName === "LI") {
      alert("你点击了：" + event.target.innerText);
    }
  });
</script>
```

👉 优点：节省内存，新加的子元素也能响应事件。

---

✅ 总结：

* 事件监听用 `addEventListener` 最好。
* 有事件对象 `event` 可以拿到各种信息。
* 事件传播有冒泡和捕获。
* 可以用 `stopPropagation` 阻止冒泡，用 `preventDefault` 阻止默认行为。
* 事件委托能提高效率。

---

### 常见事件
| 事件类型          | 事件名           | 触发时机                     | 常见应用        |
| ------------- | ------------- | ------------------------ | ----------- |
| **鼠标事件**      | `click`       | 单击元素时                    | 按钮点击、提交表单   |
|               | `dblclick`    | 双击元素时                    | 双击放大图片      |
|               | `mousedown`   | 鼠标按下时                    | 自定义拖拽、绘图工具  |
|               | `mouseup`     | 鼠标松开时                    | 拖拽释放        |
|               | `mousemove`   | 鼠标移动时                    | 跟随效果、绘图     |
|               | `mouseover`   | 鼠标移入元素时                  | 下拉菜单显示      |
|               | `mouseout`    | 鼠标移出元素时                  | 下拉菜单隐藏      |
|               | `mouseenter`  | 鼠标移入元素时（不冒泡）             | 更精准的 hover  |
|               | `mouseleave`  | 鼠标移出元素时（不冒泡）             | 更精准的 hover  |
| **键盘事件**      | `keydown`     | 键盘按下时                    | 快捷键监听       |
|               | `keyup`       | 键盘松开时                    | 输入框动态搜索     |
|               | `keypress`    | 按下字符键（已废弃，推荐用 `keydown`） | 旧版输入监听      |
| **表单事件**      | `input`       | 输入框内容发生变化时               | 搜索框实时提示     |
|               | `change`      | 输入框值改变且失去焦点时             | 下拉框选择、复选框勾选 |
|               | `focus`       | 元素获得焦点时                  | 输入框高亮       |
|               | `blur`        | 元素失去焦点时                  | 表单校验        |
|               | `submit`      | 表单提交时                    | 登录注册提交      |
| **窗口事件**      | `load`        | 页面资源加载完成时                | 页面初始化       |
|               | `resize`      | 窗口大小改变时                  | 响应式布局       |
|               | `scroll`      | 页面滚动时                    | 懒加载、回到顶部    |
|               | `unload`      | 页面关闭/刷新时                 | 统计数据上报      |
| **触摸事件**（移动端） | `touchstart`  | 手指触摸屏幕                   | 手势识别        |
|               | `touchend`    | 手指离开屏幕                   | 滑动结束        |
|               | `touchmove`   | 手指在屏幕滑动                  | 滑动切换        |
|               | `touchcancel` | 系统取消触摸时                  | 中断操作        |



# 🚀Day 3
---
## 知识要点 📌

---

# 🌱 Vue 常用指令讲解

在 Vue 中，**指令（Directive）** 是以 `v-` 开头的特殊属性，用来操作 DOM 或绑定数据。
核心思想就是：**把数据和页面绑定起来，页面会自动根据数据变化而更新**。

---

## 1. `v-bind` —— 动态绑定属性


很好 👍 你已经写出了 **`v-bind` 的基本用法**，我来给你做一个更全面的讲解和扩展。

---

### 1. 什么是 `v-bind`

* **作用**：把 Vue 实例中的数据 **动态绑定** 到 HTML 标签的 **属性** 上。
* **语法**：`v-bind:属性名="表达式"`
* **简写**：可以省略 `v-bind:`，只写 `:属性名`。

---

### 2. 常见绑定场景

#### （1）绑定 **src**

```vue
<img :src="imageUrl" alt="logo">
```

👉 当 `imageUrl` 改变时，图片会自动更新。

---

#### （2）绑定 **href**

```vue
<a :href="url" target="_blank">访问 Vue 官网</a>
```

👉 `url` 改变时，链接会自动更新。

---

#### （3）绑定 **class**

`v-bind:class` 可以动态控制样式类。

```vue
<div :class="{ active: isActive, error: hasError }"></div>
```

* 当 `isActive = true` 时，元素有 `active` 类。
* 当 `hasError = true` 时，元素有 `error` 类。

✅ 也可以直接绑定数组：

```vue
<div :class="[activeClass, errorClass]"></div>
```

---

#### （4）绑定 **style**

`v-bind:style` 可以动态绑定内联样式。

```vue
<div :style="{ color: textColor, fontSize: fontSize + 'px' }">
  动态样式
</div>
```

数据：

```javascript
data() {
  return {
    textColor: "red",
    fontSize: 20
  }
}
```

结果：

```html
<div style="color:red; font-size:20px;">动态样式</div>
```

---

#### （5）绑定 **多个属性**

Vue 提供对象语法，一次绑定多个属性：

```vue
<button v-bind="{ id: buttonId, disabled: isDisabled }">
  按钮
</button>
```

相当于：

```html
<button :id="buttonId" :disabled="isDisabled">按钮</button>
```

---

### 3. `v-bind` 的特点

* 适合绑定 **任意 HTML 属性**（src、href、title、id、disabled、class、style 等）。
* 表达式里可以写 **变量**、**计算结果**，甚至 **三元表达式**：

  ```vue
  <button :disabled="count <= 0">提交</button>
  ```

---

### 4. 一个综合案例

```vue
<template>
  <div>
    <!-- 动态图片 -->
    <img :src="imageUrl" :alt="altText">

    <!-- 动态链接 -->
    <a :href="url" target="_blank">访问官网</a>

    <!-- 动态 class -->
    <p :class="{ highlight: isHighlight }">动态类名</p>

    <!-- 动态 style -->
    <p :style="{ color: textColor, fontSize: fontSize + 'px' }">动态样式</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageUrl: "https://vuejs.org/images/logo.png",
      altText: "Vue Logo",
      url: "https://vuejs.org",
      isHighlight: true,
      textColor: "blue",
      fontSize: 18
    };
  }
};
</script>
```

---

✅ **一句话总结**：
`v-bind` 是 Vue 中 **动态绑定 HTML 属性** 的万能指令，凡是标签上的属性，都可以用它来实现数据驱动。

---




---

## 2. `v-model` —— 双向绑定

实现 **输入框与数据的双向绑定**。

```vue
<template>
  <div>
    <input v-model="name" placeholder="请输入名字">
    <p>你好，{{ name }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return { name: "" };
  }
};
</script>
```

📌 输入框内容变 → 数据变；数据变 → 输入框也更新。

---

## 3. `v-if` / `v-else-if` / `v-else` —— 条件渲染

根据条件决定是否渲染某个 DOM。

```vue
<template>
  <div>
    <p v-if="age >= 18">成年人</p>
    <p v-else-if="age > 12">青少年</p>
    <p v-else>小朋友</p>
  </div>
</template>

<script>
export default {
  data() {
    return { age: 16 };
  }
};
</script>
```

📌 Vue 会 **真正移除/添加 DOM 节点**。

---

## 4. `v-show` —— 显示/隐藏

和 `v-if` 类似，但它不会删除节点，只是控制 `display: none`。

```vue
<template>
  <p v-show="isVisible">我能显示或隐藏</p>
</template>

<script>
export default {
  data() {
    return { isVisible: true };
  }
};
</script>
```

📌 `v-if` 开销大（频繁增删 DOM），`v-show` 开销小（只是切换显示），选择看场景。

---
好的 👍 我给你整理一个 **`v-if` 和 `v-show` 的对比表格**，这样你可以快速理解两者的区别：

---

### Vue 中 `v-if` 与 `v-show` 的对比表

| 特性         | `v-if`                      | `v-show`                         |
| ---------- | --------------------------- | -------------------------------- |
| **本质**     | 条件渲染（真正的 DOM 节点增删）          | 条件展示（通过 `display: none` 控制显示/隐藏） |
| **DOM 开销** | 每次条件切换都会 **销毁和重建 DOM 节点**   | 只是在切换时 **修改 CSS 样式**，DOM 节点始终存在  |
| **初始渲染开销** | 如果条件为 `false`，不会渲染 DOM，性能较优 | 无论条件真假，都会渲染 DOM，初始开销稍大           |
| **切换开销**   | 切换开销大，因为涉及 DOM 的创建和销毁       | 切换开销小，只是修改样式                     |
| **适用场景**   | 条件不常变动（例如：登录框、权限相关 UI）      | 条件频繁切换（例如：Tab 切换、展开/收起）          |

---

📌 **一句话记忆**：

* **`v-if`** = 按需生成，条件为假就不渲染，适合 **不常变动的场景**。
* **`v-show`** = 先渲染再隐藏，适合 **频繁切换的场景**。

要不要我帮你把 **`v-if` / `v-show` 和 `v-bind` 常用指令整理成一个大表**，让你在学习 Vue 指令的时候有一个 **对照速查表**？

## 5. `v-for` —— 循环渲染

用来遍历数组或对象。

```vue
<template>
  <ul>
    <li v-for="(item, index) in items" :key="index">
      {{ index }} - {{ item }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return { items: ["苹果", "香蕉", "橘子"] };
  }
};
</script>
```

📌 `:key` 很重要，用来唯一标识节点，优化性能。

---

## 6. `v-on` —— 事件绑定

绑定事件（点击、输入、键盘等）。

```vue
<template>
  <button v-on:click="sayHello">点我</button>
  <!-- 简写 -->
  <button @click="sayHello">简写版</button>
</template>

<script>
export default {
  methods: {
    sayHello() {
      alert("你好 Vue！");
    }
  }
};
</script>
```

---

## 7. `v-html` —— 解析 HTML

直接把数据当成 HTML 插入。

```vue
<template>
  <div v-html="content"></div>
</template>

<script>
export default {
  data() {
    return { content: "<b>加粗文字</b>" };
  }
};
</script>
```

📌 ⚠️ 可能有 **XSS 攻击风险**，要小心用。

---

## 8. `v-text` —— 设置文本

和 `{{ }}` 插值一样，不过写在属性里。

```vue
<template>
  <p v-text="message"></p>
  <p>{{ message }}</p> <!-- 效果一样 -->
</template>

<script>
export default {
  data() {
    return { message: "Hello Vue" };
  }
};
</script>
```

---

# ✨ 总结常用指令

| 指令              | 作用                |
| --------------- | ----------------- |
| `v-bind`        | 动态绑定属性            |
| `v-model`       | 双向绑定表单输入          |
| `v-if / v-else` | 条件渲染（删除/添加 DOM）   |
| `v-show`        | 显示/隐藏（切换 display） |
| `v-for`         | 列表渲染              |
| `v-on` / `@`    | 绑定事件              |
| `v-html`        | 渲染 HTML           |
| `v-text`        | 设置文本              |

---

# 插值表达式
## 1. 插值表达式是什么？

在 Vue 模板中，插值表达式用 **双大括号 `{{ }}`** 表示，常用于把数据绑定到页面上。
简单来说：插值表达式就是在 HTML 模板里，动态显示 Vue 实例中的数据。

---

## 2. 基本用法

假设你的 Vue 实例里有以下数据：

```javascript
data() {
  return {
    message: "Hello Vue!",
    count: 10
  }
}
```

在模板里：

```html
<p>{{ message }}</p>   <!-- 输出 Hello Vue! -->
<p>{{ count }}</p>     <!-- 输出 10 -->
```

---

## 3. 插值里可以放什么？

插值表达式里面不仅可以放 **变量**，还可以放 **简单的 JavaScript 表达式**。

✅ 常见示例：

```html
<p>{{ count + 1 }}</p>          <!-- 输出 11 -->
<p>{{ message.toUpperCase() }}</p>  <!-- 输出 HELLO VUE! -->
<p>{{ count > 5 ? '大于5' : '小于等于5' }}</p>  <!-- 输出 大于5 -->
```

❌ 注意：不能放复杂的语句（比如 `if`、`for`、`while` 等），只能放**单个表达式**。

---

## 4. 特点

* **自动更新**：当 Vue 实例中的数据变化时，页面里的插值内容也会自动更新。
* **安全性**：Vue 会自动对插值内容进行 **HTML 转义**，防止 XSS 攻击。

  ```javascript
  data() {
    return {
      htmlCode: "<h1>我是标题</h1>"
    }
  }
  ```

  ```html
  <p>{{ htmlCode }}</p>  
  <!-- 页面上显示 <h1>我是标题</h1>，不会被解析成真正的标题 -->
  ```

如果你希望插入真正的 HTML，而不是转义后的字符串，需要用 **v-html 指令**。

---

## 5. 插值表达式的限制

* **不能写语句**（如 `if`、`for`），只能写表达式。
* **不能进行赋值操作**，比如 `{{ count = 100 }}` 是非法的。
* 复杂逻辑建议写到 **计算属性（computed）** 或 **方法（methods）** 里。

---

✅ **总结一句话**：
插值表达式 `{{ }}` 是 Vue 最常见的数据绑定方式，可以直接在页面中显示数据，并支持简单的 JS 表达式。

---

好嘞 👍 我用**通俗+代码演示**给你讲一下 **Axios** 的使用。Axios 是 Vue（或者 React、Node.js 等）里最常用的 HTTP 请求库，帮你从前端向后端请求数据。

---

## 1. 安装 Axios

如果你是用 Vue CLI 或 Vite 创建的项目，可以先装一下：

```bash
npm install axios
```

安装好以后就能用了。

---
# axios的使用方法
## 2. 基本用法

### （1）GET 请求（获取数据）

```javascript
import axios from "axios";

axios.get("https://jsonplaceholder.typicode.com/posts/1")
  .then(response => {
    console.log("返回数据：", response.data);
  })
  .catch(error => {
    console.error("出错了：", error);
  });
```

👉 **说明**：

* `get(url)` → 访问接口
* `response.data` → 取到返回的真实数据

---

### （2）POST 请求（提交数据）

```javascript
axios.post("https://jsonplaceholder.typicode.com/posts", {
    title: "Hello Vue",
    body: "Axios is easy!",
    userId: 1
  })
  .then(response => {
    console.log("提交成功：", response.data);
  })
  .catch(error => {
    console.error("出错了：", error);
  });
```

👉 **说明**：

* `post(url, data)` → 向后端提交数据
* 第二个参数就是提交的内容

---

## 3. 在 Vue 组件里用 Axios

假设你有一个 Vue 组件：

```vue
<template>
  <div>
    <h2>文章标题：{{ post.title }}</h2>
    <button @click="getPost">获取文章</button>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      post: {}
    };
  },
  methods: {
    getPost() {
      axios.get("https://jsonplaceholder.typicode.com/posts/1")
        .then(res => {
          this.post = res.data; // 更新数据
        })
        .catch(err => {
          console.error("请求失败：", err);
        });
    }
  }
};
</script>
```

👉 **说明**：

* 点击按钮调用 `getPost()`
* 请求到数据后用 `this.post = res.data` 更新页面

---

## 4. 常见用法总结

| 用法        | 语法                                                | 说明          |
| --------- | ------------------------------------------------- | ----------- |
| GET 请求    | `axios.get(url, { params: {id:1} })`              | 传 URL 参数    |
| POST 请求   | `axios.post(url, data)`                           | 提交数据        |
| PUT 请求    | `axios.put(url, data)`                            | 修改数据        |
| DELETE 请求 | `axios.delete(url)`                               | 删除数据        |
| 设置请求头     | `axios.get(url, { headers: {...} })`              | 自定义 headers |
| 全局配置      | `axios.defaults.baseURL = "http://api.test.com";` | 设置默认地址      |

---


# Promise 的两种不同使用方式
## 🔹 方式一：`.then().catch()` 写法

```javascript
axios.get("https://jsonplaceholder.typicode.com/posts/1")
  .then(res => {
    this.post = res.data; // 更新数据
  })
  .catch(err => {
    console.error("请求失败：", err);
  });
```

✅ 优点：

1. **简单直接**：不用写 `async function`，随时可以直接用。
2. **链式调用**：多个异步任务可以写成链式，很直观：

   ```js
   axios.get("/api/step1")
     .then(res => axios.get(`/api/step2/${res.data.id}`))
     .then(res2 => console.log(res2))
     .catch(err => console.error(err));
   ```
3. 对于**小逻辑**，写法简洁。

❌ 缺点：

* 当请求比较多、逻辑复杂时，会出现 **回调地狱**（虽然比回调函数好一点，但依旧不好读）。
* 错误处理不够灵活，所有错误都集中到最后一个 `.catch()`。

---

## 🔹 方式二：`async/await` 写法

```javascript
async mounted() {
  try {
    const res = await axios.get("https://jsonplaceholder.typicode.com/posts/1");
    this.post = res.data;
  } catch (err) {
    console.error("请求失败：", err);
  }
}
```

✅ 优点：

1. **可读性强**：看起来就像同步代码，逻辑很清晰。

   ```js
   const user = await axios.get("/user");
   const posts = await axios.get(`/user/${user.data.id}/posts`);
   ```

   读起来比 `.then()` 的嵌套更自然。
2. **错误处理灵活**：你可以在多个 `try...catch` 里分开处理不同请求的错误。
3. 更适合**复杂逻辑和长流程**的代码。

❌ 缺点：

* 必须在 `async` 函数里才能用。
* 多个请求并行时，如果写成 `await`，会变成顺序执行（效率低），需要配合 `Promise.all` 来优化：

  ```js
  const [user, posts] = await Promise.all([
    axios.get("/user"),
    axios.get("/posts")
  ]);
  ```

---

## 🔹 总结（通俗比喻）

* `.then().catch()` → **快餐风格**，写起来快，适合小任务。
* `async/await` → **家常菜风格**，代码可读性高，适合复杂逻辑。

如果你写的是 **Vue 项目**，在组件的 `mounted` 或 `methods` 里，一般推荐 **`async/await`**，因为逻辑清晰、维护方便。
但在一些一次性的小请求场景（比如按钮点击立即发起请求），用 `.then()` 更简洁。

---



### 示例代码（Vue 3 + CDN 版）

你可以直接复制到本地保存为 `index.html` 打开即可运行：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <title>Axios 链式调用查询示例</title>
  <!-- Vue 3 CDN -->
  <script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
  <!-- Axios CDN -->
  <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
</head>
<body>
  <div id="app">
    <h2>文章查询</h2>
    <input v-model="queryId" type="number" placeholder="输入文章ID (1-100)" />
    <button @click="fetchPost">查询</button>

    <div v-if="loading">正在加载中...</div>
    <div v-if="error" style="color:red;">请求失败：{{ error }}</div>

    <div v-if="post">
      <h3>文章标题：{{ post.title }}</h3>
      <p>{{ post.body }}</p>
    </div>
  </div>

  <script>
    const { createApp } = Vue;

    createApp({
      data() {
        return {
          queryId: 1,   // 输入框默认值
          post: null,   // 查询结果
          loading: false,
          error: null
        };
      },
      methods: {
        fetchPost() {
          this.loading = true;
          this.error = null;
          this.post = null;

          axios.get("https://jsonplaceholder.typicode.com/posts/" + this.queryId)
            .then(res => {
              this.post = res.data;   // 更新数据
            })
            .catch(err => {
              this.error = err.message;  // 捕获错误
            })
            .finally(() => {
              this.loading = false;  // 不管成功失败都执行
            });
        }
      }
    }).mount("#app");
  </script>
</body>
</html>
```

---

✅ 运行效果：

* 页面有一个输入框和按钮。
* 输入 **文章 ID (1-100)**，点击查询，就会请求 API，显示文章标题和内容。
* 查询时会显示 `正在加载中...`，失败时会显示红色的错误提示。

---
# vue的生命周期


## 🌀 什么是生命周期？

Vue 里的一个组件，从 **创建 → 挂载到页面 → 更新数据 → 销毁**，会经历一系列的过程。
就像人从 **出生 → 成长 → 工作学习 → 去世**。

Vue 给我们提供了一些 **钩子函数（生命周期函数）**，你可以在这些时刻“插队”，执行代码。

---

## 🌱 Vue2 生命周期流程（最常见的）

1. **beforeCreate**

   * 出生前，还没有血肉（`data`、`methods` 都还没初始化）。
   * 你啥都拿不到。

2. **created**

   * 出生了，有了血肉（`data`、`methods` 可以用了）。
   * 但是还没上舞台（页面 DOM 没渲染）。
   * 👉 常用来：发请求、处理数据。

3. **beforeMount**

   * 马上要登台了，后台已经准备好舞台（虚拟 DOM），但观众还看不到。

4. **mounted**

   * 正式上台，DOM 挂载到页面上。
   * 👉 常用来：操作 DOM、用第三方库（比如 echarts）。

---

### 🔄 更新阶段（数据变化 → 重新渲染）

5. **beforeUpdate**

   * 数据变了，但页面还没更新。
   * 👉 你还能拿到“旧的 DOM”。

6. **updated**

   * 页面 DOM 已经根据数据更新好了。
   * 👉 适合做“依赖 DOM 的操作”。

---

### ❌ 销毁阶段（组件被移除）

7. **beforeDestroy**

   * 还没死，活在最后一口气。
   * 👉 适合清理定时器、解绑事件。

8. **destroyed**

   * 彻底没了，组件实例销毁。

---

## 📊 生命周期图（简化记忆版）

```
创建阶段：beforeCreate → created → beforeMount → mounted
更新阶段：beforeUpdate → updated
销毁阶段：beforeDestroy → destroyed
```

---

## 🌟 Vue3 的变化（用 `setup`）

Vue3 里推荐用 **组合式 API** (`setup`)，生命周期钩子改了写法：

* `beforeCreate`、`created` → 都不需要了（逻辑放在 `setup` 里）
* `mounted` → `onMounted`
* `beforeUpdate` → `onBeforeUpdate`
* `updated` → `onUpdated`
* `beforeDestroy` → `onBeforeUnmount`
* `destroyed` → `onUnmounted`

👉 Vue3 就是把生命周期变成了 **函数调用形式**，更直观。

---

## 📌 举个例子（Vue2 写法）

```js
export default {
  data() {
    return {
      msg: "Hello Vue"
    }
  },
  created() {
    console.log("组件创建，数据是：", this.msg);
  },
  mounted() {
    console.log("组件挂载，DOM 可以用了");
  },
  beforeDestroy() {
    console.log("组件即将销毁，清理资源");
  }
}
```

---

`mounted` 是 Vue 生命周期钩子函数之一，它在 **组件挂载（渲染到真实 DOM）完成后立即执行**。这是一个非常重要的阶段，因为在这时你可以安全地操作 DOM、访问子组件、发起请求等。下面我帮你详细讲解一下。

---

## 📌 1. mounted 触发时机

- Vue 的生命周期大概是：
    
    1. 创建前（`beforeCreate`）
        
    2. 创建后（`created`）
        
    3. 挂载前（`beforeMount`）
        
    4. **挂载后（`mounted`）**
        
    5. 更新前（`beforeUpdate`）
        
    6. 更新后（`updated`）
        
    7. 销毁前（`beforeUnmount`）
        
    8. 销毁后（`unmounted`）
        

👉 `mounted` 的特点是：

- 在这个阶段，模板已经编译完成，并且 DOM 节点已经渲染到了页面中。
    
- 所以你可以在这里 **获取 DOM 节点**、**初始化第三方插件**、**发送请求加载数据**。
    

---

## 📌 2. mounted 的常见使用场景

1. **操作 DOM**
    
    ```vue
    <template>
      <div ref="box">Hello Vue</div>
    </template>
    
    <script>
    export default {
      mounted() {
        console.log(this.$refs.box.innerText); // Hello Vue
        this.$refs.box.style.color = "red";
      }
    }
    </script>
    ```
    
    👉 这里用 `ref` 拿到 DOM 节点，并修改颜色。
    

---

2. **发起网络请求（axios、fetch）**
    
    ```vue
    <template>
      <div>
        <h2>用户列表</h2>
        <ul>
          <li v-for="user in users" :key="user.id">{{ user.name }}</li>
        </ul>
      </div>
    </template>
    
    <script>
    import axios from "axios";
    
    export default {
      data() {
        return {
          users: []
        };
      },
      mounted() {
        axios.get("https://jsonplaceholder.typicode.com/users")
          .then(response => {
            this.users = response.data;
          })
          .catch(error => {
            console.error("请求出错：", error);
          });
      }
    }
    </script>
    ```
    
    👉 页面加载完成后，自动获取用户数据并展示。
    

---

3. **初始化第三方插件（如图表库 ECharts / 地图插件）**
    
    ```vue
    <template>
      <div ref="chart" style="width:400px; height:300px;"></div>
    </template>
    
    <script>
    import * as echarts from "echarts";
    
    export default {
      mounted() {
        const chart = echarts.init(this.$refs.chart);
        chart.setOption({
          title: { text: "示例图表" },
          xAxis: { data: ["A", "B", "C"] },
          yAxis: {},
          series: [{ type: "bar", data: [5, 20, 36] }]
        });
      }
    }
    </script>
    ```
    
    👉 `mounted` 里可以安全地初始化 ECharts，因为此时 DOM 节点已经存在。
    

---

4. **监听窗口事件**
    
    ```vue
    <script>
    export default {
      mounted() {
        window.addEventListener("resize", this.handleResize);
      },
      beforeUnmount() {
        window.removeEventListener("resize", this.handleResize);
      },
      methods: {
        handleResize() {
          console.log("窗口大小变化了", window.innerWidth);
        }
      }
    }
    </script>
    ```
    
    👉 常见于响应式布局，记得在组件销毁时解绑事件，避免内存泄漏。
    

---

## 📌 3. 注意事项

1. **不要在 mounted 里修改 data 并立即依赖 DOM**  
    因为修改 `data` 会触发重新渲染，可能导致 DOM 状态和预期不符。  
    如果必须等待 DOM 更新完成，可以用：
    
    ```js
    this.$nextTick(() => {
      // DOM 更新完成后执行
      console.log(this.$refs.box.offsetHeight);
    });
    ```
    
2. **适合做副作用操作**  
    比如请求数据、操作 DOM、绑定事件，但不建议写太多业务逻辑。
    

---

# 🚀Day 4
---
## 知识要点 📌

---
# Maven 的作用和使用方法



## 一、Maven 的作用

Maven 本质上是一个 **项目管理和构建工具**，尤其常用于 **Java 项目**。它的核心作用主要有以下几点：

1. **依赖管理（最重要）**

   * 开发一个 Java 项目时，经常需要用到第三方库（例如 MySQL 驱动、Spring、JUnit 等）。
   * 如果没有 Maven，开发者需要自己手动下载 jar 包，拷贝到项目中，维护起来很麻烦。
   * 有了 Maven，只需要在配置文件 `pom.xml` 中声明依赖（例如 mysql-connector），Maven 会自动从远程仓库下载合适版本的 jar 包并放到项目中。

   👉 相当于一个“包管理器”，类似于 Python 的 `pip` 或 JavaScript 的 `npm`。

---

2. **统一的项目结构和构建流程**

   * Maven 定义了一个标准化的项目目录结构，比如：

     ```
     src/main/java        → 源代码
     src/main/resources   → 配置文件
     src/test/java        → 单元测试代码
     target/              → 编译输出目录
     ```
   * 所有人用 Maven 创建的项目结构都一样，这样团队协作时就非常方便。

   👉 不需要自己定义项目的目录规范，直接遵循 Maven 约定即可。

---

3. **自动化构建**

   * Maven 提供了一个统一的命令来执行项目构建、编译、测试、打包、部署等操作。
   * 比如：

     * `mvn compile` 编译代码
     * `mvn test` 运行单元测试
     * `mvn package` 打包成 `.jar` 或 `.war` 文件
     * `mvn install` 安装到本地仓库，供其他项目使用

   👉 省去了一大堆手动执行的步骤，提高效率。

---

4. **插件机制**

   * Maven 自身功能有限，但可以通过插件扩展。
   * 比如：

     * 使用 `maven-compiler-plugin` 指定 Java 版本
     * 使用 `maven-surefire-plugin` 运行单元测试
     * 使用 `spring-boot-maven-plugin` 打包 Spring Boot 项目

   👉 灵活扩展，满足不同项目的需求。

---

## 二、Maven 的使用方法

### 1. 安装

1. 下载 [Maven](https://maven.apache.org/download.cgi)
2. 解压并配置环境变量（`MAVEN_HOME`、`PATH`）
3. 在命令行输入：

   ```bash
   mvn -v
   ```

   如果能显示版本号说明安装成功。

---

### 2. 创建项目

可以用 Maven 自带的命令创建一个 Java 项目：

```bash
mvn archetype:generate -DgroupId=com.example -DartifactId=myapp -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

这会创建一个标准化的项目结构。

---

### 3. 依赖管理

核心文件是 `pom.xml`，它用来描述项目信息和依赖。

示例：

```xml
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 
         http://maven.apache.org/xsd/maven-4.0.0.xsd">

    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>myapp</artifactId>
    <version>1.0-SNAPSHOT</version>

    <dependencies>
        <!-- MySQL 依赖 -->
        <dependency>
            <groupId>mysql</groupId>
            <artifactId>mysql-connector-java</artifactId>
            <version>8.0.33</version>
        </dependency>

        <!-- JUnit 单元测试 -->
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13.2</version>
            <scope>test</scope>
        </dependency>
    </dependencies>
</project>
```

只要写上这些依赖，Maven 就会自动去中央仓库下载 jar 包并加入项目。

---

### 4. 常用命令

| 命令            | 作用                     |
| ------------- | ---------------------- |
| `mvn clean`   | 清除编译输出（删除 `target` 目录） |
| `mvn compile` | 编译代码                   |
| `mvn test`    | 执行测试                   |
| `mvn package` | 打包成 `jar/war`          |
| `mvn install` | 安装到本地仓库（供其他项目使用）       |
| `mvn deploy`  | 部署到远程仓库                |

---

✅ 总结：

* **Maven = 包管理器 + 构建工具 + 项目管理工具**
* 它解决了依赖管理混乱、项目结构不统一、构建过程繁琐等问题
* 用法就是：写 `pom.xml` → 用 `mvn` 命令执行

---

# maven使用教程
[黑马的maven使用教程](https://heuqqdmbyk.feishu.cn/wiki/KTOKw4PvzipYeIkl3N5cSSxYnPb)

---
# Maven 的依赖管理
---
## 1. 什么是依赖管理？

在 Java 项目里，我们经常需要用到别人的代码库（第三方库），比如：

* Spring 框架
* MyBatis
* Gson / Jackson
* JUnit

如果你不用 Maven，以前需要自己：

1. 去官网找 jar 包下载
2. 拷贝到项目的 lib 目录
3. 手动配置 classpath

这样很麻烦，而且 **不同库之间还可能互相依赖**，你要一个个去找，非常累。

👉 **Maven 的依赖管理** 就是帮你 **自动下载、管理版本、处理传递依赖**，省心省力。

---

## 2. 依赖的基本配置

在 `pom.xml` 里声明依赖，比如我要用 Spring Context：

```xml
<dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>6.1.4</version>
    </dependency>
</dependencies>
```

含义：

* **groupId**：组织的唯一标识（相当于公司/组织名）
* **artifactId**：具体项目名（模块名）
* **version**：版本号

Maven 会自动去 **中央仓库** 下载对应的 jar 包。

---

## 3. 依赖的作用范围（scope）

不同依赖有不同的 **作用范围**（什么时候能用）：

* `compile`（默认）：编译 + 运行 + 打包 都需要（比如 Spring）
* `provided`：编译需要，但运行环境已经有了（比如 Servlet API，Tomcat 会提供）
* `runtime`：只在运行时需要（比如 JDBC 驱动）
* `test`：只在测试阶段需要（比如 JUnit）

示例：

```xml
<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.13.2</version>
    <scope>test</scope>
</dependency>
```

---

## 4. 传递依赖（Transitive Dependency）

重点 ⚡

如果你引入了 A，而 A 又依赖了 B，Maven 会 **自动帮你把 B 也下载好**。

例如：

* 你加了 `spring-context`
* 它会自动拉取 `spring-beans`、`spring-core` 等

👉 这就是你刚才看到的：

```
spring-context → spring-beans
```

spring-context 依赖 spring-beans，所以你间接获得了它。

---

## 5. 依赖冲突（版本冲突）

如果两个库依赖了同一个库的不同版本，Maven 默认会：

* 采用 **最短路径优先**（距离最近的版本）
* 路径相同时，取 **先声明的版本**

你可以用命令查看依赖树：

```bash
mvn dependency:tree
```

然后手动用 `<dependencyManagement>` 或 `<exclusions>` 来解决冲突。

---

## 6. 依赖管理（dependencyManagement）

在父 `pom.xml` 里统一规定版本号，子项目就不用每次写 `<version>`。

示例：

```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-context</artifactId>
            <version>6.1.4</version>
        </dependency>
    </dependencies>
</dependencyManagement>
```

子模块只需要：

```xml
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
</dependency>
```

---

## 7. 总结

Maven 依赖管理帮我们解决了 3 个大问题：

1. **自动下载 jar 包**（不用手动下载）
2. **自动处理传递依赖**（不用一个个去找）
3. **解决版本冲突**（提供统一管理机制）

---

好问题 👍 我用**通俗易懂**的方式给你讲一下 **单元测试（Unit Test）**。

---
# 测试

---

## 一、测试的基本概念

测试（Testing）就是在软件开发过程中，通过**设计和执行测试用例**，去验证软件是否满足需求、是否存在错误、是否达到预期的质量标准。

一句话理解：
👉 测试就是**发现问题、定位问题、预防问题**，保证软件质量。

---

## 二、测试的目的

1. **验证功能正确性**：检查程序是否按照需求文档实现。
2. **发现缺陷**：尽早暴露错误，降低后期修复成本。
3. **保证质量**：确保软件可用、稳定、安全。
4. **辅助开发**：通过测试反馈帮助开发人员改进设计和代码。

---

## 三、软件测试的分类

软件测试可以从不同角度分类：

### 1. 按执行方式

* **手工测试**：人工设计、执行用例，适合灵活性强的场景。
* **自动化测试**：通过脚本和工具自动执行测试，提高效率和可重复性。

### 2. 按测试阶段（软件生命周期）

* **单元测试**：验证某个最小单元（方法、类）的正确性。
* **集成测试**：验证不同模块之间的交互是否正确。
* **系统测试**：对完整系统进行验证，看是否符合需求。
* **验收测试**：最终由客户或用户确认系统是否满足业务目标。

### 3. 按测试内容

* **功能测试**：验证功能是否正确。
* **性能测试**：检查响应时间、并发处理能力、稳定性。
* **安全测试**：验证是否存在安全漏洞（SQL 注入、XSS、权限绕过）。
* **兼容性测试**：检查在不同系统、浏览器、设备上的表现。
* **回归测试**：修改代码后，验证之前的功能是否被破坏。

---

## 四、测试的基本流程

1. **分析需求**：理解要测试什么。
2. **设计测试用例**：编写输入、操作步骤、预期结果。
3. **准备测试环境**：配置服务器、数据库、测试数据。
4. **执行测试**：运行测试用例（手动或自动化）。
5. **缺陷管理**：记录 Bug，并跟踪修复情况。
6. **测试报告**：输出测试结论，给项目决策参考。

---

## 五、常见测试工具

* **单元测试**：JUnit（Java）、pytest（Python）。
* **自动化测试**：Selenium（UI 自动化）、Postman（接口测试）。
* **性能测试**：JMeter、LoadRunner。
* **持续集成**：Jenkins、GitHub Actions。

---

✅ 总结：
测试就是在软件开发中用来**保障质量、发现缺陷**的重要环节。它贯穿软件生命周期，从**单元测试**到**系统测试**，从**功能测试**到**性能、安全测试**，再到最终的**验收测试**。

---



 # 单元测试
## 1. 什么是单元测试？

* **定义**：单元测试就是对程序中**最小的可测试单元**（通常是一个方法或函数）进行验证，确保它的逻辑是正确的。
* **目的**：在代码开发阶段，快速验证每个小块代码是否按照预期运行。

比如，你写了一个计算器类：

```java
public class Calculator {
    public int add(int a, int b) {
        return a + b;
    }
}
```

👉 单元测试就是写一段“测试代码”去检查 `add(2,3)` 结果是不是等于 5。

---

## 2. 单元测试的特点

* **小范围**：只测一个类、一个方法，不依赖外部复杂环境。
* **自动化**：不用手动运行，可以直接运行测试方法，结果一目了然。
* **可重复**：随时都能跑，确保以后改动没把原来的功能搞坏（防止“回归错误”）。

---

## 3. 为什么要写单元测试？

* **提高代码质量**：发现 bug 越早，修复成本越低。
* **提高开发效率**：以后修改代码时，不用担心影响别的地方，跑一遍测试就知道。
* **促进良好设计**：代码更模块化、更清晰。

---

## 4. 在 Java 中怎么写单元测试（JUnit 示例）

最常见的是用 **JUnit**（单元测试框架）。

① 添加依赖（如果你用 Maven）：

```xml
<dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter</artifactId>
    <version>5.10.2</version>
    <scope>test</scope>
</dependency>
```

② 写测试类：

```java
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

public class CalculatorTest {

    @Test  // 表示这是一个测试方法
    public void testAdd() {
        Calculator calculator = new Calculator();
        int result = calculator.add(2, 3);
        assertEquals(5, result);  // 断言：期望结果是 5
    }
}
```

③ 运行测试：

* 如果通过 ✅ → 绿色
* 如果失败 ❌ → 红色，提示预期和实际不符

---

## 5. 单元测试常用的断言

* `assertEquals(expected, actual)` → 判断结果是否相等
* `assertTrue(condition)` → 判断条件是否为 true
* `assertThrows(Exception.class, () -> { ... })` → 判断是否抛出某个异常

---

## 6. 单元测试和其他测试的关系

* **单元测试**：测最小单元（函数、类）
* **集成测试**：测多个模块协同工作
* **系统测试**：测整个系统是否符合需求
* **验收测试**：最终交付前的用户测试

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f69e3e2836314b33812d88c8cce1152c.png)

---

👉 总结一句话：
**单元测试就是给你的代码戴上“安全网”，让你改代码时更安心。**

---

# 白盒测试、黑盒测试、灰盒测试

| 测试类型     | 关注点                  | 测试者是否了解代码          | 优点                                 | 缺点                    | 典型应用场景            |
| -------- | -------------------- | ------------------ | ---------------------------------- | --------------------- | ----------------- |
| **白盒测试** | 程序的内部逻辑、代码结构、执行路径    | 需要了解源码（开发人员常做）     | 可以覆盖内部逻辑，发现隐藏错误；能检查代码的执行情况（如分支、循环） | 对测试者要求高；无法发现需求或逻辑上的遗漏 | 单元测试、代码审查、覆盖率测试   |
| **黑盒测试** | 软件的功能是否满足需求（输入-输出关系） | 不需要了解源码（用户或测试人员常做） | 模拟真实用户使用，测试软件功能是否符合需求              | 无法发现代码层次的问题；覆盖率不够高    | 功能测试、系统测试、回归测试    |
| **灰盒测试** | 综合了白盒和黑盒的优点，部分了解代码实现 | 测试者对内部结构有部分了解      | 兼顾功能和逻辑，测试更高效，能发现更多问题              | 依赖测试者经验；容易遗漏深层逻辑问题    | 集成测试、安全测试、Web应用测试 |

📌 总结一句话：

* **白盒测试**：像 **修理工**，直接看引擎内部。
* **黑盒测试**：像 **司机**，只管开车，关心是否能跑起来。
* **灰盒测试**：像 **专业玩家**，既知道车的构造，又体验实际驾驶。

太好了 👍，既然你已经用 **Maven** 创建好了项目，那么我们就一步一步来写一个 **JUnit 单元测试案例**。我会用最常见的 **JUnit 5** 来演示。

---
# 实操单元测试
## 1. 确认依赖

在你的 `pom.xml` 里加入 JUnit 依赖（JUnit 5 版本）：

```xml
<dependencies>
    <!-- JUnit 5 单元测试依赖 -->
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter</artifactId>
        <version>5.10.2</version>
        <scope>test</scope>
    </dependency>
</dependencies>
```

然后执行：

```bash
mvn clean install
```

确保依赖下载成功。

---

## 2. 新建一个业务类

假设我们写一个最简单的 **计算器类**：

👉 在 `src/main/java/com/example/` 目录下创建 `Calculator.java`：

```java
package com.example;

public class Calculator {

    // 加法
    public int add(int a, int b) {
        return a + b;
    }

    // 除法
    public int divide(int a, int b) {
        if (b == 0) {
            throw new IllegalArgumentException("除数不能为0");
        }
        return a / b;
    }
}
```

---

## 3. 编写测试类

👉 在 `src/test/java/com/example/` 目录下创建 `CalculatorTest.java`：

```java
package com.example;

import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

class CalculatorTest {

    @Test
    void testAdd() {
        Calculator calc = new Calculator();
        int result = calc.add(2, 3);
        assertEquals(5, result, "2 + 3 应该等于 5");
    }

    @Test
    void testDivide() {
        Calculator calc = new Calculator();
        int result = calc.divide(10, 2);
        assertEquals(5, result, "10 / 2 应该等于 5");
    }

    @Test
    void testDivideByZero() {
        Calculator calc = new Calculator();
        Exception exception = assertThrows(IllegalArgumentException.class, () -> {
            calc.divide(10, 0);
        });
        assertEquals("除数不能为0", exception.getMessage());
    }
}
```

---

## 4. 运行测试

在项目根目录执行：

```bash
mvn test
```

如果一切正确，你会看到类似输出：

```
[INFO] Results:
[INFO] Tests run: 3, Failures: 0, Errors: 0, Skipped: 0
[INFO] BUILD SUCCESS
```

---

## 5. 验证点

* `testAdd()` ✅ 验证加法正确性
* `testDivide()` ✅ 验证正常除法
* `testDivideByZero()` ✅ 验证异常抛出

---

好的，我来给你**详细讲解 JUnit 里面的断言（Assertions）**，让你理解每种断言的作用和常用写法。我们以 **JUnit 5（Jupiter）** 为例。

---
# Junit中的断言
## 一、什么是断言（Assertions）？

**断言**是单元测试里用来 **判断测试结果是否符合预期** 的方法。

* 如果断言成立 → 测试通过
* 如果断言失败 → 测试失败，JUnit 会报告错误

一句话理解：**断言就是告诉 JUnit：“我期望这里的结果是这样，如果不是，就报错。”**

---

## 二、JUnit 常用断言方法

| 断言方法                                                   | 用法示例                                                                                               | 说明                     |
| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------- | ---------------------- |
| `assertEquals(expected, actual)`                       | `assertEquals(5, calc.add(2,3));`                                                                  | 判断实际值和期望值是否相等          |
| `assertNotEquals(unexpected, actual)`                  | `assertNotEquals(0, calc.add(2,3));`                                                               | 判断实际值和期望值不相等           |
| `assertTrue(condition)`                                | `assertTrue(calc.add(2,3) > 0);`                                                                   | 判断条件是否为真               |
| `assertFalse(condition)`                               | `assertFalse(calc.add(2,3) < 0);`                                                                  | 判断条件是否为假               |
| `assertNull(object)`                                   | `assertNull(obj);`                                                                                 | 判断对象是否为 null           |
| `assertNotNull(object)`                                | `assertNotNull(calc);`                                                                             | 判断对象是否不为 null          |
| `assertThrows(Exception.class, executable)`            | `assertThrows(IllegalArgumentException.class, () -> calc.divide(1,0));`                            | 判断指定操作是否抛出预期异常         |
| `assertAll("group name", executable1, executable2, …)` | `assertAll("检查多个断言", () -> assertEquals(5, calc.add(2,3)), () -> assertEquals(6, calc.add(3,3)));` | 组合多个断言，一起执行，方便同时验证多个条件 |
| `fail("message")`                                      | `fail("不应该执行到这里");`                                                                                | 强制测试失败，通常用于逻辑分支不该到达的情况 |

---

## 三、断言常用用法示例

```java
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

class CalculatorTest {

    Calculator calc = new Calculator();

    @Test
    void testAdd() {
        assertEquals(5, calc.add(2,3), "2 + 3 应该等于 5");
        assertNotEquals(4, calc.add(2,3));
        assertTrue(calc.add(2,3) > 0);
        assertFalse(calc.add(2,3) < 0);
    }

    @Test
    void testDivide() {
        assertEquals(2, calc.divide(6,3));
        // 断言异常
        Exception ex = assertThrows(IllegalArgumentException.class, () -> calc.divide(1,0));
        assertEquals("Division by zero", ex.getMessage());
    }

    @Test
    void testAllTogether() {
        assertAll("Calculator 组合断言",
            () -> assertEquals(5, calc.add(2,3)),
            () -> assertEquals(1, calc.subtract(3,2)),
            () -> assertThrows(IllegalArgumentException.class, () -> calc.divide(1,0))
        );
    }
}
```

---

## 四、总结

1. **断言是单元测试的核心**，所有测试结果都是通过断言判断的。
2. **JUnit 5 提供丰富的断言**，不仅能判断值，还能判断异常、组合多个断言。
3. **建议写测试时尽量加提示信息**（message 参数），方便发现问题。

---


好问题 👍，你贴的这一段其实是 **JUnit Jupiter（JUnit 5）的注解全集说明**。
我来给你详细拆解，分三步：

1. **逐类讲解这些注解的用法和场景**
2. **给出几个简单代码例子**
3. **最后做一张完整总结表格**

---

# JUnit 5 注解分类与用法

## 1. 基本测试注解

* **@Test**

  * 标记方法为测试方法。
  * 没有参数（不同于 JUnit4 的 `expected`、`timeout`）。

  ```java
  @Test
  void testAdd() {
      assertEquals(4, 2 + 2);
  }
  ```

* **@ParameterizedTest**

  * 参数化测试，可以用不同输入重复执行相同逻辑。

  ```java
  @ParameterizedTest
  @ValueSource(ints = {1, 2, 3})
  void testWithParams(int num) {
      assertTrue(num > 0);
  }
  ```

* **@RepeatedTest(n)**

  * 重复执行测试 n 次。

  ```java
  @RepeatedTest(3)
  void repeatedTest() {
      System.out.println("执行一次");
  }
  ```

* **@TestFactory**

  * 工厂方法，动态生成测试用例。

  ```java
  @TestFactory
  Stream<DynamicTest> dynamicTests() {
      return Stream.of("a", "b", "c")
          .map(str -> DynamicTest.dynamicTest("测试 " + str,
                  () -> assertTrue(str.length() == 1)));
  }
  ```

* **@TestTemplate**

  * 定义一个测试模板，由扩展调用多次。
    （常见于集成测试框架扩展，普通开发用得少）

---

## 2. 生命周期注解

* **@BeforeAll**

  * 在所有测试执行前运行一次（必须 `static`，除非 `@TestInstance(PER_CLASS)`）。
* **@AfterAll**

  * 在所有测试执行后运行一次。
* **@BeforeEach**

  * 每个测试方法前执行。
* **@AfterEach**

  * 每个测试方法后执行。

```java
@BeforeAll
static void initAll() { System.out.println("全局初始化"); }

@BeforeEach
void init() { System.out.println("准备测试数据"); }

@AfterEach
void tearDown() { System.out.println("清理数据"); }

@AfterAll
static void tearDownAll() { System.out.println("全局清理"); }
```

---

## 3. 测试类配置相关

* **@TestClassOrder**

  * 控制测试类执行顺序。

* **@TestMethodOrder**

  * 控制测试方法执行顺序。

  ```java
  @TestMethodOrder(MethodOrderer.OrderAnnotation.class)
  class OrderedTests {
      @Test @Order(1) void testA() {}
      @Test @Order(2) void testB() {}
  }
  ```

* **@TestInstance**

  * 配置生命周期：`PER_CLASS`（同一个实例执行所有测试），`PER_METHOD`（默认，每个测试新建实例）。

* **@DisplayName**

  * 定义测试的可读性名称。

  ```java
  @DisplayName("加法运算测试")
  @Test
  void addTest() { ... }
  ```

* **@DisplayNameGeneration**

  * 定义类内所有测试方法的名称生成规则（如去掉驼峰）。

* **@Nested**

  * 嵌套测试类，方便分组。

  ```java
  @Nested
  class InnerTest {
      @Test void testInside() {}
  }
  ```

---

## 4. 条件执行

* **@Disabled**

  * 禁用测试。
* **@EnabledOnOs / @DisabledOnOs**

  * 根据操作系统启用/禁用。
* **@EnabledOnJre / @DisabledOnJre**

  * 根据 JDK 版本启用/禁用。

---

## 5. 参数化与扩展

* **@ParameterizedClass**

  * 声明整个测试类是参数化类（比较少见）。
* **@BeforeParameterizedClassInvocation / @AfterParameterizedClassInvocation**

  * 在参数化类运行前/后执行。
* **@ClassTemplate**

  * 类级别的测试模板。

---

## 6. 其他增强注解

* **@Tag**

  * 给测试分类打标签，方便分组运行。
* **@AutoClose**

  * 标记的资源会在测试结束后自动关闭。
* **@Timeout**

  * 指定超时时间，超时则失败。
* **@TempDir**

  * 提供临时目录/文件夹。
* **@ExtendWith**

  * 声明式注册扩展。
* **@RegisterExtension**

  * 编程式注册扩展。

---

# JUnit 5 注解总结表

| 注解                                  | 作用                             | 使用场景          |
| ----------------------------------- | ------------------------------ | ------------- |
| @Test                               | 声明测试方法                         | 普通单元测试        |
| @ParameterizedTest                  | 参数化测试                          | 多组输入测试        |
| @RepeatedTest                       | 重复执行测试                         | 压力测试、稳定性      |
| @TestFactory                        | 动态测试工厂                         | 动态生成用例        |
| @TestTemplate                       | 测试模板                           | 框架扩展          |
| @BeforeAll                          | 所有测试前执行一次                      | 全局初始化（DB 连接等） |
| @AfterAll                           | 所有测试后执行一次                      | 全局清理          |
| @BeforeEach                         | 每个测试前执行                        | 准备测试数据        |
| @AfterEach                          | 每个测试后执行                        | 清理数据          |
| @TestClassOrder                     | 控制测试类执行顺序                      | 多类测试有依赖       |
| @TestMethodOrder                    | 控制方法执行顺序                       | 测试步骤有先后       |
| @TestInstance                       | 控制生命周期（PER\_CLASS/PER\_METHOD） | 控制实例化策略       |
| @DisplayName                        | 定义友好名称                         | 生成报告更直观       |
| @DisplayNameGeneration              | 自定义方法名生成规则                     | 一致性命名         |
| @Nested                             | 嵌套测试类                          | 分组测试          |
| @Disabled                           | 禁用测试                           | 临时跳过          |
| @EnabledOnOs / @DisabledOnOs        | 根据 OS 启用/禁用                    | 跨平台兼容         |
| @EnabledOnJre / @DisabledOnJre      | 根据 JDK 版本启用/禁用                 | 多版本兼容         |
| @ParameterizedClass                 | 声明参数化类                         | 高级参数化测试       |
| @BeforeParameterizedClassInvocation | 参数化类运行前执行                      | 参数化生命周期       |
| @AfterParameterizedClassInvocation  | 参数化类运行后执行                      | 参数化生命周期       |
| @ClassTemplate                      | 类级别测试模板                        | 扩展场景          |
| @Tag                                | 给测试打标签                         | 分组执行          |
| @AutoClose                          | 自动关闭资源                         | 自动释放资源        |
| @Timeout                            | 设置超时                           | 避免无限循环        |
| @TempDir                            | 注入临时文件夹                        | 文件 IO 测试      |
| @ExtendWith                         | 注册扩展（声明式）                      | 使用外部扩展        |
| @RegisterExtension                  | 注册扩展（编程式）                      | 自定义扩展逻辑       |

---

好的 👍 我来给你讲解 **Maven 的依赖范围（Dependency Scope）**，这是你写 `pom.xml` 时经常会遇到的关键知识点。

---
# Maven的依赖范围
## 1. 依赖范围（Scope）的作用

Maven 的依赖不仅仅是“有没有”，还要控制 **在哪些阶段** 依赖生效，比如：

* **编译**的时候需要吗？
* **测试**的时候需要吗？
* **打包**时要不要带进去？

Maven 用 `<scope>` 标签来定义这些使用范围。

---

## 2. 常见的依赖范围

### ① `compile`（默认范围）

* **作用**：编译、测试、运行都需要。
* **使用场景**：项目的核心依赖，比如 `spring-core`、`guava`。
* **特点**：打包时会被带上（比如 `.jar` 或 `.war`）。

```xml
<dependency>
  <groupId>com.google.guava</groupId>
  <artifactId>guava</artifactId>
  <version>32.0.0</version>
  <scope>compile</scope>
</dependency>
```

---

### ② `provided`（已提供）

* **作用**：编译和测试需要，但 **运行时不会带上**。
* **使用场景**：依赖由外部容器或 JDK 提供，比如：

  * `servlet-api`（Tomcat 已经有了）
  * `jsp-api`
* **特点**：打包时不会被包含进去。

```xml
<dependency>
  <groupId>javax.servlet</groupId>
  <artifactId>servlet-api</artifactId>
  <version>2.5</version>
  <scope>provided</scope>
</dependency>
```

---

### ③ `runtime`

* **作用**：编译时不需要，但运行和测试需要。
* **使用场景**：典型如 **JDBC 驱动**（编译只需要 `java.sql` 接口，运行才需要 MySQL 驱动）。
* **特点**：打包时会被带上。

```xml
<dependency>
  <groupId>mysql</groupId>
  <artifactId>mysql-connector-java</artifactId>
  <version>8.0.32</version>
  <scope>runtime</scope>
</dependency>
```

---

### ④ `test`

* **作用**：只在测试编译和测试运行时需要。
* **使用场景**：JUnit、Mockito、Spring Test。
* **特点**：打包时不会带上。

```xml
<dependency>
  <groupId>junit</groupId>
  <artifactId>junit</artifactId>
  <version>4.13.2</version>
  <scope>test</scope>
</dependency>
```

---

### ⑤ `system`

* **作用**：和 `provided` 类似，但需要 **手动指定 jar 的路径**。
* **使用场景**：极少用，一般只在公司内部私有 jar 又没有放进 Maven 仓库时才会用。
* **特点**：可移植性差，不推荐。

```xml
<dependency>
  <groupId>com.example</groupId>
  <artifactId>my-lib</artifactId>
  <version>1.0</version>
  <scope>system</scope>
  <systemPath>${project.basedir}/lib/my-lib.jar</systemPath>
</dependency>
```

---

### ⑥ `import`（仅在 `<dependencyManagement>` 中用）

* **作用**：用于引入 **一整套依赖配置**，常用于 **BOM（Bill of Materials）**。
* **使用场景**：Spring Boot 的依赖管理。

```xml
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-dependencies</artifactId>
  <version>3.1.0</version>
  <type>pom</type>
  <scope>import</scope>
</dependency>
```

---

## 3. 总结表格

| 依赖范围（Scope）      | 编译 | 测试 | 运行 | 打包 | 常见场景                     |
| ---------------- | -- | -- | -- | -- | ------------------------ |
| **compile** (默认) | ✔  | ✔  | ✔  | ✔  | 核心依赖（Spring、Guava）       |
| **provided**     | ✔  | ✔  | ✘  | ✘  | 由容器或 JDK 提供（Servlet API） |
| **runtime**      | ✘  | ✔  | ✔  | ✔  | JDBC 驱动、日志实现             |
| **test**         | ✘  | ✔  | ✘  | ✘  | 测试框架（JUnit、Mockito）      |
| **system**       | ✔  | ✔  | ✘  | ✘  | 本地 jar（不推荐）              |
| **import**       | ✘  | ✘  | ✘  | ✘  | BOM 依赖管理                 |

---

# 如何解决Maven中遇到的常见问题
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cf6efea1b7554bd396a2cc6059526334.png)

# 什么是jar包


---

## 1. JAR 包的基本概念

* **JAR** 全称是 **Java ARchive（Java归档文件）**。
* 它本质上就是一个 **压缩文件（ZIP 格式）**，只不过后缀名是 `.jar`。
* 里面通常会包含：

  1. **Java 编译后的 `.class` 文件**（字节码）
  2. **配置文件**（如 `META-INF/MANIFEST.MF`）
  3. **资源文件**（比如图片、XML 配置、属性文件）

👉 你可以把 JAR 包理解为 **Java 的“安装包”或者“工具箱”**，把相关的 Java 类和资源打包到一起，方便复用和分发。

---

## 2. JAR 包的用途

1. **代码复用**：别人写好的工具类打成 JAR，你直接引入就能用。
2. **模块化开发**：项目拆成多个 JAR，分别负责不同的功能模块。
3. **发布运行**：很多 Java 应用就是以一个可执行 JAR 包的形式运行的。

   * 可执行 JAR 里面有 `MANIFEST.MF` 文件，指定了程序的入口点（`Main-Class`）。
   * 执行方式：

     ```bash
     java -jar myapp.jar
     ```

---

## 3. JAR 包的常见分类

1. **普通 JAR**：只包含类库或工具类（不能直接运行）。
2. **可执行 JAR**：有 `main()` 方法，可以直接运行。
3. **依赖 JAR**：作为第三方库使用，比如 `mysql-connector-java.jar`。
4. **fat jar / uber jar**：把项目和所有依赖都打进一个大 JAR，比如 Spring Boot 打包的应用。

---

## 4. 如何生成和使用 JAR 包

* **生成 JAR 包**
  在 Maven 项目中，运行：

  ```bash
  mvn package
  ```

  会在 `target` 目录下生成 `.jar` 文件。

* **使用 JAR 包**
  把 JAR 放到项目的 `classpath` 中，或者在 Maven 的 `pom.xml` 里添加依赖。

---

## 5. 举个例子 🎯

假设你有一个 `utils.jar`，里面有个 `StringUtils` 工具类。
别人只要把 `utils.jar` 加入项目，就能直接用：

```java
import com.example.utils.StringUtils;

public class Test {
    public static void main(String[] args) {
        System.out.println(StringUtils.reverse("Hello")); // 输出 olleH
    }
}
```

---


# 🚀Day 5
---
## 知识要点 📌

# Spring Boot入门


---

## 一、Spring Boot 是什么？

* **Spring 框架**：是 Java 世界里最常用的企业级开发框架，帮我们写 Web 项目、数据库连接等，很方便，但配置比较复杂（XML 配置文件多，容易出错）。
* **Spring Boot**：是 Spring 的升级工具，帮我们把繁琐的配置都自动化了，开发者几乎不用管复杂的 XML 文件，只需要写业务逻辑。
  👉 可以理解成 **“开箱即用”**，适合快速开发 Web 应用和微服务。

\*\*一句话总结：\*\*Spring Boot 就是让你写 Java Web 项目更快、更轻松的框架。

---

## 二、Spring Boot 的特点

1. **自动配置**：不需要写大量配置文件。
2. **内置服务器**：不用再手动安装 Tomcat，直接运行项目就能启动 Web 服务。
3. **开箱即用**：内置了很多常用功能，比如 Web、数据库、消息队列等。
4. **微服务友好**：适合构建分布式系统。

---

## 三、Spring Boot 入门步骤

### 1. 准备环境

* 安装 **JDK 8 或以上**
* 安装 **Maven**（管理依赖）
* 一个 IDE（推荐 IntelliJ IDEA）

### 2. 创建项目

可以通过两种方式：

* 去 [Spring Initializr](https://start.spring.io/) 网站生成项目
* 在 IDE 中选择 **Spring Initializr** 新建项目

选择依赖：

* `Spring Web`（用来写 Web 应用）

---

## 四、第一个 Spring Boot 程序

目录结构大概是这样的：

```
demo
 └─ src
    └─ main
       ├─ java
       │   └─ com.example.demo
       │       ├─ DemoApplication.java   ← 启动类
       │       └─ controller
       │           └─ HelloController.java  ← 控制器
       └─ resources
           ├─ application.properties   ← 配置文件
```

### 1. 启动类（入口）

```java
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication  // 标记这是一个Spring Boot应用
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args); // 启动项目
    }
}
```

### 2. 写一个控制器（Hello World）

```java
package com.example.demo.controller;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController  // 表示这是一个REST接口
public class HelloController {

    @GetMapping("/hello")  // 定义一个接口，访问 http://localhost:8080/hello
    public String sayHello() {
        return "Hello, Spring Boot!";
    }
}
```

### 3. 配置文件（application.properties）

默认可以不写，但我们可以改端口号：

```properties
server.port=8081
```

---

## 五、运行项目

* 直接运行 `DemoApplication.java`
* 浏览器访问：`http://localhost:8081/hello`
* 输出结果：

```
Hello, Spring Boot!
```

---

## 六、总结经验

1. **Spring Boot 把复杂的配置都帮我们做好了**，入门非常快。
2. **启动类 + 控制器** 就能完成一个最简单的 Web 服务。
3. 熟悉了之后，可以逐步学习数据库、前后端交互、REST API、微服务架构等。

---

# 超文本（Hypertext）


---

### 1. 普通文本

普通文本就是我们平时看到的文字，比如一本电子书里的纯文字。它是**线性的**，只能从头到尾读，就像翻书一样。

---

### 2. 超文本的概念

**超文本**是在普通文本的基础上，加入了\*\*链接（Hyperlink）\*\*的概念。

* 你在阅读时，点击某个文字、图片，就能跳转到另一个内容。
* 这些内容可以是别的文字、图片、音频、视频，甚至是另外一份文档。

换句话说，超文本是**非线性的**阅读方式，你不需要按照顺序读，而是可以通过超链接在不同内容之间自由跳转。

---

### 3. 举个例子

* 普通文本：一本纸质书，从第 1 页读到第 100 页。
* 超文本：网页中的一篇文章，里面有很多蓝色的下划线链接，你可以点击直接跳转到相关内容。

比如在 HTML 中：

```html
<p>这是一个 <a href="https://www.wikipedia.org/">超文本链接</a> 示例。</p>
```

点击“超文本链接”，就会跳转到维基百科。

---

### 4. 总结经验

* **超文本的本质**：让信息通过链接关联起来。
* **超文本的优势**：打破线性阅读的限制，更方便地组织和获取信息。
* **应用场景**：网页、电子书、Wiki 知识库、学习文档等等。

👉 也就是说，现在我们用的 **互联网本质上就是一个巨大的超文本系统**（Web = World Wide Web）。

---

# HTTP协议
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f3ca3ec72c474c59855ec31c80c6ea38.png)

## 什么是 HTTP

HTTP（HyperText Transfer Protocol）是用于在客户端（通常是浏览器或其他 HTTP 客户端）和服务器之间**请求-响应**式通信的应用层协议。

* 基本思想：客户端发起请求（Request），服务器返回响应（Response）。
* 运行基于 TCP（传统）或基于 QUIC（HTTP/3）传输。
* 常用端口：HTTP → 80，HTTPS → 443（加密）。

---

## 版本演进（要点）

* **HTTP/0.9**：极简，只支持 GET，单行响应。
* **HTTP/1.0**：引入头部、状态码、Content-Type。连接默认短连接。
* **HTTP/1.1**：常用版本，支持持久连接（Keep-Alive）、分块传输、Host 头、管道化（pipelining，浏览器少用）。
* **HTTP/2**：二进制帧、流与多路复用（同一 TCP 连接多请求并发）、头压缩（HPACK），更高效。
* **HTTP/3**：基于 QUIC（UDP + 用户态加速 + 内建多路复用与连接迁移），更低延迟，解决 TCP/ head-of-line blocking 问题。

---

## HTTP 消息结构（请求/响应）

**请求（Request）** 三部分：

1. 起始行（Request-Line）：`METHOD path HTTP/x.y`
2. 头部（Headers）：若干 `Name: value` 行
3. 空行 + 可选消息体（Body）

示例（GET）：

```
GET /api/users/1 HTTP/1.1
Host: api.example.com
Accept: application/json
User-Agent: curl/8.0
```

**响应（Response）** 三部分：

1. 状态行（Status-Line）：`HTTP/x.y <status-code> <reason-phrase>`
2. 头部（Headers）
3. 空行 + 可选消息体（Body）

示例（200 OK）：

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Content-Length: 27

{"id":1,"name":"Alice"}
```

---

## 常用 HTTP 方法（简表与语义）

| 方法                | 含义                | 是否幂等                    | 常用场景                                       |
| ----------------- | ----------------- | ----------------------- | ------------------------------------------ |
| `GET`             | 读取资源              | 是（不改变服务器状态）             | 获取列表/详情                                    |
| `HEAD`            | 与 GET 相同但不返回 body | 是                       | 获取头（如检测缓存/大小）                              |
| `POST`            | 创建/提交数据           | 否                       | 新建资源、表单提交                                  |
| `PUT`             | 用请求体替换资源          | 是（对同一资源重复 PUT 相同内容相同效果） | 更新整个资源或创建（幂等）                              |
| `PATCH`           | 局部修改资源            | 非幂等/依场景                 | 局部更新                                       |
| `DELETE`          | 删除资源              | 是（对同一资源多次删除结果相同）        | 删除                                         |
| `OPTIONS`         | 查询服务器/资源支持的操作     | 是                       | CORS 预检或功能探测                               |
| `TRACE`/`CONNECT` | 调试/建立隧道           | —                       | CONNECT 用于代理建立 TLS 隧道（HTTPS through proxy） |

> 幂等 (idempotent)：对同一请求重复执行多次，结果相同（不一定不副作用，但最终状态一致）。

---

## 常见状态码（重要的一些）

| 类别        | 常见码                                                             | 含义                |
| --------- | --------------------------------------------------------------- | ----------------- |
| 2xx 成功    | 200 OK                                                          | 请求成功，返回资源/结果      |
|           | 201 Created                                                     | 资源已创建（通常 POST 后）  |
|           | 204 No Content                                                  | 成功但无返回体（删除/更新空响应） |
| 3xx 重定向   | 301 Moved Permanently                                           | 永久重定向             |
|           | 302 Found / 307 / 308                                           | 临时或保留方法重用         |
|           | 304 Not Modified                                                | 缓存未修改（客户端可用缓存）    |
| 4xx 客户端错误 | 400 Bad Request                                                 | 请求格式错误            |
|           | 401 Unauthorized                                                | 未认证（需要登录/凭证）      |
|           | 403 Forbidden                                                   | 已认证但无权限           |
|           | 404 Not Found                                                   | 资源不存在             |
|           | 405 Method Not Allowed                                          | 方法不允许             |
|           | 429 Too Many Requests                                           | 速率限制（限流）          |
| 5xx 服务端错误 | 500 Internal Server Error                                       | 通用服务错误            |
|           | 502 Bad Gateway / 503 Service Unavailable / 504 Gateway Timeout | 代理/服务不可用或超时       |

---

## 头部（Headers）详解（常见分类）

* **通用头（General）**：`Cache-Control`、`Connection`
* **请求头（Request）**：`Host`、`User-Agent`、`Accept`、`Authorization`、`Cookie`、`Accept-Encoding`、`Accept-Language`、`If-Modified-Since`、`If-None-Match`
* **响应头（Response）**：`Server`、`Set-Cookie`、`Location`（重定向）、`WWW-Authenticate`
* **实体头（Entity）**（关于 body）：`Content-Type`、`Content-Length`、`Transfer-Encoding`、`Content-Encoding`、`Content-Language`

重点解释：

* `Host`：HTTP/1.1 必需。用于虚拟主机识别。
* `Content-Type`：指明 body 类型，例如 `application/json; charset=utf-8`、`text/html`、`multipart/form-data`。
* `Content-Length`：字节长度（当有固定长度时）。
* `Transfer-Encoding: chunked`：分块传输，不需要预先知道长度（常见于流或动态生成）。
* `Connection: keep-alive` / `close`：控制连接持久化（HTTP/1.1 默认持久）。
* `Accept-Encoding: gzip, br`：客户端可接收的压缩算法（响应可用 `Content-Encoding` 指示）。
* `Set-Cookie` / `Cookie`：会话和状态管理（详下）。

---

## Cookies / Session / Token

* **Cookie**：服务器通过 `Set-Cookie` 设置；浏览器随后请求会自动带上相应域名/路径的 Cookie。常用于 session id、跟踪。
* **Session（服务器端）**：Cookie（例如 `JSESSIONID`）标记客户端，服务器在内存/存储维护会话数据。
* **Token（无状态）**：如 JWT（JSON Web Token），通常放在 `Authorization: Bearer <token>`。无状态，服务器不保存 session（可横向扩展更好）。

---

## 缓存（Caching）关键头

* `Cache-Control`（最重要，现代用法）：`no-cache`, `no-store`, `public`, `private`, `max-age=3600`
* `Expires`（旧式，HTTP/1.0）
* `ETag`（实体标签，响应唯一标识） + `If-None-Match`（客户端带上以便 304）
* `Last-Modified` + `If-Modified-Since`

**常见缓存流程**：客户端请求→如果有缓存则发送带条件的请求（If-None-Match/If-Modified-Since）→服务器返回 304（未修改）或 200（并返回新资源）。

---

## 内容协商（Content Negotiation）

* 通过请求头 `Accept`, `Accept-Language`, `Accept-Encoding`, `Accept-Charset` 指示客户端偏好。
* 服务器根据这些头选择最佳表示并在 `Content-Type`、`Content-Language` 中返回。
* 常见：JSON vs HTML，压缩与编码（gzip, br）。

---

## 传输编码与分块（Transfer-Encoding: chunked）

* `Transfer-Encoding: chunked` 允许把响应切成多个块发送，适合流式、动态生成内容或不提前计算 Content-Length 的场景。每块前有十六进制长度，末尾是 `0` 块。

---

## HTTPS / TLS（加密层）

* HTTPS = HTTP over TLS。加密、完整性校验、身份验证（证书）。
* TLS 握手建立安全通道，之后应用数据加密传输。
* 要点：为所有网页 API 使用 HTTPS（避免明文传输敏感数据），并启用 HSTS（`Strict-Transport-Security`）防止降级攻击。使用现代 TLS 配置并禁用过时协议。

---

## HTTP 与 REST / API 设计（工程角度）

* **RESTful 风格**：使用 HTTP 方法表达操作（GET=读、POST=创建、PUT=替换、PATCH=部分更新、DELETE=删除）；使用资源 URL（例如 `/api/users/123`）。
* 建议：用合适的状态码、清晰的错误消息体、版本化（如 `/v1/`），并保证幂等性（PUT/DELETE/GET 等）。

常见 API 设计要点：

* 返回一致 JSON 结构（`{ code, message, data }` 或 HTTP 状态直达）
* 支持分页（`page`/`size` 或 `Link` header）
* Rate limiting（限流）与速率反馈（`Retry-After`）
* 并发安全与幂等操作（尤其支付/重要操作）

---

## CORS（跨域资源共享）

* 浏览器的同源策略限制跨域请求。若前端跨域请求后端，后端需返回合适的 CORS 头：

  * `Access-Control-Allow-Origin: https://example.com`（或 `*`）
  * `Access-Control-Allow-Methods: GET, POST, OPTIONS`
  * `Access-Control-Allow-Headers: Content-Type, Authorization`
  * `Access-Control-Allow-Credentials: true`（允许携带 cookie）
* `OPTIONS` 预检请求（preflight）用于判断是否允许跨域。

---

## 常见安全问题与防护

* **中间人/窃听**：用 HTTPS 避免（TLS）。
* **XSS**（跨站脚本）：输出（HTML）必须转义，或使用 CSP（Content-Security-Policy）。
* **CSRF**（跨站请求伪造）：对有状态 cookie 的操作需防御（使用 CSRF Token、SameSite cookie）。
* **HTTP头注入、路径遍历、未验证输入**：严格校验输入/路径、避免直接用用户输入构造文件路径。
* **HSTS、Secure + HttpOnly Cookie、SameSite**：硬化 cookie 和浏览器行为。

---

## 性能优化与工程实践

* **使用缓存（CDN）**：静态资源走 CDN，减服务器压力。
* **Cache-Control 与 ETag**：合理配置，减少不必要下载。
* **开启压缩**：`gzip` 或 `brotli`（`Accept-Encoding`），减少传输大小。
* **使用 HTTP/2 或 HTTP/3**：多路复用、头压缩，减少延迟。
* **连接复用（Keep-Alive）**：减少 TCP 握手成本。
* **避免重定向链**：每个重定向增加延迟。
* **减小 Header 大小与 Cookies**：每次请求都带头部或 cookie，过大影响性能。
* **长连接与短连接权衡**：根据客户端并发和服务器资源选择（HTTP/2 使这问题好很多）。

---

## 常见调试工具与示例

* **curl**：命令行测试 HTTP（最常用）

  ```bash
  # GET
  curl -i https://api.example.com/users/1

  # POST JSON
  curl -i -X POST https://api.example.com/users \
    -H "Content-Type: application/json" \
    -d '{"name":"Alice"}'

  # 带 Header 与认证
  curl -i -H "Authorization: Bearer <token>" https://api.example.com/me
  ```

* **浏览器 DevTools（Network 面板）**：查看请求/响应头、状态码、时间线、请求体/响应体、cookies、CORS 问题。

* **Postman / Insomnia**：交互式 API 调试工具。

* **tcpdump / Wireshark**（调低层）或 **ngrep**。

* **日志**：后端接收到的原始请求头、请求体、响应时间与错误堆栈是定位问题关键。

---

## 示例：完整 GET 请求与响应（raw）

请求：

```
GET /api/books/42 HTTP/1.1
Host: api.example.com
Accept: application/json
User-Agent: curl/8.0
```

响应：

```
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8
Cache-Control: max-age=60
ETag: "abc123"
Content-Length: 45

{"id":42,"title":"HTTP深度解析","author":"Bob"}
```

## 示例：fetch（浏览器）调用 API

```javascript
fetch('https://api.example.com/items', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json', 'Authorization': 'Bearer ' + token },
  body: JSON.stringify({ name: 'item1', qty: 3 }),
  credentials: 'include' // 如果需要带 cookie
})
.then(r => {
  if (!r.ok) throw new Error(r.status);
  return r.json();
})
.then(data => console.log(data))
.catch(err => console.error(err));
```

---

## 调试常见问题与排查建议

* **响应 404**：确认 URL、方法（GET/POST）、Host、路径大小写。
* **401 / 403**：检查认证头（Authorization）、Token 是否过期、CORS 是否阻止凭证。
* **CORS 错误**：看浏览器控制台，检查服务器是否返回 `Access-Control-Allow-*` 头，确认 `Credentials` 与 `Allow-Origin` 配合使用是否正确。
* **慢请求**：用浏览器 Network 面板或 APM（NewRelic、Zipkin、Jaeger）定位是网络、后端处理、DB 还是外部服务。
* **缓存不生效**：查看 `Cache-Control`、`ETag`、`Expires`、`Vary`，确认条件请求（If-None-Match）是否返回 304。
* **错误 502/504**：可能是反向代理与后端通信异常或后端超时。

---

## 最后小结（记忆要点）

1. HTTP 是请求-响应协议，消息 = 起始行 + 头 + 空行 + body。
2. 选用正确的方法（GET/POST/PUT/PATCH/DELETE）、合适状态码、合适头部。
3. 使用 HTTPS（TLS）保护数据与身份。
4. 理解缓存（Cache-Control/ETag）和内容协商（Accept）。
5. HTTP/2/3 优化性能，多路复用、头压缩、QUIC。
6. CORS、CSRF、XSS 是常见安全边界，需配置服务器端头和 cookie 策略。
7. 用 `curl`、浏览器 Network、Postman、日志来调试。

---

# HTTP 协议的请求数据格式


---

## 1. HTTP 请求的基本结构

一次完整的 HTTP 请求分为 **三部分**：

1. **请求行（Request Line）**
2. **请求头（Request Headers）**
3. **请求体（Request Body，可选）**

---

## 2. 请求行（Request Line）

请求行决定了客户端想干什么，格式如下：

```
<请求方法> <请求路径> <协议版本>
```

举例：

```
GET /index.html HTTP/1.1
```

* **请求方法**（Method）：告诉服务器要做的操作

  * 常见方法：

    * `GET`：获取资源
    * `POST`：提交数据
    * `PUT`：更新数据
    * `DELETE`：删除数据
* **请求路径**（Path）：访问的资源地址

  * `/index.html` 表示请求服务器的 `index.html` 页面
* **协议版本**（HTTP Version）：例如 `HTTP/1.1`

---

## 3. 请求头（Request Headers）

请求头是一些 **键值对**，提供额外的说明信息，格式是：

```
Header-Name: value
```

常见的请求头有：

* `Host`：指定访问的主机名和端口（必须有）
* `User-Agent`：说明客户端信息（浏览器/应用）
* `Accept`：告诉服务器希望接收什么类型的数据
* `Content-Type`：说明请求体的数据格式（例如 JSON、表单）
* `Content-Length`：请求体的长度（字节数）

举例：

```
Host: www.example.com
User-Agent: Mozilla/5.0
Accept: text/html,application/json
Content-Type: application/json
```

---

## 4. 请求体（Request Body）

请求体是可选的，主要出现在 **POST、PUT** 这种需要上传数据的请求中。

* **GET 请求**：一般没有请求体，参数写在 URL 里。
* **POST 请求**：有请求体，用来传输数据。

常见的请求体格式：

1. **表单数据**

   ```
   name=Tom&age=18
   ```

   对应的请求头：`Content-Type: application/x-www-form-urlencoded`

2. **JSON 数据**

   ```json
   {
     "name": "Tom",
     "age": 18
   }
   ```

   对应的请求头：`Content-Type: application/json`

---

## 5. 一个完整的 HTTP 请求示例

### GET 请求

```
GET /hello?name=Tom HTTP/1.1
Host: www.example.com
User-Agent: Mozilla/5.0
Accept: text/html
```
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f8484ad3402d4776b73587bec1af2c44.png)

👉 请求体为空

---

### POST 请求（提交 JSON 数据）

```
POST /api/user HTTP/1.1
Host: www.example.com
User-Agent: curl/7.68.0
Content-Type: application/json
Content-Length: 25

{
  "name": "Tom",
  "age": 18
}
```

---

✅ 总结一句话：
**HTTP 请求 = 请求行 + 请求头 + 请求体**

* 请求行：干什么 + 哪个资源 + 用的协议版本
* 请求头：附加说明信息
* 请求体：要传的数据（可选）

---


# HTTP 协议中的请求数据获取
---

## 一、HTTP 请求数据的来源

当我们在浏览器里输入网址、点击按钮、提交表单时，浏览器会给服务器发送一条 **HTTP 请求**。
服务器接收到请求后，就需要**获取请求数据**，比如：

* 你访问的地址（URL）
* 请求方式（GET/POST/PUT/DELETE 等）
* 请求头（Headers，比如浏览器信息、语言、cookie）
* 请求体（Body，通常是表单数据、JSON、文件）

---

## 二、HTTP 请求的数据组成

一个 HTTP 请求主要分 3 部分：

1. **请求行（Request Line）**

   * 格式：`请求方法 请求路径 协议版本`
   * 示例：

     ```
     GET /user?id=1 HTTP/1.1
     POST /login HTTP/1.1
     ```

2. **请求头（Request Headers）**

   * 描述请求的附加信息。
   * 示例：

     ```
     Host: www.example.com
     User-Agent: Mozilla/5.0
     Content-Type: application/json
     ```

3. **请求体（Request Body）**

   * **GET 请求一般没有请求体**，参数放在 URL 里。
   * **POST/PUT 请求常有请求体**，存放提交的数据。
   * 示例（表单数据）：

     ```
     username=jack&password=123456
     ```
   * 示例（JSON 数据）：

     ```json
     {
       "username": "jack",
       "password": "123456"
     }
     ```

---

## 三、如何获取请求数据

这部分要分 **不同的层次** 来理解：

### 1. 在浏览器里

* 地址栏 `?key=value` 叫做 **查询参数**。
* 表单提交的数据，会进入 **请求体**。

### 2. 在抓包工具里（如 Fiddler、Postman、浏览器开发者工具）

你能清楚看到：

* **请求头**
* **请求体**
* **请求方法**
* **URL**

### 3. 在后端代码里（以 Spring Boot 为例）

```java
@RestController
public class UserController {

    // 获取 URL 查询参数 (GET 请求)
    @GetMapping("/user")
    public String getUser(@RequestParam String name, @RequestParam int age) {
        return "name=" + name + ", age=" + age;
    }

    // 获取请求体 JSON 数据 (POST 请求)
    @PostMapping("/login")
    public String login(@RequestBody Map<String, String> user) {
        return "username=" + user.get("username") + ", password=" + user.get("password");
    }

    // 获取请求头
    @GetMapping("/header")
    public String header(@RequestHeader("User-Agent") String userAgent) {
        return "Your browser is: " + userAgent;
    }
}
```

---

## 四、总结

* **HTTP 请求数据** 包含：请求行、请求头、请求体。
* **获取方式**：

  * 浏览器 → 通过 URL、表单。
  * 抓包工具 → 直接查看请求。
  * 服务器 → 通过代码获取（路径参数、查询参数、请求头、请求体）。

---


# HTTP 协议的响应数据格式
---

## 一、HTTP 响应数据的基本格式

```
响应行 (Status Line)
响应头 (Response Headers)
空行
响应体 (Response Body)
```

---

## 二、详细讲解

### 1. **响应行（Status Line）**

响应行包含 3 部分：

```
协议版本 状态码 状态描述
```

✅ 例子：

```
HTTP/1.1 200 OK
```

* **协议版本**：常见的有 `HTTP/1.1`、`HTTP/2`，现在也有 `HTTP/3`。
* **状态码**：告诉客户端请求处理的结果（如成功、失败等）。
* **状态描述**：对状态码的文字说明。

常见状态码：

* **200 OK**：请求成功
* **301 Moved Permanently**：永久重定向
* **302 Found**：临时重定向
* **400 Bad Request**：请求错误（客户端问题）
* **401 Unauthorized**：未授权
* **403 Forbidden**：禁止访问
* **404 Not Found**：资源未找到
* **500 Internal Server Error**：服务器内部错误

---

### 2. **响应头（Response Headers）**

响应头以键值对形式描述服务器和响应体的信息。格式为：

```
Header-Name: Header-Value
```

常见响应头：

* **Content-Type**：响应内容的 MIME 类型

  * `text/html; charset=UTF-8`
  * `application/json`
* **Content-Length**：响应体的字节长度
* **Date**：响应时间
* **Server**：服务器类型（如 Apache、Nginx、Spring Boot 内置 Tomcat）
* **Set-Cookie**：告诉浏览器存储 Cookie
* **Cache-Control**：缓存策略（如 `no-cache`, `max-age=3600`）

---

### 3. **空行**

响应头和响应体之间必须有一个空行，表示头部结束。

---

### 4. **响应体（Response Body）**

* 响应体是实际的数据内容，格式由 `Content-Type` 决定。
* 如果是 `text/html`，返回 HTML 页面；
* 如果是 `application/json`，返回 JSON 数据；
* 如果是文件下载，返回二进制数据流。

✅ 示例：

```http
HTTP/1.1 200 OK
Date: Mon, 01 Sep 2025 11:30:00 GMT
Server: Apache/2.4.41 (Ubuntu)
Content-Type: application/json
Content-Length: 85

{
  "id": 101,
  "name": "Alice",
  "role": "student"
}
```

---

## 三、总结

HTTP 响应的格式分为四个部分：

1. **响应行**：状态码 + 协议版本
2. **响应头**：元数据（类型、长度、服务器信息等）
3. **空行**：分隔头和体
4. **响应体**：真正的返回内容（HTML/JSON/文件等）

这样，客户端（浏览器或其他程序）就能根据响应头和响应体来处理服务器返回的内容。

---


# HTTP 协议的响应数据设置
---

## 一、HTTP 响应的基本格式

HTTP 响应报文由 **三部分**组成：

1. **响应行（Response Line）**

   ```
   HTTP/1.1 200 OK
   ```

   * 协议版本（HTTP/1.1、HTTP/2 等）
   * 状态码（200、404、500…）
   * 状态描述（OK、Not Found、Internal Server Error …）

2. **响应头（Response Headers）**
   描述返回数据的属性，比如数据类型、长度、缓存策略等。
   常见的响应头：

   * `Content-Type: text/html; charset=UTF-8`  → 告诉浏览器返回的内容类型
   * `Content-Length: 512` → 告诉浏览器内容大小
   * `Set-Cookie: sessionId=abc123` → 设置 Cookie
   * `Cache-Control: no-cache` → 不缓存

3. **响应体（Response Body）**
   真正的内容，比如 HTML 页面、JSON 数据、图片二进制流等。

---

## 二、如何在代码里设置 HTTP 响应

在 **Java Web 开发**里，我们常用 `HttpServletResponse` 对象来设置响应。

### 1. 设置状态码

```java
response.setStatus(HttpServletResponse.SC_OK); // 200
response.setStatus(HttpServletResponse.SC_NOT_FOUND); // 404
```

### 2. 设置响应头

```java
response.setHeader("Content-Type", "application/json; charset=UTF-8");
response.setHeader("Cache-Control", "no-cache");
```

### 3. 设置响应体

```java
PrintWriter out = response.getWriter();
out.write("{\"msg\": \"Hello, HTTP!\"}");
out.flush();
out.close();
```

### 4. 设置重定向

```java
response.sendRedirect("https://www.example.com");
```

---

## 三、Spring Boot 中的响应设置

在 Spring Boot 里，我们不用直接操作 `HttpServletResponse`，而是通过 **注解和返回值**来设置响应：

### 示例

```java
@RestController
public class HelloController {

    // 返回 JSON 数据
    @GetMapping("/json")
    public Map<String, String> getJson() {
        Map<String, String> map = new HashMap<>();
        map.put("msg", "Hello, JSON!");
        return map;
    }

    // 返回指定状态码
    @GetMapping("/status")
    public ResponseEntity<String> getStatus() {
        return ResponseEntity
                .status(HttpStatus.CREATED) // 设置 201 状态码
                .header("Custom-Header", "MyValue") // 设置响应头
                .body("Resource Created"); // 设置响应体
    }
}
```

---
## 四、完整示例代码
```java
package com.lele.springbootwebquickstart;

import jakarta.servlet.http.HttpServletResponse;
import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.io.IOException;

@RestController
public class response {
    @RequestMapping("/response1")
    public void response1(HttpServletResponse response) throws IOException {
        response.setStatus(401) ;
        response.setHeader("name","lele");
        response.addHeader("name","lele");
        response.getWriter().write("<h1>hello world</h1>");

    }
    @RequestMapping("/response2")
    public ResponseEntity<String> response2()  {
        return ResponseEntity.status(401).header("name","lele").body("<h1>hello world</h1>");
    }
}

```
✅ 总结：

* HTTP 响应 = **响应行 + 响应头 + 响应体**
* 在 Java EE 里用 `HttpServletResponse` 设置；
* 在 Spring Boot 里用 **返回值 / ResponseEntity** 更优雅。


# SpringBootWeb案例

做一个 **Spring Boot + Vue 前后端分离的 Web 案例**，数据来源是 `user.txt` 文件。我们分成三个部分来写：

1. **后端：Spring Boot 服务端**
2. **前端：Vue 页面**
3. **数据文件：user.txt**

---

## 1. Spring Boot 后端部分

### 1.1 创建工程

* 使用 Spring Initializr 创建 Spring Boot 工程，选择依赖：

  * **Spring Web**
  * **Lombok**

目录结构大致如下：

```
springboot-vue-demo
 ├─ src/main/java/com/example/demo
 │   ├─ DemoApplication.java
 │   ├─ controller
 │   │    └─ UserController.java
 │   ├─ entity
 │   │    └─ User.java
 │   ├─ service
 │   │    └─ UserService.java
 │   └─ util
 │        └─ FileReaderUtil.java
 ├─ src/main/resources
 │   ├─ static  (Vue 打包文件后可放这里，开发时不用)
 │   ├─ user.txt   ← 存放用户数据
 │   └─ application.properties
```

---

### 1.2 数据文件 user.txt

模拟简单数据，格式类似 `id,name,age,email`：

```
1,张三,20,zhangsan@example.com
2,李四,22,lisi@example.com
3,王五,25,wangwu@example.com
```

---

### 1.3 实体类 User.java

```java
package com.example.demo.entity;

import lombok.AllArgsConstructor;
import lombok.Data;
import lombok.NoArgsConstructor;

@Data
@NoArgsConstructor
@AllArgsConstructor
public class User {
    private Integer id;
    private String name;
    private Integer age;
    private String email;
}
```

---

### 1.4 工具类 FileReaderUtil.java

```java
package com.example.demo.util;

import com.example.demo.entity.User;

import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.util.ArrayList;
import java.util.List;

public class FileReaderUtil {
    public static List<User> readUsers(String fileName) {
        List<User> users = new ArrayList<>();
        try (BufferedReader reader = new BufferedReader(
                new InputStreamReader(FileReaderUtil.class.getClassLoader().getResourceAsStream(fileName), "UTF-8"))) {
            String line;
            while ((line = reader.readLine()) != null) {
                String[] arr = line.split(",");
                if (arr.length == 4) {
                    users.add(new User(
                            Integer.parseInt(arr[0]),
                            arr[1],
                            Integer.parseInt(arr[2]),
                            arr[3]
                    ));
                }
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
        return users;
    }
}
```

---

### 1.5 Service 层 UserService.java

```java
package com.example.demo.service;

import com.example.demo.entity.User;
import com.example.demo.util.FileReaderUtil;
import org.springframework.stereotype.Service;

import java.util.List;

@Service
public class UserService {
    public List<User> getAllUsers() {
        return FileReaderUtil.readUsers("user.txt");
    }
}
```

---

### 1.6 控制层 UserController.java

```java
package com.example.demo.controller;

import com.example.demo.entity.User;
import com.example.demo.service.UserService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.web.bind.annotation.*;

import java.util.List;

@CrossOrigin // 解决跨域问题
@RestController
@RequestMapping("/api/users")
public class UserController {

    @Autowired
    private UserService userService;

    @GetMapping
    public List<User> getUsers() {
        return userService.getAllUsers();
    }
}
```

---

### 1.7 application.properties

```properties
server.port=8080
```

---

## 2. Vue 前端部分

你可以使用 Vue CLI 创建一个项目，或者在 `vite` 项目中写。
我给你一个最简单的 Vue3 + Axios 示例。

### 2.1 安装依赖

```bash
npm install axios
```

### 2.2 App.vue

```vue
<template>
  <div>
    <h1>用户列表</h1>
    <table border="1">
      <tr>
        <th>ID</th><th>姓名</th><th>年龄</th><th>Email</th>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.age }}</td>
        <td>{{ user.email }}</td>
      </tr>
    </table>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import axios from 'axios'

const users = ref([])

onMounted(() => {
  axios.get('http://localhost:8080/api/users')
    .then(res => {
      users.value = res.data
    })
    .catch(err => console.error(err))
})
</script>
```

---

## 3. 运行步骤

1. 启动 Spring Boot 项目，后端接口 `http://localhost:8080/api/users` 可返回 JSON 数据。
2. 启动 Vue 前端，访问 `http://localhost:5173`（vite 默认端口）。
3. 页面展示 `user.txt` 中的数据。

---

好的，我用通俗的语言来给你讲解一下 **三层架构**（Three-tier Architecture），这是做后端开发（比如 Spring Boot 项目）经常会用到的一种设计模式。

---
# 三层架构
## 🔑 三层架构包含三个层次：

1. **表示层（Presentation Layer，也叫 UI 层 / 控制层）**
2. **业务逻辑层（Business Logic Layer，简称 Service 层）**
3. **数据访问层（Data Access Layer，简称 DAO 层 / Repository 层）**

---

### 1. 表示层（Controller 层）

* **作用**：负责接收客户端的请求（比如浏览器、Vue 前端发过来的 HTTP 请求），然后把请求转交给业务层处理；业务处理完再把结果返回给客户端。
* **类比**：相当于餐厅的**服务员**，点单（接收请求）、把单子交给厨师（业务层），再把菜端给顾客（返回响应）。
* **在 Spring Boot 里**：就是 `@Controller` 或 `@RestController`。

示例：

```java
@RestController
@RequestMapping("/user")
public class UserController {
    @Autowired
    private UserService userService;

    @GetMapping("/{id}")
    public User getUser(@PathVariable Long id) {
        return userService.findUserById(id);
    }
}
```

---

### 2. 业务逻辑层（Service 层）

* **作用**：处理具体的业务逻辑，比如注册用户需要：检查用户名是否重复、加密密码、保存到数据库。
* **类比**：相当于餐厅的**厨师**，真正把点单变成菜。
* **在 Spring Boot 里**：通常用 `@Service` 标注。

示例：

```java
@Service
public class UserService {
    @Autowired
    private UserRepository userRepository;

    public User findUserById(Long id) {
        return userRepository.findById(id).orElse(null);
    }
}
```

---

### 3. 数据访问层（DAO/Repository 层）

* **作用**：直接和数据库打交道，执行 SQL 查询、插入、更新、删除。
* **类比**：相当于**仓库管理员**，厨师（Service 层）要食材，就来仓库拿。
* **在 Spring Boot 里**：通常是 `@Repository`，或者直接用 Spring Data JPA 的接口。

示例：

```java
@Repository
public interface UserRepository extends JpaRepository<User, Long> {
    // JpaRepository 已经帮我们封装好了常见的增删改查
}
```

---

## 🏗 三层架构的好处

1. **职责清晰**：控制层负责接收请求，业务层负责处理逻辑，数据层负责数据库操作，不会混乱。
2. **易于维护**：比如数据库变了，只要改 DAO 层，Controller 和 Service 不用动。
3. **可扩展性强**：后期要换前端（Vue → React）、数据库（MySQL → PostgreSQL），改动较小。
4. **解耦合**：不同层之间通过接口交互，互相独立。

---

总结一下：
👉 **Controller** 接收请求 → **Service** 处理逻辑 → **Repository/DAO** 访问数据库 → 结果返回给 Controller → 返回前端。

---
# 简单三层架构项目
我们按照 **三层架构** 来分：

* **Controller 层（表现层）**：接收前端请求，返回数据。
* **Service 层（业务逻辑层）**：处理业务逻辑。
* **DAO 层（数据访问层/持久层）**：操作数据库。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5f51e656cfb74dc69f40f790c12a9be3.png)

数据库用 MySQL 举例。

---

## 1. 前端 Vue 页面 (简单 HTML)

前端通过 Vue 发送请求，展示用户列表。

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>用户管理</title>
  <script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
  <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
</head>
<body>
<div id="app">
  <h2>用户列表</h2>
  <ul>
    <li v-for="user in users" :key="user.id">
      {{ user.id }} - {{ user.name }} - {{ user.email }}
    </li>
  </ul>
  <h2>添加用户</h2>
  <input v-model="newUser.name" placeholder="姓名">
  <input v-model="newUser.email" placeholder="邮箱">
  <button @click="addUser">添加</button>
</div>

<script>
new Vue({
  el: '#app',
  data: {
    users: [],
    newUser: { name: '', email: '' }
  },
  created() {
    this.fetchUsers();
  },
  methods: {
    fetchUsers() {
      axios.get("http://localhost:8080/users")
           .then(res => { this.users = res.data; });
    },
    addUser() {
      axios.post("http://localhost:8080/users", this.newUser)
           .then(() => {
             this.fetchUsers();
             this.newUser = { name: '', email: '' };
           });
    }
  }
});
</script>
</body>
</html>
```

---

## 2. 后端 Spring Boot 项目

假设我们用 Maven，新建一个 Spring Boot 项目。

### (1) pom.xml 依赖

```xml
<dependencies>
    <!-- Web -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <!-- MyBatis 或 JPA，这里用 JPA -->
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-data-jpa</artifactId>
    </dependency>

    <!-- MySQL 驱动 -->
    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <scope>runtime</scope>
    </dependency>

    <!-- lombok (简化 getter/setter) -->
    <dependency>
        <groupId>org.projectlombok</groupId>
        <artifactId>lombok</artifactId>
        <optional>true</optional>
    </dependency>
</dependencies>
```

### (2) application.properties

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/demo?useSSL=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=123456
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### (3) 实体类 (User.java)

```java
import jakarta.persistence.*;
import lombok.Data;

@Entity
@Table(name = "users")
@Data
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String name;
    private String email;
}
```

### (4) DAO 层 (UserRepository.java)

```java
import org.springframework.data.jpa.repository.JpaRepository;

public interface UserRepository extends JpaRepository<User, Long> {
}
```

### (5) Service 层 (UserService.java)

```java
import java.util.List;

public interface UserService {
    List<User> findAll();
    User save(User user);
}
```

实现类：

```java
import org.springframework.stereotype.Service;
import java.util.List;

@Service
public class UserServiceImpl implements UserService {
    private final UserRepository userRepository;

    public UserServiceImpl(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    @Override
    public List<User> findAll() {
        return userRepository.findAll();
    }

    @Override
    public User save(User user) {
        return userRepository.save(user);
    }
}
```

### (6) Controller 层 (UserController.java)

```java
import org.springframework.web.bind.annotation.*;
import java.util.List;

@RestController
@RequestMapping("/users")
@CrossOrigin // 允许前端跨域请求
public class UserController {
    private final UserService userService;

    public UserController(UserService userService) {
        this.userService = userService;
    }

    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }

    @PostMapping
    public User addUser(@RequestBody User user) {
        return userService.save(user);
    }
}
```

---

## 3. 数据库准备

MySQL 创建一个数据库：

```sql
CREATE DATABASE demo;
```

启动项目后，JPA 会自动建表。

---

✅ 到这里，完整的三层架构小项目就好了：

* 前端 Vue（静态 HTML） → axios 请求 →
* Spring Boot Controller → Service → DAO → MySQL

---
# 分层解耦思想

---

### 1. 什么是“分层解耦”？

* **分层**：把系统分成不同的层次，每一层只做自己该做的事。
* **解耦**：减少层与层之间的依赖关系，避免“牵一发而动全身”。

这样做的目的：
✅ 代码更清晰
✅ 功能更独立
✅ 方便测试和维护
✅ 以后要改功能或换技术时，影响范围更小
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0940f38835d943629aaad24a18ba3753.png)

---

### 2. Spring 常见的分层结构

在 Spring Boot 项目里，最常见的是 **三层架构**（有时候会加一层 Repository）：

1. **Controller 层（表现层）**

   * 负责接收请求、返回响应。
   * 不处理业务逻辑，只是“入口”。
   * 例如：接收用户请求 `/user/login`，把用户名和密码传给 Service。

2. **Service 层（业务层）**

   * 负责业务逻辑处理。
   * 可以调用多个 Repository 层方法，完成一个业务流程。
   * 例如：登录时，先查数据库 → 校验密码 → 生成 Token → 返回结果。

3. **Repository/DAO 层（数据访问层）**

   * 专门负责和数据库打交道。
   * 不写业务逻辑，只做 CRUD（增删改查）。
   * 例如：`findUserByUsername("tom")`，返回用户对象。

---

### 3. Spring 如何实现“解耦”？

Spring 的核心是 **IOC（控制反转）和 DI（依赖注入）**，这就是解耦的关键。

* **传统方式（强耦合）**

  ```java
  UserService service = new UserServiceImpl();
  ```

  直接 `new`，写死了依赖，Service 一旦改，Controller 也得改。

* **Spring 方式（解耦）**

  ```java
  @RestController
  public class UserController {
      @Autowired
      private UserService userService;
  }
  ```

  * 这里 `UserController` 不关心 `UserService` 的具体实现，Spring 会自动注入。
  * 如果以后换 `UserServiceImpl2`，只要在配置里改，不需要动 Controller。

这样，每一层只依赖接口，而不依赖具体实现，耦合度就降低了。

---

### 4. 分层解耦的好处

1. **职责清晰**：Controller 不写业务逻辑，Service 不直接写 SQL。
2. **方便扩展**：要改数据库，从 MySQL 换成 MongoDB，只改 Repository 层即可。
3. **便于测试**：写单元测试时，可以用“假数据实现”替代真实数据库，不影响业务逻辑。
4. **降低风险**：某一层的变化不会影响到整个系统。

---

📌 总结一句话：
Spring 的分层解耦思想就是 **“一层只管一层的事，通过接口和依赖注入来隔离上下层”**。

---
# Spring 框架中的控制反转（IoC）、依赖注入（DI）、Bean对象
---


## 1. 控制反转（IoC, Inversion of Control）

👉 **核心思想**：把对象的创建权、依赖关系的管理权，从程序员手里“反转”交给 Spring 容器。

### 举个例子：

* **没有 IoC 的情况**
  你要炒菜（业务逻辑），还得自己去市场买菜（new 对象）、洗菜（初始化依赖），很麻烦。

```java
public class UserService {
    private UserRepository userRepository = new UserRepository(); // 自己创建依赖
}
```

* **有 IoC 的情况**
  你只管炒菜（写逻辑），至于食材（对象）的买、洗、切，都由“管家”（Spring 容器）来准备好，然后直接给你用。

```java
public class UserService {
    private UserRepository userRepository; // 不用自己 new
}
```

📌 **总结一句话**：IoC = 对象的控制权交给了 Spring。

---

## 2. 依赖注入（DI, Dependency Injection）

👉 IoC 是个大思想，而 **DI 是 IoC 的具体实现方式**。
就是说：对象需要什么（依赖），Spring 就把什么 **注入（传进来）**。

### 三种常见注入方式：

1. **构造器注入**

```java
@Service
public class UserService {
    private final UserRepository userRepository;

    // Spring 自动把 UserRepository 注入进来
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

2. **Setter 注入**

```java
@Service
public class UserService {
    private UserRepository userRepository;

    @Autowired
    public void setUserRepository(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

3. **字段注入（不推荐，常用于快速写 Demo）**

```java
@Service
public class UserService {
    @Autowired
    private UserRepository userRepository;
}
```

📌 **总结一句话**：DI = Spring 容器把需要的对象“注入”给类，而不是让类自己去创建。

---

## 3. Bean 对象

👉 **Bean** = 被 Spring 容器管理的对象。
只要一个类交给 Spring 管理，它在容器里的实例就叫 Bean。

### 定义 Bean 的方式：

1. **注解方式**（最常见）

```java
@Component  // 或者 @Service, @Repository, @Controller
public class UserService { }
```

2. **配置类方式**

```java
@Configuration
public class AppConfig {
    @Bean
    public UserService userService() {
        return new UserService();
    }
}
```

3. **XML 配置方式**（现在基本少用）

```xml
<bean id="userService" class="com.example.UserService"/>
```

### Bean 的生命周期（简单理解版）：

* 容器启动时：Spring 创建 Bean（new 对象）
* 容器运行时：Spring 注入依赖、调用初始化方法
* 容器关闭时：Spring 销毁 Bean

📌 **总结一句话**：Bean = Spring 容器中的“食材”，随时可以被拿来用。

---

## 4. 三者关系总结

* **IoC（控制反转）**：对象不再自己 new，交给 Spring 容器来管理。
* **DI（依赖注入）**：Spring 把对象之间的依赖关系注入好。
* **Bean**：Spring 容器里被托管的对象。

👉 打个比方：

* Spring 就像一个“外卖平台”
* Bean 就是“各种菜品”
* DI 就是“把菜送到你家餐桌”
* IoC 就是“你不用再下厨房了，一切交给外卖平台管”。

---

# `@Component`

---

## 1. `@Component` 是什么

* 它的作用就是：**把一个类标记为 Spring 容器中的 Bean**。
* 当 Spring 启动时，会自动扫描（通过 `@ComponentScan`）带有 `@Component` 注解的类，并把它们交给 IoC 容器管理。

简单理解：
👉 你写个普通类，本来要自己 `new` 对象，现在只要加个 `@Component`，Spring 就会帮你去创建并管理这个对象。

---

## 2. 使用 `@Component` 的例子

```java
import org.springframework.stereotype.Component;

@Component  // 把这个类交给 Spring 容器管理
public class UserService {
    public void sayHello() {
        System.out.println("Hello from UserService!");
    }
}
```

然后在别的类里就可以直接 **依赖注入** 了：

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;

@Component
public class UserController {

    @Autowired   // 自动注入 UserService
    private UserService userService;

    public void doSomething() {
        userService.sayHello(); // 不需要 new UserService()
    }
}
```

---

## 3. `@Component` 的几个衍生注解

其实 `@Component` 是一个 **泛化注解**，Spring 为了更语义化，又提供了几个专门的：

* `@Service` —— 用在 **业务层**（Service 层类）
* `@Repository` —— 用在 **数据访问层**（DAO 层类）
* `@Controller` —— 用在 **控制层**（Web 控制器类）

它们本质上和 `@Component` 一样，都是把类交给 Spring 管理，只是为了代码更清晰。

---

## 4. 总结

* **控制反转（IoC）**：对象的创建不由你自己 `new`，而是由容器（Spring）来管理。
* **依赖注入（DI）**：当一个类需要另一个类时，不用手动去 `new`，Spring 会自动把对应的 Bean 注入进来。
* **`@Component`**：用来标记一个类，让 Spring 容器管理它。

---

# 代码具体实现

---

## 1. 没有 IoC/DI 的传统写法（硬编码依赖）

```java
class UserService {
    private UserRepository userRepository = new UserRepository(); // 手动创建依赖

    public void saveUser(String name) {
        userRepository.save(name);
    }
}

class UserRepository {
    public void save(String name) {
        System.out.println("保存用户: " + name);
    }
}

public class Main {
    public static void main(String[] args) {
        UserService userService = new UserService(); // 直接 new
        userService.saveUser("张三");
    }
}
```

👉 问题：

* `UserService` 强耦合 `UserRepository`，想换成 `MySQLRepository` 或 `MongoRepository` 就很麻烦。
* 程序员要自己 `new` 对象，扩展性差。

---

## 2. 使用 **IoC + DI**（由 Spring 管理 Bean）

Spring 会帮我们**创建对象（Bean）**并把依赖**注入**进去。

### （1）定义依赖关系

```java
import org.springframework.stereotype.Repository;
import org.springframework.stereotype.Service;

// 数据访问层
@Repository
class UserRepository {
    public void save(String name) {
        System.out.println("保存用户: " + name);
    }
}

// 业务层
@Service
class UserService {
    private final UserRepository userRepository;

    // 构造方法注入（推荐）
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    public void saveUser(String name) {
        userRepository.save(name);
    }
}
```

### （2）Spring Boot 主程序

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.ApplicationContext;

@SpringBootApplication
public class DemoApplication {
    public static void main(String[] args) {
        ApplicationContext context = SpringApplication.run(DemoApplication.class, args);

        // 从 Spring 容器获取 Bean，而不是自己 new
        UserService userService = context.getBean(UserService.class);
        userService.saveUser("李四");
    }
}
```

👉 关键点：

* `@Service`、`@Repository` → 把类交给 Spring 容器管理。
* 构造函数参数 `UserRepository` → Spring 自动注入（DI）。
* `context.getBean(UserService.class)` → 从容器拿对象。

---

## 3. IoC 和 DI 的关系

* **IoC（控制反转）**：对象的创建和依赖关系的管理由 **Spring 容器**负责，而不是由我们 `new`。
* **DI（依赖注入）**：容器在创建对象时，把它需要的依赖 **自动注入**（构造方法、Setter、字段）。

一句话总结：
👉 **IoC 是思想**，Spring 容器帮你管对象；
👉 **DI 是实现方式**，Spring 用注入来解决依赖。

---
# IoC 和 DI 详解

IoC（Inversion of Control，控制反转）和 DI（Dependency Injection，依赖注入）是软件开发中重要的设计原则和模式，尤其在面向对象编程（如 Java 的 Spring 框架）中广泛应用。它们旨在降低代码耦合度，提高可维护性和可测试性。下面我将从定义、关系、原理、优点、实现方式和示例等方面进行详细讲解。

---

## 1. **IoC（控制反转）的概念**
IoC 是软件设计的一种思想，它将对象的创建、生命周期管理和依赖关系的控制权从程序代码中转移到外部容器或框架中。传统编程中，代码直接控制对象的创建和依赖（如通过 `new` 关键字创建实例），这会导致高耦合。IoC 则“反转”了这种控制，让容器负责这些工作。

### **核心思想**
- **传统控制**：代码主动创建和管理对象（例如：`ClassA a = new ClassA();`）。
- **控制反转**：容器（如 Spring 的 IoC 容器）被动注入对象，代码只需声明依赖。
- IoC 强调“不要调用我们，我们会调用你”（好莱坞原则）。

### **IoC 的类型**
IoC 不是一个具体技术，而是范式，主要通过 DI 来实现（详见下文）。其他形式包括依赖查找（Dependency Lookup），但 DI 更常见。

---

## 2. **DI（依赖注入）的概念**
DI 是 IoC 的具体实现方式之一。它是指容器在运行时自动将对象的依赖（其他对象或资源）注入到目标对象中，而不是由目标对象自己创建依赖。

### **核心思想**
- **依赖**：一个对象需要另一个对象来完成工作（如 Service 需要 DAO）。
- **注入**：容器负责提供这些依赖，而不是手动编码。
- DI 解决了传统代码中“硬编码”依赖的问题，提高了灵活性。

### **DI 的注入方式**
DI 有三种常见注入方式：
1. **构造器注入（Constructor Injection）**：
   - 通过对象的构造方法注入依赖。
   - 优点：强制依赖，确保对象创建时依赖已就绪；适合不可变依赖。
   - 示例：在 Spring 中，通过 `<constructor-arg>` 或注解 `@Autowired` 在构造器上。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/07aee63c9eb545a394d70f044189127c.png)

2. **Setter 方法注入（Setter Injection）**：
   - 通过 Setter 方法注入依赖。
   - 优点：灵活，可选依赖；支持运行时修改。
   - 缺点：可能导致对象不完整（依赖未注入）。
   - 示例：在 Spring 中，通过 `<property>` 或 `@Autowired` 在 Setter 上。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d673f81b42e34582b5d000fc5e9f3df0.png)

3. **接口注入（Interface Injection）**：
   - 通过接口定义注入方法，较少使用，因为侵入性强。
   - 示例：对象实现一个接口，容器调用接口方法注入依赖。

在现代框架中，还支持字段注入（Field Injection，使用 `@Autowired` 直接在字段上），但不推荐，因为它隐藏了依赖，影响测试。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/44a3633f208c4ec9b70dd900920fbf33.png)

---

## 3. **IoC 和 DI 的关系**
- **IoC 是目标，DI 是手段**：IoC 是一种设计原则，DI 是实现 IoC 的最常见方式。简单说，DI 是 IoC 的子集。
- **为什么关联**：IoC 通过 DI 来反转控制——容器注入依赖，而不是代码自己管理。
- **其他实现 IoC 的方式**：如服务定位器（Service Locator）模式，但 DI 更被动、更解耦。

如果没有 DI，IoC 就难以实现；反之，DI 体现了 IoC 的精髓。

---

## 4. **IoC 和 DI 的优点**
1. **降低耦合**：对象不直接依赖具体实现，而是依赖抽象接口，便于替换实现类。
2. **提高可测试性**：易于 mock 依赖，进行单元测试。
3. **提升可维护性**：代码更模块化，修改一个类不影响其他类。
4. **支持配置化**：通过 XML、注解或 Java 配置外部化依赖，便于环境切换（如开发/生产）。
5. **促进复用**：容器管理单例/原型等作用域，优化资源使用。

### **缺点**
- 学习曲线陡峭：初学者需理解容器机制。
- 性能开销：容器初始化和注入有轻微 overhead。
- 过度使用可能导致“魔法”代码，调试困难。

---

## 5. **IoC 和 DI 的实现原理**
以 Spring 框架为例（最典型的应用）：
- **IoC 容器**：如 `ApplicationContext`，负责 Bean（对象）的创建、管理和销毁。
  - Bean 定义：通过 XML（`<bean>`）、注解（`@Component`、`@Service` 等）或 Java 配置（`@Configuration`）。
  - 生命周期：初始化（init-method）、使用、销毁（destroy-method）。
- **DI 过程**：
  1. 扫描 Bean 定义。
  2. 创建 Bean 实例。
  3. 注入依赖（autowire by type/name）。
  4. 处理 AOP（切面）等扩展。

其他框架如 Google Guice、.NET 的 Autofac 也类似实现。

---

## 6. **示例讲解**
假设一个简单的 Java 应用：UserService 依赖 UserDao。

#### **传统方式（无 IoC/DI）**
```java
public class UserDao {
    public void getUser() { System.out.println("Getting user from DB"); }
}

public class UserService {
    private UserDao userDao = new UserDao();  // 硬编码依赖
    public void findUser() { userDao.getUser(); }
}
```
- 问题：UserService 紧耦合 UserDao，无法轻松替换 mock。

### **使用 DI（Spring 示例）**
1. **定义 Bean**：
   ```java
   @Repository
   public class UserDao {
       public void getUser() { System.out.println("Getting user from DB"); }
   }

   @Service
   public class UserService {
       private final UserDao userDao;

       @Autowired  // 构造器注入
       public UserService(UserDao userDao) {
           this.userDao = userDao;
       }

       public void findUser() { userDao.getUser(); }
   }
   ```

2. **配置**：
   - 使用注解扫描：`@ComponentScan`。
   - 启动容器：`ApplicationContext context = new AnnotationConfigApplicationContext(Config.class);`。
   - 获取 Bean：`UserService service = context.getBean(UserService.class); service.findUser();`。

- 优点：UserService 只声明依赖，Spring 容器自动注入。测试时可注入 mock UserDao。

---

## 7. **常见应用场景**
- **企业级应用**：Spring Boot 使用 IoC/DI 管理控制器、服务、仓库。
- **微服务**：通过 DI 注入远程服务客户端。
- **测试框架**：如 JUnit 与 Spring Test 结合，注入 mock。
- **其他语言**：Python 的 Dependency Injector、C# 的 ASP.NET Core 内置 DI。

---

## 8. **总结与注意事项**
IoC 和 DI 是现代软件架构的核心，帮助构建松耦合、高可扩展的系统。IoC 提供控制反转的理念，DI 则是其实际落地。掌握它们，能显著提升代码质量。在实际开发中，优先使用构造器注入，避免循环依赖（通过 Setter 或懒加载解决）。


---
# `@ComponentScan`
---
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cf59cdc4ebee455b8f715fd18f358c56.png)

## 1. `@ComponentScan` 的作用

* 它的主要作用是：
  **告诉 Spring 在哪里去找标注了组件注解（`@Component`、`@Service`、`@Repository`、`@Controller`）的类，并把它们注册到 IoC 容器里。**

简单来说：
👉 你写了一个类，并在上面加了 `@Component`，Spring 并不会自动认识它。
👉 只有配置了 `@ComponentScan`，Spring 才会去扫描这个类，并把它交给容器管理。

---

## 2. 常见用法

```java
@Configuration  // 表示这是一个配置类（类似以前的 XML 配置）
@ComponentScan(basePackages = "com.example.project")  
public class AppConfig {
}
```

这里 `basePackages = "com.example.project"` 表示：

* Spring 会从 `com.example.project` 包开始，往下递归扫描所有类，
* 找出带有 `@Component`、`@Service`、`@Repository`、`@Controller` 的类，
* 把它们自动注册成 Spring Bean。

如果不写 `basePackages`，默认会扫描 **当前配置类所在包及其子包**。

---

## 3. 和 `@Component` 的关系

* `@Component`：标记某个类是一个 Bean（需要交给 IoC 容器管理）。
* `@ComponentScan`：告诉 Spring 去哪里找这些 `@Component`。

没有 `@ComponentScan`，Spring 不会自动去找 Bean；
有了 `@ComponentScan`，Spring 就能批量发现并加载这些 Bean。

---

## 4. 高级用法

### 4.1 扫描多个包

```java
@ComponentScan(basePackages = {"com.example.service", "com.example.dao"})
```

### 4.2 使用 `excludeFilters` 排除

```java
@ComponentScan(
    basePackages = "com.example",
    excludeFilters = @ComponentScan.Filter(
        type = FilterType.ANNOTATION, 
        classes = {Controller.class}  // 排除 @Controller 标记的类
    )
)
```

### 4.3 使用 `includeFilters` 精准控制

```java
@ComponentScan(
    basePackages = "com.example",
    includeFilters = @ComponentScan.Filter(
        type = FilterType.ANNOTATION, 
        classes = {Service.class} // 只扫描 @Service
    ),
    useDefaultFilters = false // 禁止默认扫描
)
```

---

## 5. 总结（直白一点）

* `@Component` → 给某个类贴上标签，告诉 Spring：这个类是 Bean。
* `@ComponentScan` → 告诉 Spring 去哪里找这些有标签的类。
* 两者配合：就能实现 Bean 的自动发现和 IoC 容器注册。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c183217116064fc98a136f93bd43da8e.png)

---


# 三种注入方式的对比分析
我们来对比一下 **属性注入、Setter 注入、构造器注入** 的优缺点，我整理成一个表格，帮你直观理解👇

| 注入方式                       | 概念                              | 优点                                                                                       | 缺点                                                                      | 使用场景                             |
| -------------------------- | ------------------------------- | ---------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | -------------------------------- |
| **属性注入** (Field Injection) | 通过 `@Autowired` 等注解直接在类的字段上注入依赖 | - 代码简洁，省去了 getter/setter<br>- 使用方便，常见于快速开发                                               | - 违反面向对象封装（字段直接暴露给容器）<br>- 不利于单元测试（不能方便地通过构造参数传入 mock 对象）<br>- 类和容器耦合度高 | 原型开发、Demo、快速实现时使用，但不推荐在正式项目中大量使用 |
| **Setter 注入**              | 通过 `setXxx()` 方法注入依赖            | - 可选依赖更灵活（某些依赖可以不注入）<br>- 符合 JavaBean 规范<br>- 容易扩展（后续可以修改依赖）                             | - 对象创建后，可能存在依赖未完全注入的情况<br>- 依赖关系不够明确（必须先看 setter 才知道依赖什么）               | 适用于依赖不是强制的情况，或者某些依赖可能后期需要动态替换    |
| **构造器注入**                  | 通过构造函数参数传入依赖                    | - 强制依赖注入（必须传入才能创建对象）<br>- 保证对象创建时依赖完整<br>- 有利于单元测试（可直接传 mock 对象）<br>- 更符合 **不可变对象** 设计理念 | - 当依赖过多时，构造函数参数会很长（可读性下降）<br>- 某些可选依赖不好处理                               | 推荐的最佳实践，尤其是依赖较多但必须完整注入的核心业务类     |

👉 总结：

* **构造器注入** 是官方和业界推荐的最佳实践（强依赖时用它）。
* **Setter 注入** 适合依赖可选、需要灵活替换的情况。
* **属性注入** 简单，但违背面向对象设计原则，一般只在特殊情况下用（如框架代码或 Demo）。

---
# Spring 容器中如果存在多个相同类型的 Bean
在 **Spring 容器中如果存在多个相同类型的 Bean**，那么在注入时就可能会出现歧义 —— Spring 不知道该注入哪一个。

为了解决这个问题，Spring 提供了几种常用的办法：

---

## 解决方案对比表

| 方法                      | 用法示例                                                                                        | 优点                     | 缺点                         | 使用场景                 |
| ----------------------- | ------------------------------------------------------------------------------------------- | ---------------------- | -------------------------- | -------------------- |
| **@Primary**            | `java  @Bean @Primary public UserService userService1() { return new UserServiceImpl1(); }` | 默认优先注入，不需要修改太多代码       | 只能有一个主 Bean，扩展性有限          | 有一个常用的默认实现，其他实现是备用的  |
| **@Qualifier**          | `java  @Autowired  @Qualifier("userService2")  private UserService userService;`            | 精确指定 Bean 名称，避免歧义      | 每次注入都要写明 Bean 名称，代码稍啰嗦     | 一个接口有多个实现，需要精确控制使用哪个 |
| **@Resource** (JSR-250) | `java  @Resource(name="userService2")  private UserService userService;`                    | 按名称注入，直观，兼容 Java EE 标准 | 灵活性比 Spring 的 @Qualifier 弱 | 和旧项目、Java EE 规范兼容    |
| **注入 List / Map**       | `java  @Autowired  private List<UserService> services; `                                    | 一次性注入所有同类型 Bean，方便批量处理 | 需要自己在代码里区分和选择              | 需要同时使用多个实现，做聚合或批处理   |
| **条件注入 @Conditional**   | `java  @Bean  @ConditionalOnProperty("use.impl1")  public UserService userService1() {...}` | 根据环境/配置选择实现，灵活         | 配置较复杂                      | 多环境切换（如开发、测试、生产）     |

---
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2c4597a913f94e2f86decd6b3d84d53b.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4d1f44e2579c47369b775d84cd63f0e6.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a6b2f15579db48ff97c9a8bc130089ef.png)

### 推荐思路：

* 如果 **只是一个默认实现**：用 `@Primary`。
* 如果 **需要明确区分**：用 `@Qualifier` 或 `@Resource`。
* 如果 **多个实现都要用**：直接注入 `List<UserService>` 或 `Map<String, UserService>`。
* 如果 **要根据环境动态切换**：用 `@Conditional` 或配置文件结合。

---
# @Resource与@autowired的区别
这个问题非常经典，也是 Spring 面试常考点 👍。我们来一步步讲解 **`@Resource` 和 `@Autowired` 的区别**，用通俗的方式帮你记牢。

---

## 1. 所属规范不同

* **`@Autowired`**

  * 来自 **Spring 框架**（`org.springframework.beans.factory.annotation.Autowired`）。
  * 是 Spring 特有的注解。

* **`@Resource`**

  * 来自 **JDK 的 JSR-250 规范**（`javax.annotation.Resource` 或 `jakarta.annotation.Resource`）。
  * 是 Java 标准的一部分，和 Spring 没有强耦合。

👉 所以：

* 如果换了 DI 框架（比如 CDI、Guice），`@Resource` 还能用；
* 但 `@Autowired` 就只能在 Spring 里用。

---

## 2. 注入方式默认规则

* **`@Autowired`**（默认按 **类型** 注入）

  1. 先根据 **类型** 找匹配的 Bean。
  2. 如果有多个同类型 Bean，再根据 **变量名 / @Qualifier** 来精确定位。
  3. 支持 `@Qualifier("beanName")` 指定 Bean。

  ```java
  @Autowired
  private UserService userService; // 按类型找，如果有多个，再看字段名或 @Qualifier
  ```

* **`@Resource`**（默认按 **名称** 注入）

  1. 默认先按 **属性名** 查找 Bean。
  2. 如果找不到，再按 **类型** 匹配。
  3. 可以用 `@Resource(name="beanName")` 明确指定 Bean。

  ```java
  @Resource
  private UserService userService; // 先按 userService 名称找
  ```

👉 记忆口诀：

* `@Autowired` —— **先看类型**；
* `@Resource` —— **先看名字**。

---

## 3. 依赖是否必须

* **`@Autowired`**

  * 默认依赖是 **必须** 的。
  * 如果找不到 Bean，会报错。
  * 可以设置 `@Autowired(required = false)` 让它变成可选。

  ```java
  @Autowired(required = false)
  private UserService userService;
  ```

* **`@Resource`**

  * 没有 `required` 属性。
  * 如果找不到 Bean，会直接报错，不支持可选注入。

---

## 4. 用法场景

* 如果你是 **纯 Spring 项目**，推荐 `@Autowired` + `@Qualifier`，灵活度高。
* 如果你希望代码更 **标准化、可移植**，推荐用 `@Resource`。
* 在团队里，通常约定一种注解统一使用，避免混乱。

---

✅ **总结表格：**

| 特性     | `@Autowired` (Spring) | `@Resource` (JSR-250)   |
| ------ | --------------------- | ----------------------- |
| 所属规范   | Spring 专用             | Java 标准（JSR-250）        |
| 默认注入规则 | 按类型 -> 名称             | 按名称 -> 类型               |
| 是否可选   | `required=false` 可选   | 不支持，可选性差                |
| 常用搭配   | `@Qualifier` 指定 Bean  | `@Resource(name="...")` |
| 可移植性   | 较差（只能在 Spring）        | 较好（标准注解）                |

---

# 🚀Day 6
---
## 知识要点 📌

# MySQL的安装
[**MySQL安装教程**](https://heuqqdmbyk.feishu.cn/wiki/ZRSFwACsRiBD2NkV7bmcrJhInme?from=from_copylink)
# MySQL的连接

---
## 1. 什么是 MySQL 连接？

当你要用 MySQL 数据库时，你的程序（或者命令行工具）需要“连”上 MySQL 服务，这就叫 **数据库连接**。
连接时要告诉 MySQL：

* **主机**（host）：数据库在哪台电脑上，一般本机是 `localhost` 或 `127.0.0.1`
* **端口**（port）：MySQL 默认端口是 `3306`
* **用户名**（user）：谁来访问数据库，比如 `root`
* **密码**（password）：防止陌生人随便访问
* **数据库名**（database）：想操作哪个数据库

---

## 2. MySQL 连接方式

### （1）命令行连接

```bash
mysql -u root -p
```

👉 `-u root` 指定用户名
👉 `-p` 让你输入密码（不会直接显示出来）

如果 MySQL 不是默认端口，可以这样：

```bash
mysql -h 127.0.0.1 -P 3306 -u root -p
```

👉 `-h`：主机
👉 `-P`：端口

---

### （2）程序连接（举例）

* **Python**

```python
import mysql.connector

conn = mysql.connector.connect(
    host="localhost",
    user="root",
    password="123456",
    database="testdb"
)

cursor = conn.cursor()
cursor.execute("SELECT * FROM users")
print(cursor.fetchall())
```

* **Java**

```java
Connection conn = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/testdb", "root", "123456");
```

---

## 3. 常见错误

* **ERROR 1045 (28000)**
  表示用户名或密码错误，或者这个用户没有权限从当前主机连接。
  👉 解决：确认用户名、密码，或者检查用户是否有 `localhost` 登录权限。

* **Can't connect to MySQL server on 'localhost' (10061)**
  表示 MySQL 服务没启动。
  👉 解决：先启动服务 `service mysql start` 或者 `net start mysql`。

---

## 4. 总结

MySQL 的连接本质上就是：
**程序（客户端） -> 主机（IP） -> 端口（3306） -> 用户名 + 密码 -> 数据库**。
你就可以像开门一样，用正确的钥匙（账号密码）去访问数据库。

---

# MySQL 的数据模型

---

## 1. 什么是 MySQL 数据模型？

在数据库里，**数据模型就是数据的组织方式**，包括数据存储的结构、数据之间的关系、以及如何约束和操作数据。
在 MySQL 中，最常见的是 **关系数据模型**，因为 MySQL 是关系型数据库。

---

## 2. MySQL 常见的数据模型类型

1. **层次模型（Hierarchical Model）**

   * 数据像树一样，一层一层往下。
   * 现在很少单独用，但可以用外键来模拟。

2. **网状模型（Network Model）**

   * 数据像网格一样，节点之间有多对多关系。
   * 在 MySQL 中主要通过**中间表**实现。

3. **关系模型（Relational Model）👉 MySQL 主要用的**

   * 把数据放到“表”里，每个表由“行”和“列”组成。
   * 表和表之间通过 **主键（Primary Key）**、**外键（Foreign Key）** 建立联系。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cd765d0577364324896dc6a2caaf1e76.png)

---

## 3. 举个例子

我们设计一个 **学生-课程-选课** 的数据模型：

* **学生表（Student）**

```sql
CREATE TABLE Student (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50),
    age INT
);
```

* **课程表（Course）**

```sql
CREATE TABLE Course (
    course_id INT PRIMARY KEY AUTO_INCREMENT,
    course_name VARCHAR(100)
);
```

* **选课表（Enrollment） → 用来建立多对多关系**

```sql
CREATE TABLE Enrollment (
    student_id INT,
    course_id INT,
    grade DECIMAL(3,1),
    PRIMARY KEY(student_id, course_id),
    FOREIGN KEY(student_id) REFERENCES Student(student_id),
    FOREIGN KEY(course_id) REFERENCES Course(course_id)
);
```

这样就能表达出：

* 一个学生可以选多门课
* 一门课可以被多个学生选

---

## 4. Java 代码演示（JDBC）

我们用 JDBC 来操作这个模型：

```java
import java.sql.*;

public class MySQLDataModelExample {
    public static void main(String[] args) {
        String url = "jdbc:mysql://localhost:3306/school";
        String user = "root";
        String password = "123456";

        try (Connection conn = DriverManager.getConnection(url, user, password)) {
            // 插入学生
            String insertStudent = "INSERT INTO Student(name, age) VALUES (?, ?)";
            try (PreparedStatement ps = conn.prepareStatement(insertStudent)) {
                ps.setString(1, "张三");
                ps.setInt(2, 20);
                ps.executeUpdate();
            }

            // 插入课程
            String insertCourse = "INSERT INTO Course(course_name) VALUES (?)";
            try (PreparedStatement ps = conn.prepareStatement(insertCourse)) {
                ps.setString(1, "数据库原理");
                ps.executeUpdate();
            }

            // 插入选课关系
            String insertEnrollment = "INSERT INTO Enrollment(student_id, course_id, grade) VALUES (?, ?, ?)";
            try (PreparedStatement ps = conn.prepareStatement(insertEnrollment)) {
                ps.setInt(1, 1);  // 学生ID
                ps.setInt(2, 1);  // 课程ID
                ps.setDouble(3, 95.5);
                ps.executeUpdate();
            }

            System.out.println("数据插入成功！");
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
```

---

## 5. 总结

* MySQL 的 **核心数据模型是关系模型**（表 + 行 + 列）。
* **一对多**：用外键实现
* **多对多**：用中间表实现
* **Java 中**一般通过 JDBC 或者 ORM（比如 Hibernate、MyBatis）操作这些数据模型。

---
# SQL语句


---

## 一、SQL 的概念

SQL（Structured Query Language，结构化查询语言）是用来 **操作数据库** 的语言，主要作用有：

1. **数据定义**（DDL：Data Definition Language） → 建库建表。
2. **数据操作**（DML：Data Manipulation Language） → 增删改。
3. **数据查询**（DQL：Data Query Language） → 查。
4. **数据控制**（DCL：Data Control Language） → 权限、安全。
5. **事务控制**（TCL：Transaction Control Language） → 提交、回滚。

---

## 二、SQL 分类 & 语法

### 1. **DDL（数据定义语言）**

主要是 **定义数据库对象**（数据库、表、视图等）。

常用命令：

```sql
-- 创建数据库
CREATE DATABASE mydb;

-- 删除数据库
DROP DATABASE mydb;

-- 使用数据库
USE mydb;

-- 创建表
CREATE TABLE student (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50) NOT NULL,
    age INT,
    score DECIMAL(5,2)
);

-- 修改表（增加字段）
ALTER TABLE student ADD gender CHAR(1);

-- 修改表（修改字段类型）
ALTER TABLE student MODIFY age SMALLINT;

-- 删除表
DROP TABLE student;
```

---

### 2. **DML（数据操作语言）**

主要是 **对数据进行增删改**。

```sql
-- 插入数据
INSERT INTO student (name, age, score, gender)
VALUES ('Tom', 18, 88.5, 'M');

-- 修改数据
UPDATE student
SET score = 90
WHERE name = 'Tom';

-- 删除数据
DELETE FROM student
WHERE age < 18;
```

---

### 3. **DQL（数据查询语言）**

核心就是 `SELECT`，SQL 的灵魂。

```sql
-- 基本查询
SELECT * FROM student;

-- 指定字段查询
SELECT name, score FROM student;

-- 条件查询
SELECT * FROM student WHERE age > 18;

-- 排序
SELECT * FROM student ORDER BY score DESC;

-- 限制条数
SELECT * FROM student LIMIT 5;

-- 聚合函数
SELECT COUNT(*) AS total, AVG(score) AS avg_score FROM student;

-- 分组
SELECT gender, AVG(score) FROM student GROUP BY gender;

-- 分组 + 条件
SELECT gender, AVG(score) AS avg_score
FROM student
GROUP BY gender
HAVING avg_score > 80;

-- 连接查询
SELECT s.name, c.course_name
FROM student s
JOIN course c ON s.id = c.stu_id;

-- 子查询
SELECT * FROM student
WHERE score > (SELECT AVG(score) FROM student);
```

👉 **重点**：`WHERE` 和 `HAVING` 区别

* `WHERE` 是在 **分组前过滤**。
* `HAVING` 是在 **分组后过滤**。

---

### 4. **DCL（数据控制语言）**

管理数据库用户 & 权限。

```sql
-- 创建用户
CREATE USER 'tom'@'localhost' IDENTIFIED BY '123456';

-- 授权
GRANT SELECT, INSERT ON mydb.* TO 'tom'@'localhost';

-- 回收权限
REVOKE INSERT ON mydb.* FROM 'tom'@'localhost';

-- 删除用户
DROP USER 'tom'@'localhost';
```

---

### 5. **TCL（事务控制语言）**

事务主要保证数据一致性。
事务四大特性：**ACID**（原子性、一致性、隔离性、持久性）。

```sql
-- 开启事务
START TRANSACTION;

-- 执行语句
UPDATE account SET balance = balance - 100 WHERE id = 1;
UPDATE account SET balance = balance + 100 WHERE id = 2;

-- 提交事务
COMMIT;

-- 回滚事务
ROLLBACK;
```

---

## 三、SQL 相关的重点知识点

### 1. **主键、外键、唯一键**

* **主键（PRIMARY KEY）**：唯一标识一行数据。
* **外键（FOREIGN KEY）**：建立表之间的联系。
* **唯一键（UNIQUE）**：值不能重复。

```sql
CREATE TABLE course (
    course_id INT PRIMARY KEY AUTO_INCREMENT,
    course_name VARCHAR(50) UNIQUE,
    stu_id INT,
    FOREIGN KEY (stu_id) REFERENCES student(id)
);
```

---

### 2. **索引（Index）**

提高查询速度，就像书本目录。

```sql
-- 创建普通索引
CREATE INDEX idx_name ON student(name);

-- 创建唯一索引
CREATE UNIQUE INDEX idx_score ON student(score);

-- 删除索引
DROP INDEX idx_name ON student;
```

---

### 3. **视图（View）**

把查询结果当成虚拟表。

```sql
CREATE VIEW high_score_students AS
SELECT name, score FROM student WHERE score > 85;

SELECT * FROM high_score_students;
```

---

### 4. **存储过程 & 函数**

SQL 中的“程序”。

```sql
-- 存储过程
DELIMITER $$
CREATE PROCEDURE getStudentById(IN stu_id INT)
BEGIN
    SELECT * FROM student WHERE id = stu_id;
END $$
DELIMITER ;

-- 调用
CALL getStudentById(1);

-- 函数
DELIMITER $$
CREATE FUNCTION addScore(base INT, extra INT)
RETURNS INT
BEGIN
    RETURN base + extra;
END $$
DELIMITER ;

SELECT addScore(80, 5);
```

---

### 5. **触发器（Trigger）**

自动触发执行的操作。

```sql
CREATE TRIGGER before_insert_student
BEFORE INSERT ON student
FOR EACH ROW
BEGIN
    SET NEW.score = IFNULL(NEW.score, 60);
END;
```

---

## 四、总结（速记表）

| 类型  | 关键字                      | 功能      |
| --- | ------------------------ | ------- |
| **DDL** | CREATE / ALTER / DROP    | 定义数据库结构 |
| **DML** | INSERT / UPDATE / DELETE | 增删改数据   |
| **DQL** | SELECT                   | 查询数据    |
| DCL | GRANT / REVOKE           | 权限控制    |
| TCL | COMMIT / ROLLBACK        | 事务控制    |

---
# DDL
## DDL-数据库
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/baae90d55ab94b08bcc61a8819ba7c85.png)
以下是对您提供的五条 SQL 语句的详细讲解，包括每条语法的用途、语法结构、注意事项，并为每条语句提供代码示例。最后，用表格总结这些语句的核心信息。

---

### **1. 查询所有数据库**
#### **语法**
```sql
SHOW DATABASES;
```
#### **用途**
用于列出当前数据库管理系统中所有的数据库名称。常用于检查数据库服务器中存在的数据库，特别是在管理多个数据库时。

#### **说明**
- 权限要求：执行此语句需要用户有 `SHOW DATABASES` 权限。
- 返回结果：一个包含所有数据库名称的列表（通常以单列形式返回）。
- 数据库特定：大多数关系型数据库（如 MySQL、MariaDB）支持此语法，但某些数据库（如 PostgreSQL）使用其他命令（如 `\l`）。
- 注意：某些数据库可能因权限限制只显示用户有权访问的数据库。

#### **示例**
```sql
SHOW DATABASES;
```
**输出示例**（假设服务器有以下数据库）：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/94f951589f7e4c35b0779d90378ce204.png)


---

### **2. 查询当前数据库**
#### **语法**
```sql
SELECT DATABASE();
```
#### **用途**
返回当前会话正在使用的数据库名称。如果未选择任何数据库，返回 `NULL`。

#### **说明**
- 无参数：`DATABASE()` 是一个函数，不需要参数。
- 使用场景：常用于调试或确认当前操作的数据库。
- 注意：如果未通过 `USE` 语句选择数据库，执行结果为 `NULL`。
- 数据库支持：MySQL、MariaDB 支持，PostgreSQL 使用 `SELECT current_database();`。

#### **示例**
```sql
SELECT DATABASE();
```
**输出示例**（假设当前使用 `shop` 数据库）：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c51da4b9ff1f47b5b9fdd8c83434276b.png)


**未选择数据库时的输出**：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/657b718e661e4d888851cb6b72320246.png)

---

### **3. 使用/切换数据库**
#### **语法**
```sql
USE database_name;
```
#### **用途**
切换当前会话的默认数据库，后续 SQL 语句将在该数据库中执行。

#### **说明**
- 参数：`database_name` 是目标数据库的名称。
- 权限要求：用户必须对目标数据库有访问权限。
- 注意：
  - 数据库必须存在，否则报错（如 `Unknown database`）。
  - 切换数据库只影响当前会话，不影响其他会话或全局设置。
- 使用场景：需要在多个数据库之间切换时使用。

#### **示例**
```sql
USE shop;
SELECT DATABASE(); -- 验证切换结果
```
**输出**：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/413102791962465cae607ed4429b27cc.png)

**错误示例**（尝试切换不存在的数据库）：
```sql
USE nonexistent_db;
```
**报错**：
```
ERROR 1049 (42000): Unknown database 'nonexistent_db'
```

---

### **4. 创建数据库**
#### **语法**
```sql
CREATE DATABASE [IF NOT EXISTS] database_name [DEFAULT CHARSET utf8mb4];
```
#### **用途**
创建新的数据库，可指定字符集以支持特定编码（如 UTF-8）。

#### **说明**
- **参数**：
  - `database_name`：新数据库的名称。
  - `IF NOT EXISTS`：可选，防止数据库已存在时报错。
  - `DEFAULT CHARSET utf8mb4`：可选，指定默认字符集（`utf8mb4` 支持完整的 Unicode 字符，包括表情符号）。
- 权限要求：需要 `CREATE` 权限。
- 注意：
  - 数据库名在同一服务器中必须唯一。
  - 字符集和排序规则（如 `COLLATE`）影响数据存储和比较。
  - 默认字符集因数据库而异（MySQL 常用 `utf8mb4`，PostgreSQL 默认 `UTF8`）。
- 使用场景：初始化项目时创建数据库。

#### **示例**
```sql
CREATE DATABASE IF NOT EXISTS blog DEFAULT CHARSET utf8mb4;
```
**验证**：
```sql
SHOW DATABASES;
```
**输出**：
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/caa799709d124150af4fa8d42132c22e.png)


---

### **5. 删除数据库**
#### **语法**
```sql
DROP DATABASE [IF EXISTS] database_name;
```
#### **用途**
永久删除指定数据库及其所有内容（包括表、数据、索引等）。

#### **说明**
- **参数**：
  - `database_name`：要删除的数据库名称。
  - `IF EXISTS`：可选，防止数据库不存在时报错。
- 权限要求：需要 `DROP` 权限。
- 注意：
  - 删除操作不可恢复，需谨慎使用。
  - 删除数据库会移除其所有表和数据。
  - 某些数据库（如 PostgreSQL）可能有类似命令（如 `DROP DATABASE name`）。
- 使用场景：清理无用数据库或重置环境。

#### **示例**
```sql
DROP DATABASE IF EXISTS blog;
```
**验证**：
```sql
SHOW DATABASES;
```
**输出**（假设 `blog` 已删除）：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/56c9ec8f73e74088b898db849810ac98.png)

---

### **6. 表格总结**
以下表格总结了上述五条 SQL 语句的核心信息：

| **语句**                     | **用途**                           | **语法**                                                                 | **关键参数**                     | **权限要求**            | **注意事项**                                                                 |
|------------------------------|------------------------------------|--------------------------------------------------------------------------|----------------------------------|-------------------------|------------------------------------------------------------------------------|
| `SHOW DATABASES`            | 查询所有数据库                     | `SHOW DATABASES;`                                                       | 无                               | `SHOW DATABASES`        | 仅显示用户有权限的数据库，可能因数据库不同（如 PostgreSQL）语法略有变化。         |
| `SELECT DATABASE()`         | 查询当前使用的数据库               | `SELECT DATABASE();`                                                    | 无                               | 无                      | 未选择数据库时返回 `NULL`。                                                  |
| `USE database_name`         | 切换当前会话的数据库               | `USE database_name;`                                                    | `database_name`                  | 数据库访问权限          | 数据库必须存在，否则报错；只影响当前会话。                                     |
| `CREATE DATABASE`           | 创建新数据库                       | `CREATE DATABASE [IF NOT EXISTS] database_name [DEFAULT CHARSET utf8mb4];` | `database_name`, `IF NOT EXISTS`, `DEFAULT CHARSET` | `CREATE`                | 数据库名需唯一，建议指定字符集（如 `utf8mb4`）。                             |
| `DROP DATABASE`             | 删除数据库及其内容                 | `DROP DATABASE [IF EXISTS] database_name;`                               | `database_name`, `IF EXISTS`     | `DROP`                  | 删除不可恢复，需谨慎；建议使用 `IF EXISTS` 避免不存在数据库时的错误。          |

---

### **7. 补充说明**
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e6818ebe127a47b38ba3568bfd0210aa.png)

- **数据库差异**：上述语法主要基于 MySQL/MariaDB。其他数据库（如 PostgreSQL、SQL Server、Oracle）可能有细微差异。例如：
  - PostgreSQL 查询数据库：`SELECT datname FROM pg_database;`
  - SQL Server 创建数据库：`CREATE DATABASE name;`
- **安全性**：执行 `DROP DATABASE` 前，建议备份数据。
- **字符集选择**：`utf8mb4` 是推荐的字符集，支持多语言和表情符号，兼容性更好。
- **权限管理**：确保用户有适当权限，否则可能遇到 `Access denied` 错误。

## 安装DataGrip
DataGrip是JetBrains旗下的一款数据库管理工具，是管理和开发MySQL、Oracle、PostgreSQL的理想解决方案。
[DataGrip官网](https://www.jetbrains.com/zh-cn/datagrip/) 

[DataGrip安装文档](https://heuqqdmbyk.feishu.cn/wiki/FAa3wj0nYi4xGBksbFuchBK8nhe?from=from_copylink)
## DDL-表结构-创建
### 整体感知
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e820ba028b224b148a12ef891d7b8245.png)
**无约束版**
```sql
create table USER(
    id int comment '用户的ID',
    username varchar(50) comment '用户名',
    name varchar(10) comment '姓名',
    age int comment '年龄',
    gender char(1) comment '性别'

) comment '用户表';
```
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d30479df469c469ea66cec6096e892bd.png)
**有约束版**
```sql
create table USER(
    id int primary key comment '用户的ID',
    username varchar(50) not null unique comment '用户名',
    name varchar(10) not null comment '姓名',
    age int comment '年龄',
    gender char(1) default '男' comment '性别'

) comment '用户表';
```
---
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e66306ce31944492859fe64b4ad7d7f1.png)

### 1️⃣ DDL 简介

DDL 是用来 **定义和管理数据库对象** 的 SQL 语言，包括：

* **CREATE**：创建数据库、表、索引等
* **ALTER**：修改表结构或数据库对象
* **DROP**：删除表或数据库
* **TRUNCATE**：清空表数据（但保留表结构）

我们这里重点讲 **CREATE TABLE**，也就是创建表结构。

---

### 2️⃣ 创建表的基本语法

```sql
CREATE TABLE 表名 (
    列名1 数据类型 [约束条件],
    列名2 数据类型 [约束条件],
    ...
    [表级约束]
);
```

* **表名**：你要创建的表的名字
* **列名**：表里的字段名
* **数据类型**：字段的数据类型（如 INT、VARCHAR、DATE 等）
* **约束条件**：字段的限制，如是否可以为空、是否唯一、是否是主键等

---

### 3️⃣ 常用数据类型

| 数据类型           | 描述             |
| -------------- | -------------- |
| INT            | 整数             |
| BIGINT         | 大整数            |
| FLOAT / DOUBLE | 浮点数            |
| CHAR(n)        | 固定长度字符串        |
| VARCHAR(n)     | 可变长度字符串        |
| DATE           | 日期（YYYY-MM-DD） |
| DATETIME       | 日期+时间          |
| TEXT           | 长文本            |

---

### 4️⃣ 常用约束条件

| 约束              | 说明                 |
| --------------- | ------------------ |
| PRIMARY KEY     | 主键，唯一标识一行，不能为 NULL |
| UNIQUE          | 唯一约束，字段值不能重复       |
| NOT NULL        | 非空，必须有值            |
| DEFAULT         | 默认值                |
| AUTO\_INCREMENT | 自增（通常用于主键）         |
| FOREIGN KEY     | 外键，关联另一张表          |

---

### 5️⃣ 创建表实例

#### 示例 1：简单用户表

```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    created_at DATETIME DEFAULT CURRENT_TIMESTAMP
);
```

* `id`：自增主键
* `username`：必填字段
* `email`：唯一字段
* `created_at`：默认值为当前时间
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/cb6fed5a553e4f919191978b0c95db96.png)

#### 示例 2：带外键的订单表

```sql
CREATE TABLE orders (
    order_id INT AUTO_INCREMENT PRIMARY KEY,
    user_id INT NOT NULL,
    order_date DATE NOT NULL,
    amount DECIMAL(10,2) NOT NULL,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

* `user_id` 是外键，关联 `users` 表的 `id`
* `amount` 是金额，保留两位小数
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/1c5c797c8d1f47b2bfdec4314ece2a62.png)

---

### 6️⃣ 小技巧

1. **命名规范**：表名用复数（如 `users`），字段名用小写下划线分隔（如 `user_id`）
2. **先规划主键**：保证数据唯一性
3. **字段顺序**：常用查询的字段放前面
4. **外键关系**：方便做数据完整性检查

**Q&A**
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/26de967690094db7a7443049f3b0258b.png)

---

## DDL-表操作-数据类型
### 数值类型

| 类型                | 大小 (Byte) | 有符号范围 (SIGNED)                                          | 无符号范围 (UNSIGNED)                | 描述      | 示例                                |
| ----------------- | --------- | ------------------------------------------------------- | ------------------------------- | ------- | --------------------------------- |
| TINYINT           | 1         | -128 \~ 127                                             | 0 \~ 255                        | 小整数值    | `TINYINT(3)`                      |
| SMALLINT          | 2         | -32,768 \~ 32,767                                       | 0 \~ 65,535                     | 大整数值    | `SMALLINT(5)`                     |
| MEDIUMINT         | 3         | -8,388,608 \~ 8,388,607                                 | 0 \~ 16,777,215                 | 较大整数值   | `MEDIUMINT(8)`                    |
| INT / INTEGER     | 4         | -2,147,483,648 \~ 2,147,483,647                         | 0 \~ 4,294,967,295              | 大整数值    | `INT(11)`                         |
| BIGINT            | 8         | -9,223,372,036,854,775,808 \~ 9,223,372,036,854,775,807 | 0 \~ 18,446,744,073,709,551,615 | 极大整数值   | `BIGINT(20)`                      |
| FLOAT             | 4         | -3.402823466E+38 \~ 3.402823466E+38                     | 0 \~ 3.402823466E+38            | 单精度浮点数  | `FLOAT(5,2)` <br> 5=总位数，2=小数位数    |
| DOUBLE / REAL     | 8         | -1.7976931348623157E+308 \~ 1.7976931348623157E+308     | 0 \~ 1.7976931348623157E+308    | 双精度浮点数  | `DOUBLE(10,2)` <br> 10=总位数，2=小数位数 |
| DECIMAL / NUMERIC | 可变        | 精确小数                                                    | 精确小数                            | 精度更高的小数 | `DECIMAL(8,3)` <br> 8=总位数，3=小数位数  |

**补充知识点：**

1. `SIGNED` 表示允许负数；`UNSIGNED` 表示非负数。
2. `FLOAT` 和 `DOUBLE` 是近似值，适合科学计算，不适合精确财务计算；`DECIMAL` 是精确小数，适合金额等。
3. 括号里的 `(M,D)` 表示总长度和小数位数，其中 `M` 包括小数点前后的数字总长度，`D` 表示小数位。

---
### 字符串类型


| 分类    | 类型         | 大小范围                     | 描述          | 备注          |
| ----- | ---------- | ------------------------ | ----------- | ----------- |
| 字符串类型 | CHAR       | 0 \~ 255 bytes           | 定长字符串       | 长度固定，不够补空格  |
| 字符串类型 | VARCHAR    | 0 \~ 65,535 bytes        | 变长字符串       | 长度可变，节省空间   |
| 二进制数据 | TINYBLOB   | 0 \~ 255 bytes           | 小型二进制数据     | 可存储小文件、图片等  |
| 字符串类型 | TINYTEXT   | 0 \~ 255 bytes           | 短文本字符串      | 存储短文本信息     |
| 二进制数据 | BLOB       | 0 \~ 65,535 bytes        | 二进制形式的长文本数据 | 用于存储图片、音频等  |
| 字符串类型 | TEXT       | 0 \~ 65,535 bytes        | 长文本数据       | 常用于文章内容     |
| 二进制数据 | MEDIUMBLOB | 0 \~ 16,777,215 bytes    | 中等长度二进制数据   | 存储中等文件      |
| 字符串类型 | MEDIUMTEXT | 0 \~ 16,777,215 bytes    | 中等长度文本数据    | 存储中等文章内容    |
| 二进制数据 | LONGBLOB   | 0 \~ 4,294,967,295 bytes | 极大二进制数据     | 可存储大型文件，如视频 |
| 字符串类型 | LONGTEXT   | 0 \~ 4,294,967,295 bytes | 极大文本数据      | 存储超长文章或书籍   |

---

**补充说明：**

1. **CHAR** 是定长，`VARCHAR` 是变长，所以在查询和存储上 `VARCHAR` 更节省空间。
2. **BLOB** 系列用于 **二进制数据**（图片、音频、视频等），`TEXT` 系列用于 **文本数据**。
3. 各类型的最大长度与 **字符集** 有关系，例如 utf8 编码一个字符占 3 字节，会影响 `VARCHAR` 和 `TEXT` 最大能存储的字符数。

---

**char与varchar的对比**

| 属性   | CHAR(n)                        | VARCHAR(n)                       |
| ---- | ------------------------------ | -------------------------------- |
| 存储方式 | 定长                             | 变长                               |
| 占用空间 | 总是占用 n 个字符空间                   | 实际字符长度 + 额外 1\~2 字节记录长度          |
| 示例 1 | `CHAR(10)` 存 `A` → 占用 10 个字节   | `VARCHAR(10)` 存 `A` → 占用 1 个字节   |
| 示例 2 | `CHAR(10)` 存 `ABC` → 占用 10 个字节 | `VARCHAR(10)` 存 `ABC` → 占用 3 个字节 |
| 性能   | 访问速度略高                         | 访问速度略低（需要动态长度计算）                 |
| 磁盘空间 | 浪费空间                           | 节约空间                             |

---

**总结：**

1. **CHAR** 适合长度固定的字段，如身份证号、性别、状态码等。
2. **VARCHAR** 适合长度可变的字段，如姓名、地址、邮箱等。
3. 如果频繁更新字段值且长度变化大，`VARCHAR` 更节省空间，但 `CHAR` 读写性能略优。

---

### 日期类型
好的，我把你提供的 **MySQL 日期时间类型**整理成一个清晰的表格，补充了一些说明，方便理解：

| 分类     | 类型        | 大小 (Byte) | 范围                                         | 格式                    | 描述               |
| ------ | --------- | --------- | ------------------------------------------ | --------------------- | ---------------- |
| 日期类型   | **DATE**      | 3         | 1000-01-01 \~ 9999-12-31                   | YYYY-MM-DD            | 仅存储日期值           |
| 时间类型   | TIME      | 3         | -838:59:59 \~ 838:59:59                    | HH\:MM\:SS            | 存储时间或持续时间        |
| 日期类型   | YEAR      | 1         | 1901 \~ 2155                               | YYYY                  | 年份值              |
| 日期时间类型 | **DATETIME**  | 8         | 1000-01-01 00:00:00 \~ 9999-12-31 23:59:59 | YYYY-MM-DD HH\:MM\:SS | 混合日期和时间值         |
| 日期时间类型 | TIMESTAMP | 4         | 1970-01-01 00:00:01 \~ 2038-01-19 03:14:07 | YYYY-MM-DD HH\:MM\:SS | 混合日期和时间值，通常用于时间戳 |

---

**补充说明：**

1. **DATE**：只存日期，不存时间。
2. **TIME**：存储一天内的时间，也可以表示时间间隔，支持负值。
3. **YEAR**：只存年份，用于表示年份信息。
4. **DATETIME**：完整的日期+时间组合，存储范围很大，适合历史记录。
5. **TIMESTAMP**：常用作系统时间戳，会随时区变化而自动转换，存储范围较短（1970–2038），适合记录操作时间。

---
 
## DDL-表结构-查询、修改、删除
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/a596a95e7aee4872a9a2990283931a75.png)
太好了👍 你已经列出了 MySQL 中和 **表结构操作相关的 DDL** 常用语句。
我来逐条帮你讲解，给出通俗说明 + 代码示例，最后再做一个总结表格。

---

### 1️⃣ 查询当前数据库所有表

```sql
SHOW TABLES;
```

* **功能**：查看当前数据库下有哪些表。
* **示例**：

```sql
USE school;
SHOW TABLES;
```

👉 会列出 `school` 数据库里的所有表。

---

### 2️⃣ 查询表结构

```sql
DESC 表名;
```

* **功能**：查看表的字段、类型、是否允许空值、主键信息等。
* **示例**：

```sql
DESC users;
```

👉 会显示 `users` 表的所有字段及约束。

---

### 3️⃣ 查询建表语句

```sql
SHOW CREATE TABLE 表名;
```

* **功能**：查看建表时完整的 SQL 语句，包括字段定义和约束。
* **示例**：

```sql
SHOW CREATE TABLE users;
```

👉 会输出 `users` 表的完整建表语句。

---

### 4️⃣ 添加字段

```sql
ALTER TABLE 表名 ADD 字段名 类型(长度) [COMMENT '注释'] [约束];
```

* **功能**：在已有表中新增字段。
* **示例**：

```sql
ALTER TABLE users ADD age INT COMMENT '年龄';
```

👉 给 `users` 表新增 `age` 字段。

---

### 5️⃣ 修改字段类型

```sql
ALTER TABLE 表名 MODIFY 字段名 新数据类型(长度);
```

* **功能**：修改字段的数据类型或长度。
* **示例**：

```sql
ALTER TABLE users MODIFY age SMALLINT;
```

👉 把 `users` 表中的 `age` 字段改为 `SMALLINT`。

---

### 6️⃣ 修改字段名和字段类型

```sql
ALTER TABLE 表名 CHANGE 旧字段名 新字段名 类型(长度) [COMMENT '注释'] [约束];
```

* **功能**：可以同时修改字段名和字段类型。
* **示例**：

```sql
ALTER TABLE users CHANGE username user_name VARCHAR(100) COMMENT '用户名';
```

👉 把 `username` 改为 `user_name`，并修改长度。

---

### 7️⃣ 删除字段

```sql
ALTER TABLE 表名 DROP COLUMN 字段名;
```

* **功能**：删除某个字段。
* **示例**：

```sql
ALTER TABLE users DROP COLUMN age;
```

👉 删除 `users` 表中的 `age` 字段。

---

### 8️⃣ 修改表名

```sql
ALTER TABLE 表名 RENAME TO 新表名;
```

* **功能**：给表改名字。
* **示例**：

```sql
ALTER TABLE users RENAME TO user_info;
```

👉 把 `users` 表改名为 `user_info`。

---

### 9️⃣ 删除表

```sql
DROP TABLE [IF EXISTS] 表名;
```

* **功能**：删除表，表内数据也会一并删除。
* **示例**：

```sql
DROP TABLE IF EXISTS orders;
```

👉 删除 `orders` 表（存在才删，不存在就忽略）。

---

### 🔟 总结表格


---

### 📑 DDL 表结构操作总结

| 功能           | 写法                                                            | 注意事项                             |
| ------------ | ------------------------------------------------------------- | -------------------------------- |
| **查询所有表**    | `SHOW TABLES;`                                                | 必须先 `USE 数据库;`，否则查不到表            |
| **查询表结构**    | `DESC 表名;`                                                    | 只展示字段名、类型、约束，不能看到完整建表语句          |
| **查询建表语句**   | `SHOW CREATE TABLE 表名;`                                       | 可以看到完整的 SQL，包括字符集、约束等            |
| **添加字段**     | `ALTER TABLE 表名 ADD 字段名 类型(长度) [COMMENT '注释'] [约束];`          | 新增字段默认在表最后；如果要指定位置可用 `AFTER 字段名` |
| **修改字段类型**   | `ALTER TABLE 表名 MODIFY 字段名 新数据类型(长度);`                        | 只能改类型和约束，**字段名不变**               |
| **修改字段名和类型** | `ALTER TABLE 表名 CHANGE 旧字段名 新字段名 类型(长度) [COMMENT '注释'] [约束];` | 改字段名时必须写新类型，不写会报错                |
| **删除字段**     | `ALTER TABLE 表名 DROP COLUMN 字段名;`                             | 删除操作不可恢复，删除前最好确认无用               |
| **修改表名**     | `ALTER TABLE 表名 RENAME TO 新表名;`                               | 表名会彻底修改，原表名失效                    |
| **删除表**      | `DROP TABLE [IF EXISTS] 表名;`                                  | `IF EXISTS` 防止报错；删除表会删除所有数据，谨慎操作 |

---

✅ **记忆小技巧**：

* **查** 用 `SHOW`（SHOW TABLES / SHOW CREATE TABLE）
* **看结构** 用 `DESC`
* **改** 用 `ALTER`（ADD / MODIFY / CHANGE / DROP / RENAME）
* **删表** 用 `DROP`

---

# DML
## DML-insert
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9d0a07a9377e44198d7c763878af546f.png)
好的 👍 我来给你系统讲解一下 **DML（Data Manipulation Language）之 INSERT 语句**。

---

### 1️⃣ DML 简介

DML（数据操作语言）主要用于 **对数据进行操作**，常见语句有：

* `INSERT`：插入数据
* `UPDATE`：更新数据
* `DELETE`：删除数据

今天我们重点讲 **INSERT 语句**。

---

### 2️⃣ INSERT 语法

```sql
-- 方式 1：插入所有字段（字段必须一一对应）
INSERT INTO 表名 VALUES (值1, 值2, 值3, ...);

-- 方式 2：插入指定字段
INSERT INTO 表名 (字段1, 字段2, ...) VALUES (值1, 值2, ...);

-- 方式 3：一次插入多行
INSERT INTO 表名 (字段1, 字段2, ...) 
VALUES (值1, 值2, ...), (值1, 值2, ...), ...;

-- 方式 4：从查询结果插入
INSERT INTO 表名 (字段1, 字段2, ...) 
SELECT 字段1, 字段2, ... FROM 其他表;
```

---

### 3️⃣ 代码示例

假设有一个 **users 表**：

```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    email VARCHAR(100),
    age INT
);
```

#### 示例 1：插入所有字段

```sql
INSERT INTO users VALUES (1, 'Alice', 'alice@test.com', 25);
```

👉 注意：必须提供 **所有字段的值**，包括 `id`。如果 `id` 是自增字段，可以用 `NULL` 或省略。

---

#### 示例 2：插入指定字段

```sql
INSERT INTO users (username, email, age) 
VALUES ('Bob', 'bob@test.com', 30);
```

👉 `id` 字段会自动递增。

---

#### 示例 3：一次插入多行

```sql
INSERT INTO users (username, email, age) 
VALUES 
('Cathy', 'cathy@test.com', 22),
('David', 'david@test.com', 28),
('Emma', 'emma@test.com', 35);
```

---

#### 示例 4：插入查询结果

```sql
INSERT INTO users (username, email, age)
SELECT username, email, age FROM old_users;
```

👉 适合 **从一个表迁移数据到另一个表**。

---

### 4️⃣ 总结表格

| 用法     | 语法                                                         | 示例                                                                       | 注意事项                       |
| ------ | ---------------------------------------------------------- | ------------------------------------------------------------------------ | -------------------------- |
| 插入所有字段 | `INSERT INTO 表名 VALUES (...);`                             | `INSERT INTO users VALUES (1, 'Alice', 'a@test.com', 25);`               | 字段顺序必须与表结构一致；自增字段可用 `NULL` |
| 插入指定字段 | `INSERT INTO 表名 (字段1, 字段2, ...) VALUES (...);`             | `INSERT INTO users (username, age) VALUES ('Bob', 30);`                  | 推荐写法，避免字段顺序变化导致出错          |
| 插入多行   | `INSERT INTO 表名 (字段1, 字段2, ...) VALUES (...), (...), ...;` | `INSERT INTO users (username, age) VALUES ('Cathy', 22), ('David', 28);` | 提高效率，减少多次插入                |
| 插入查询结果 | `INSERT INTO 表名 (字段1, 字段2, ...) SELECT ... FROM ...;`      | `INSERT INTO users (username, age) SELECT name, age FROM old_users;`     | 适合批量迁移或复制数据                |

---

⚠️ **注意事项**：

1. 插入时要保证字段类型匹配，否则报错（如 `age` 必须是数字）。
2. 插入字符串要用 `'单引号'`。
3. 插入多行比单行效率高。
4. 推荐使用 **指定字段插入**，避免表结构变更导致 SQL 出错。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/3f3042ae1c154d338162b866f9709a8b.png)


---

## DML-update
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f7abd414cecb4c51bac3b819f631ffe2.png)


在数据库里，**DML（Data Manipulation Language）** 是用来操作表中数据的语言，包括 `INSERT`、`UPDATE`、`DELETE`、`SELECT`。
其中 **`UPDATE`** 就是修改表中已有数据的语句。

---

### 1. 基本语法

```sql
UPDATE 表名
SET 列名1 = 值1, 列名2 = 值2, ...
WHERE 条件;
```

🔹 说明：

* `UPDATE 表名` → 指定要修改数据的表
* `SET` → 设置要修改的列及新值
* `WHERE` → 限定修改范围（⚠️ 如果不写，会修改整个表的所有行，非常危险！）

---

### 2. 简单示例

假设有一个学生表 `students`：

| id | name  | age | score |
| -- | ----- | --- | ----- |
| 1  | Tom   | 18  | 85    |
| 2  | Jerry | 19  | 90    |
| 3  | Alice | 20  | 95    |

#### （1）修改单列

```sql
UPDATE students
SET age = 21
WHERE id = 3;
```

👉 把 `id=3` 的 Alice 年龄改为 21。

---

#### （2）修改多列

```sql
UPDATE students
SET age = 20, score = 100
WHERE name = 'Tom';
```

👉 把 Tom 的年龄改成 20，分数改成 100。

---

#### （3）不加 WHERE（⚠️危险）

```sql
UPDATE students
SET score = 60;
```

👉 所有学生的 `score` 都变成 60。

---

#### （4）结合条件运算符

```sql
UPDATE students
SET score = score + 5
WHERE score < 90;
```

👉 给分数小于 90 的学生加 5 分。

---

#### （5）结合子查询

```sql
UPDATE students
SET score = (SELECT MAX(score) FROM students)
WHERE id = 2;
```

👉 把 Jerry 的分数改为全班最高分。

---

### 3. 注意事项

1. **一定要加 `WHERE` 条件**，否则会全表更新。
2. **UPDATE 是一条一条执行的**，如果数据量大，要注意效率。
3. 可以结合 **事务（Transaction）** 使用：

   ```sql
   START TRANSACTION;
   UPDATE students SET score = 50 WHERE id = 1;
   ROLLBACK; -- 撤销
   COMMIT;   -- 确认提交
   ```
4. **谨慎使用子查询**，有可能带来性能问题。
5. 在批量更新前，最好先 `SELECT` 查看会影响哪些行。

---

### 4. 总结表格

| 用法场景  | 示例语句                                                                      | 说明与注意事项          |
| ----- | ------------------------------------------------------------------------- | ---------------- |
| 修改单列  | `UPDATE students SET age=21 WHERE id=3;`                                  | 只改一列，带 WHERE     |
| 修改多列  | `UPDATE students SET age=20, score=100 WHERE name='Tom';`                 | 可以同时修改多个字段       |
| 批量修改  | `UPDATE students SET score=60;`                                           | ⚠️ 无 WHERE 会全表更新 |
| 条件修改  | `UPDATE students SET score=score+5 WHERE score<90;`                       | 结合条件运算符          |
| 子查询修改 | `UPDATE students SET score=(SELECT MAX(score) FROM students) WHERE id=2;` | 可引用其他查询结果        |
| 事务安全  | `START TRANSACTION; UPDATE ...; ROLLBACK;`                                | 批量更新建议用事务        |
| 性能注意  | 大数据量更新时考虑分批处理                                                             | 避免锁表、阻塞          |

---

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/da1610ecd0984a4cbe3bfcbde98b0493.png)
## DML-delete
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c97a10a8fd3642edbd83676606240674.png)

好的，我们来系统地讲一下 **DML - DELETE**。

在 SQL 中，**DELETE** 属于 DML（Data Manipulation Language，数据操作语言），用来 **删除表中的数据**，但不会删除表本身的结构。

---

### 1. 基本语法

```sql
DELETE FROM 表名
WHERE 条件;
```

* **表名**：要删除数据的表。
* **条件**：指定要删除哪些行，如果省略条件，则会删除整张表的所有数据。

---

### 2. 示例讲解

假设我们有一个 `students` 表：

```sql
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    grade VARCHAR(10)
);

INSERT INTO students (id, name, age, grade) VALUES
(1, 'Tom', 18, 'A'),
(2, 'Lily', 19, 'B'),
(3, 'Jack', 20, 'C'),
(4, 'Lucy', 19, 'B');
```

表数据如下：

| id | name | age | grade |
| -- | ---- | --- | ----- |
| 1  | Tom  | 18  | A     |
| 2  | Lily | 19  | B     |
| 3  | Jack | 20  | C     |
| 4  | Lucy | 19  | B     |

---

#### 示例 1：删除指定条件的记录

```sql
DELETE FROM students
WHERE id = 3;
```

👉 删除 `id=3` 的 Jack，执行后表：

| id | name | age | grade |
| -- | ---- | --- | ----- |
| 1  | Tom  | 18  | A     |
| 2  | Lily | 19  | B     |
| 4  | Lucy | 19  | B     |

---

#### 示例 2：删除多条记录

```sql
DELETE FROM students
WHERE grade = 'B';
```

👉 删除所有成绩为 B 的 Lily、Lucy，执行后表：

| id | name | age | grade |
| -- | ---- | --- | ----- |
| 1  | Tom  | 18  | A     |

---

#### 示例 3：删除所有记录（慎用）

```sql
DELETE FROM students;
```

👉 删除整张表的数据，表为空，但表结构还在。

---

#### 示例 4：带子查询删除

```sql
DELETE FROM students
WHERE id IN (
    SELECT id FROM students WHERE age > 18
);
```

👉 删除所有大于 18 岁的学生。

---

### 3. DELETE 和 TRUNCATE / DROP 的区别

| 操作       | 功能            | 是否可回滚  | 是否删除结构 | 速度 |
| -------- | ------------- | ------ | ------ | -- |
| DELETE   | 删除表中数据（可带条件）  | ✅ 可回滚  | ❌ 保留结构 | 较慢 |
| TRUNCATE | 清空表中所有数据      | ❌ 不可回滚 | ❌ 保留结构 | 较快 |
| DROP     | 删除表本身（连结构一起删） | ❌ 不可回滚 | ✅ 删除结构 | 最快 |

---

### 4. DELETE 使用注意事项

| 注意点           | 说明                                                 |
| ------------- | -------------------------------------------------- |
| 慎用无条件 DELETE  | `DELETE FROM 表名;` 会清空整个表数据                         |
| 最好带 WHERE 子句  | 避免误删数据                                             |
| 可结合事务         | 用 `BEGIN TRANSACTION ... COMMIT / ROLLBACK` 保护数据安全 |
| 索引影响效率        | 如果 WHERE 条件字段有索引，删除会更快                             |
| DELETE 不会释放空间 | 删除后表空间仍存在，可以用 `OPTIMIZE TABLE` 或 `VACUUM`（不同数据库）回收 |

---

✅ 总结：

* **DELETE** 是逐行删除，可带条件。
* 想清空表但保留结构，用 `TRUNCATE`。
* 想删除整个表连结构一起删，用 `DROP`。
* 大量删除时，建议用事务 + 分批删除，避免锁表。

---

要不要我帮你再写一个 **事务+DELETE的示例**，展示如何防止误删？


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4eab55ea9fea40d5bc053450e8667c32.png)
# DQL
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/52471920649c4201945d80c33d6238ca.png)
## DQL-基本查询
 ![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4b9e2a52df3d4685bd31142bf52d073d.png)

---

### 1. 查询多个字段

语法：

```sql
SELECT 字段1, 字段2, 字段3
FROM 表名;
```

👉 用来查询指定的多个字段。

**示例：**

```sql
SELECT id, name, age
FROM students;
```

结果只显示 `id`、`name` 和 `age`，而不是整张表。

---

### 2. 查询所有字段（通配符 \*）

语法：

```sql
SELECT *
FROM 表名;
```

👉 使用 `*` 通配符，可以一次性查询表中的所有字段。

**示例：**

```sql
SELECT *
FROM students;
```

结果包含 `id, name, age, grade` 等所有字段。

⚠️ 注意：生产环境中不建议经常用 `*`，因为字段过多会影响性能，推荐明确写字段名。

---

### 3. 为查询字段设置别名

语法：

```sql
SELECT 字段1 [AS 别名1], 字段2 [AS 别名2]
FROM 表名;
```
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/001336a485b7402c9e9d73ecae59d495.png)

👉 `AS` 可以给查询结果中的列起一个新名字，便于阅读。
👉 `AS` 可以省略，直接写空格即可。
👉别名有空格的时候不能省略引号。

**示例：**

```sql
SELECT name AS student_name, age AS student_age
FROM students;
```

结果显示的列标题是 `student_name` 和 `student_age`。

也可以写成：

```sql
SELECT name student_name, age student_age
FROM students;
```

---

### 4. 去除重复记录（DISTINCT）

语法：

```sql
SELECT DISTINCT 字段列表
FROM 表名;
```

👉 `DISTINCT` 用来去掉查询结果中重复的行。

**示例：**

```sql
SELECT DISTINCT grade
FROM students;
```

如果 `students` 表中有多个学生的成绩是 `B`，只会返回一个 `B`。

---

### 5. 总结表格

| 用法     | 语法                            | 示例                                     | 说明与注意事项                 |
| ------ | ----------------------------- | -------------------------------------- | ----------------------- |
| 查询多个字段 | `SELECT 字段1, 字段2 FROM 表名;`    | `SELECT id, name FROM students;`       | 只查询需要的字段，减少数据量          |
| 查询所有字段 | `SELECT * FROM 表名;`           | `SELECT * FROM students;`              | 查询表的所有字段，开发调试时方便，但生产不推荐 |
| 字段别名   | `SELECT 字段 AS 别名 FROM 表名;`    | `SELECT name AS 姓名 FROM students;`     | 别名便于理解，`AS` 可省略         |
| 去重查询   | `SELECT DISTINCT 字段 FROM 表名;` | `SELECT DISTINCT grade FROM students;` | 去掉重复记录，只保留唯一值           |

---
### 6.基本查询案例
我们来写一个 **SQL 基本查询（SELECT语句）的案例**。我会用一个简单的 **学生表 (students)** 来举例，这样容易理解。

---

#### 表结构：`students`

| id | name | age | grade |
| -- | ---- | --- | ----- |
| 1  | 张三   | 18  | 90    |
| 2  | 李四   | 19  | 85    |
| 3  | 王五   | 17  | 92    |
| 4  | 赵六   | 18  | 75    |

---

#### 1. 查询所有数据

```sql
SELECT * FROM students;
```

👉 显示整张表的所有字段和数据。

---

#### 2. 查询指定字段（只查姓名和成绩）

```sql
SELECT name, grade FROM students;
```

👉 只显示学生姓名和成绩，不显示年龄和id。

---

#### 3. 条件查询（查成绩大于85分的学生）

```sql
SELECT * FROM students
WHERE grade > 85;
```

👉 结果只会显示 **张三(90)** 和 **王五(92)**。

---

#### 4. 排序查询（按成绩从高到低排序）

```sql
SELECT * FROM students
ORDER BY grade DESC;
```

👉 结果会按成绩降序排列。

---

#### 5. 限制结果数量（只查前2个学生）

```sql
SELECT * FROM students
LIMIT 2;
```

👉 只显示前两行数据。

---



✅ 小结：

* 查询时最好明确字段名，避免用 `*`。
* 别名可以提高可读性，尤其是当字段名很复杂时。
* `DISTINCT` 主要用在分类、统计时去重。
**Q&A**
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c6b48c3d58ba42898d221a2ad145c08b.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d686be15f3ff4812be6a2a08e66ff064.png)

---

## DQL-条件查询
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2ec1a906d7724e5bae8c6582bd114584.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d400191162bf40f69033a15332287a5a.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/da6228c1526a41059d8de4917f99d990.png)

我们来系统讲解一下 **DQL（Data Query Language，数据查询语言）中的条件查询**，这是 MySQL 使用最频繁的一部分。

---

### 一、条件查询的作用

条件查询的核心是通过 **`WHERE` 子句** 设置过滤条件，从而只返回满足条件的记录。
常见的应用场景有：

* 查找特定用户
* 筛选出满足条件的订单
* 查询某个时间段内的数据

---

### 二、条件查询常见语法

```sql
SELECT 列名列表
FROM 表名
WHERE 条件表达式;
```

---

### 三、条件运算符分类

#### 1. 比较运算符

* `=` 等于
* `<>` 或 `!=` 不等于
* `>` 大于
* `<` 小于
* `>=` 大于等于
* `<=` 小于等于

示例：

```sql
-- 查询工资大于5000的员工
SELECT name, salary
FROM employee
WHERE salary > 5000;
```

---

#### 2. 逻辑运算符

* `AND` 与（同时满足）
* `OR` 或（满足一个即可）
* `NOT` 非（取反）

示例：

```sql
-- 查询工资大于5000并且部门是IT的员工
SELECT name, salary, dept
FROM employee
WHERE salary > 5000 AND dept = 'IT';
```

---

#### 3. 模糊查询

* `LIKE`：配合通配符

  * `%` 表示任意多个字符
  * `_` 表示单个字符

示例：

```sql
-- 查询名字以A开头的员工
SELECT name
FROM employee
WHERE name LIKE 'A%';
```

---

#### 4. 范围查询

* `BETWEEN ... AND ...`：范围内
* `IN (...)`：集合内

示例：

```sql
-- 查询工资在3000到6000之间的员工
SELECT name, salary
FROM employee
WHERE salary BETWEEN 3000 AND 6000;

-- 查询部门是HR或IT的员工
SELECT name, dept
FROM employee
WHERE dept IN ('HR', 'IT');
```

---

#### 5. 空值判断

* `IS NULL`
* `IS NOT NULL`

示例：

```sql
-- 查询手机号为空的员工
SELECT name
FROM employee
WHERE phone IS NULL;
```

⚠️ 注意：不能用 `= NULL` 判断空值。

---

#### 6. 排序 + 条件组合

配合 `ORDER BY` 使用：

```sql
-- 查询工资大于4000的员工，按工资降序排列
SELECT name, salary
FROM employee
WHERE salary > 4000
ORDER BY salary DESC;
```

---

### 四、总结表格

| 分类    | 运算符                       | 示例                              | 注意事项               |
| ----- | ------------------------- | ------------------------------- | ------------------ |
| 比较运算符 | `=, !=, <>, >, <, >=, <=` | `salary > 5000`                 | 数值和字符串都能用          |
| 逻辑运算符 | `AND, OR, NOT`            | `salary > 5000 AND dept = 'IT'` | 优先级：NOT > AND > OR |
| 模糊查询  | `LIKE` + `%`、`_`          | `name LIKE 'A%'`                | `%`匹配多个，`_`匹配一个    |
| 范围查询  | `BETWEEN ... AND ...`     | `salary BETWEEN 3000 AND 6000`  | 包含边界值              |
| 集合查询  | `IN (...)`                | `dept IN ('HR','IT')`           | 等价于多个 `OR`         |
| 空值判断  | `IS NULL / IS NOT NULL`   | `phone IS NULL`                 | 不能用 `= NULL`       |
| 排序    | `ORDER BY ASC/DESC`       | `ORDER BY salary DESC`          | ASC 升序（默认），DESC 降序 |

---

## DQL-分组查询
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6859b47d93554c9fb730447040c78be7.png)
### 聚合函数
我们来讲解 **SQL 分组查询（GROUP BY）中的聚合函数**，这是 DQL 的核心功能之一，尤其在统计和报表场景中非常常用。

---

#### 1️⃣ 聚合函数概述

聚合函数用于 **对一组数据进行计算**，返回单个值。常用的聚合函数包括：

| 聚合函数      | 功能   | 示例                     |
| --------- | ---- | ---------------------- |
| `COUNT()` | 统计行数 | `COUNT(*)`、`COUNT(id)` |
| `SUM()`   | 求和   | `SUM(salary)`          |
| `AVG()`   | 平均值  | `AVG(score)`           |
| `MAX()`   | 最大值  | `MAX(age)`             |
| `MIN()`   | 最小值  | `MIN(score)`           |

> 注意：聚合函数常与 `GROUP BY` 结合，用于按组统计。

---

#### 2️⃣ 分组查询语法

```sql
SELECT 字段1, 聚合函数(字段2)
FROM 表名
WHERE 条件
GROUP BY 字段1
HAVING 聚合条件
ORDER BY 排序字段;
```

* `GROUP BY`：指定按哪个字段分组
* `HAVING`：对分组结果进行条件过滤（类似 WHERE，但作用于分组后的结果）
* `ORDER BY`：排序

---

#### 3️⃣ 示例案例

假设有一个 **学生成绩表 `students`**：

| id | name | class | score |
| -- | ---- | ----- | ----- |
| 1  | 张三   | 1     | 85    |
| 2  | 李四   | 1     | 90    |
| 3  | 王五   | 2     | 78    |
| 4  | 赵六   | 2     | 88    |
| 5  | 小明   | 1     | 92    |

---

##### （1）统计每个班级的人数

```sql
SELECT class, COUNT(*) AS student_count
FROM students
GROUP BY class;
```

结果：

| class | student\_count |
| ----- | -------------- |
| 1     | 3              |
| 2     | 2              |

---

##### （2）统计每个班级的总分

```sql
SELECT class, SUM(score) AS total_score
FROM students
GROUP BY class;
```

结果：

| class | total\_score |
| ----- | ------------ |
| 1     | 85+90+92=267 |
| 2     | 78+88=166    |

---

##### （3）统计每个班级的平均分

```sql
SELECT class, AVG(score) AS avg_score
FROM students
GROUP BY class;
```

结果：

| class | avg\_score |
| ----- | ---------- |
| 1     | 89         |
| 2     | 83         |

---

##### （4）查询每个班级的最高分

```sql
SELECT class, MAX(score) AS max_score
FROM students
GROUP BY class;
```

结果：

| class | max\_score |
| ----- | ---------- |
| 1     | 92         |
| 2     | 88         |

---

##### （5）结合 HAVING 过滤

查询 **平均分大于 85 的班级**：

```sql
SELECT class, AVG(score) AS avg_score
FROM students
GROUP BY class
HAVING AVG(score) > 85;
```

结果：

| class | avg\_score |
| ----- | ---------- |
| 1     | 89         |

---

#### 4️⃣ 总结表格

| 聚合函数     | 功能   | 用法示例                   | 注意事项                                          |
| -------- | ---- | ---------------------- | --------------------------------------------- |
| COUNT()  | 统计行数 | `COUNT(*)`、`COUNT(id)` | `COUNT(*)` 统计总行数，包括 NULL；`COUNT(列名)` 不统计 NULL |
| SUM()    | 求和   | `SUM(score)`           | 字段必须是数值类型                                     |
| AVG()    | 平均值  | `AVG(score)`           | 字段必须是数值类型                                     |
| MAX()    | 最大值  | `MAX(score)`           | 可用于数值、字符串、日期类型                                |
| MIN()    | 最小值  | `MIN(score)`           | 可用于数值、字符串、日期类型                                |
| GROUP BY | 分组统计 | `GROUP BY class`       | 所有非聚合字段必须在 GROUP BY 中                         |
| HAVING   | 分组条件 | `HAVING AVG(score)>85` | 作用于分组后的结果，不能用 WHERE 替代                        |


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9d987148fe1648bb84b5f7750f40a72c.png)

---

### 分组查询
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fc8f49c49ef348c895a0edcc717194ad.png)

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/16ed8d77756547b3baf8efd161932e15.png)
好的，我们来详细讲解 **SQL 分组查询语法**：

---

#### 1️⃣ 语法结构

```sql
SELECT 字段列表
FROM 表名
[WHERE 条件列表]
GROUP BY 分组字段名
[HAVING 分组后过滤条件];
```

##### 组成部分说明

| 关键字        | 作用       | 说明                     |
| ---------- | -------- | ---------------------- |
| `SELECT`   | 指定查询哪些字段 | 可以是普通字段，也可以是聚合函数       |
| `FROM`     | 指定数据来源表  | 必填                     |
| `WHERE`    | 行过滤条件    | 在分组前对行进行筛选（可选）         |
| `GROUP BY` | 分组字段     | 按指定字段把数据分成若干组，每组作为一个整体 |
| `HAVING`   | 分组后过滤    | 对分组后的结果进行条件筛选（可选）      |

---

#### 2️⃣ 执行顺序（注意理解顺序）

1. **FROM**：从表中获取数据
2. **WHERE**：对行进行过滤（分组前）
3. **GROUP BY**：按指定字段分组
4. **聚合函数计算**：对每组应用 COUNT、SUM、AVG、MAX、MIN 等聚合函数
5. **HAVING**：对分组后的结果进行过滤
6. **SELECT**：返回查询字段
7. **ORDER BY**（如果有）：对结果排序

> ⚠️ 注意：`WHERE` 作用于 **分组前的行**，`HAVING` 作用于 **分组后的结果**。

---

#### 3️⃣ 示例

假设有一个学生成绩表 `students`：

| id | name | class | score |
| -- | ---- | ----- | ----- |
| 1  | 张三   | 1     | 85    |
| 2  | 李四   | 1     | 90    |
| 3  | 王五   | 2     | 78    |
| 4  | 赵六   | 2     | 88    |
| 5  | 小明   | 1     | 92    |

---

##### （1）基础分组查询：按班级统计人数

```sql
SELECT class, COUNT(*) AS student_count
FROM students
GROUP BY class;
```

结果：

| class | student\_count |
| ----- | -------------- |
| 1     | 3              |
| 2     | 2              |

---

##### （2）分组 + WHERE：只统计成绩大于80的学生

```sql
SELECT class, COUNT(*) AS student_count
FROM students
WHERE score > 80
GROUP BY class;
```

结果：

| class | student\_count |
| ----- | -------------- |
| 1     | 3              |
| 2     | 1              |

> ⚠️ 这里 `WHERE` 先筛掉分数 ≤ 80 的行，再分组。

---

##### （3）分组 + HAVING：只保留平均成绩大于85的班级

```sql
SELECT class, AVG(score) AS avg_score
FROM students
GROUP BY class
HAVING AVG(score) > 85;
```

结果：

| class | avg\_score |
| ----- | ---------- |
| 1     | 89         |

> ⚠️ `HAVING` 是 **分组后的过滤**，可以用聚合函数条件。

---

##### （4）总结要点

| 部分       | 用法                        | 注意事项                     |
| -------- | ------------------------- | ------------------------ |
| WHERE    | 分组前过滤行                    | 不能使用聚合函数                 |
| GROUP BY | 指定分组字段                    | 非聚合列必须在 GROUP BY 中或用聚合函数 |
| HAVING   | 分组后过滤结果                   | 可以使用聚合函数，如 AVG、SUM、COUNT |
| SELECT   | 返回字段                      | 可以是普通字段或聚合结果             |
| 聚合函数     | COUNT, SUM, AVG, MAX, MIN | 对每组数据进行统计计算              |

---

✅ 小结：

1. **WHERE** → 分组前行筛选
2. **GROUP BY** → 按字段分组
3. **聚合函数** → 对每组统计
4. **HAVING** → 分组后结果筛选
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/46f7db9b092c4ae1bdd9a69234899068.png)

---

## DQL-排序查询
 ![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b0d8611d01de49e28b591d5b4250e5f5.png)
好，这里我们来详细讲解一下 **排序查询（ORDER BY）**，它是 DQL（数据查询语言）中非常常用的一个功能。

---

### 1️⃣ 排序查询语法

```sql
SELECT 字段列表
FROM 表名
[WHERE 条件列表]
[GROUP BY 分组字段名 HAVING 分组后过滤条件]
ORDER BY 排序字段 [ASC|DESC];
```

---

### 2️⃣ 关键部分解释

| 关键字        | 作用       | 说明                   |
| ---------- | -------- | -------------------- |
| `ORDER BY` | 排序关键字    | 必须放在语句最后             |
| `排序字段`     | 用来排序的字段  | 可以是表字段，也可以是别名，甚至是表达式 |
| `ASC`      | 升序排列（默认） | 从小到大，从旧到新            |
| `DESC`     | 降序排列     | 从大到小，从新到旧            |

---

### 3️⃣ 执行顺序复习

SQL 的大致执行顺序是：

1. **FROM** → 选择数据来源
2. **WHERE** → 过滤行
3. **GROUP BY** → 分组
4. **HAVING** → 分组后过滤
5. **SELECT** → 选择要展示的列
6. **ORDER BY** → 排序
7. **LIMIT**（如果有） → 限制返回结果

👉 可以看到，`ORDER BY` 一定是最后执行的。

---

### 4️⃣ 示例案例

假设有一个成绩表 `students`：

| id | name | class | score |
| -- | ---- | ----- | ----- |
| 1  | 张三   | 1     | 85    |
| 2  | 李四   | 1     | 90    |
| 3  | 王五   | 2     | 78    |
| 4  | 赵六   | 2     | 88    |
| 5  | 小明   | 1     | 92    |

---

#### （1）单字段排序：按成绩升序

```sql
SELECT name, score
FROM students
ORDER BY score ASC;
```

👉 从低到高排列分数。

---

#### （2）单字段排序：按成绩降序

```sql
SELECT name, score
FROM students
ORDER BY score DESC;
```

👉 从高到低排列分数。

---

#### （3）多字段排序：先按班级升序，再按成绩降序

```sql
SELECT name, class, score
FROM students
ORDER BY class ASC, score DESC;
```

👉 结果会先按班级分组显示，班级内再按成绩从高到低排列。

---

#### （4）结合分组：统计每个班级的平均分，并按平均分降序

```sql
SELECT class, AVG(score) AS avg_score
FROM students
GROUP BY class
ORDER BY avg_score DESC;
```

👉 结果按每个班级的平均分排序。

---

### 5️⃣ 总结表格

| 部分       | 用法                    | 注意事项                              |
| -------- | --------------------- | --------------------------------- |
| ORDER BY | 排序关键字                 | 必须放在最后（LIMIT 之前）                  |
| ASC      | 升序（默认）                | 小→大，旧→新                           |
| DESC     | 降序                    | 大→小，新→旧                           |
| 多字段排序    | `ORDER BY 字段1, 字段2`   | 先按字段1排序，再按字段2排序                   |
| 聚合结果排序   | `ORDER BY AVG(score)` | 可以对聚合函数结果排序                       |
| 别名排序     | `ORDER BY 别名`         | 例如 `SELECT score AS s ORDER BY s` |

---

✅ 小结：
排序查询用 `ORDER BY`，默认升序 `ASC`，可选降序 `DESC`。支持多字段排序，还能对聚合结果或别名排序。

---

## DQL-分页查询
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b721f5f0b2524f2ab79dee2647b7d5c1.png)
好，这里我们在 **排序查询** 的基础上，再加上 **LIMIT** 子句来控制结果集的数量和起始位置。

---

### 1️⃣ 完整语法

```sql
SELECT 字段列表
FROM 表名
[WHERE 条件]
[GROUP BY 分组字段 HAVING 分组后过滤条件]
[ORDER BY 排序字段 ASC|DESC]
[LIMIT 起始索引, 查询记录数];
```

---

### 2️⃣ 关键部分解释

| 关键字               | 作用                 | 说明                       |
| ----------------- | ------------------ | ------------------------ |
| `ORDER BY`        | 对结果排序              | 默认 `ASC` 升序，可用 `DESC` 降序 |
| `LIMIT n`         | 限制返回 n 条记录         | 常用于只看部分数据                |
| `LIMIT offset, n` | 从 offset 开始，取 n 条  | `offset` 从 0 开始计数        |
| **结合使用**          | `ORDER BY + LIMIT` | 常用于分页、排行榜等场景             |

---

### 3️⃣ 示例案例

假设有一个学生成绩表 `students`：

| id | name | class | score |
| -- | ---- | ----- | ----- |
| 1  | 张三   | 1     | 85    |
| 2  | 李四   | 1     | 90    |
| 3  | 王五   | 2     | 78    |
| 4  | 赵六   | 2     | 88    |
| 5  | 小明   | 1     | 92    |
| 6  | 小红   | 2     | 95    |

---

#### （1）查询前 3 名成绩最高的学生

```sql
SELECT name, score
FROM students
ORDER BY score DESC
LIMIT 3;
```

👉 结果：小红(95)，小明(92)，李四(90)

---

#### （2）分页查询：查询第 2 页，每页显示 2 条

```sql
SELECT name, score
FROM students
ORDER BY score DESC
LIMIT 2, 2;
```

👉 `LIMIT 2, 2` = 从第 3 条开始（偏移量 2），取 2 条。
结果：张三(85)，王五(78)

---

#### （3）分组 + 排序 + 限制：查询平均成绩最高的 1 个班级

```sql
SELECT class, AVG(score) AS avg_score
FROM students
GROUP BY class
ORDER BY avg_score DESC
LIMIT 1;
```

👉 结果：返回平均分最高的班级。

---

### 4️⃣ 总结表格

| 子句              | 用法                                                           | 注意事项                |
| --------------- | ------------------------------------------------------------ | ------------------- |
| ORDER BY        | 对结果排序                                                        | 默认升序 ASC，可改为 DESC   |
| LIMIT n         | 返回前 n 条记录                                                    | 从第 1 行开始            |
| LIMIT offset, n | 从 offset 处取 n 条                                              | offset 从 0 开始计数     |
| WHERE           | 分组前行过滤                                                       | 不允许聚合函数             |
| GROUP BY        | 按字段分组                                                        | 非聚合字段必须在 GROUP BY 中 |
| HAVING          | 分组后过滤                                                        | 可以使用聚合函数            |
| 执行顺序            | FROM → WHERE → GROUP BY → HAVING → SELECT → ORDER BY → LIMIT | LIMIT 总是最后执行        |

---

✅ 小结：

* **ORDER BY** 决定排序方式；
* **LIMIT** 控制返回数量；
* 两者结合常用于 **分页** 和 **排行榜**。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a5bb03f463b407198e35028e39452d9.png)

---


