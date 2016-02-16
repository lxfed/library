# <center>前端规范文档
## 索引
  - [规范与风格](#style)
  - [模块化工具](#module)
  - [构建工具](#build)
  - [项目目录结构](#structure)
  - [单页web框架的选定](#spaFramework)
  - [其他较常用的插件选定](#tools)
  - [UI框架的可选项了解](#uiFrame)
  - [文档链接](#doc)
  - [学习书籍推荐](#books)
  - [学习网站](#websites)

## <span id="standard">一、规范与风格</span>
* ### HTML

	- 使用4格缩进；
	- 不要创建无样式信息的`class`，使用`id`和属性作为hook方式；
	- 同一页面避免使用同名`name`和`id`；
	- 对于无需自闭合的标签，不要自闭合；
	
		> 常见无需自闭合标签有input、br、img、hr等。
	- 标签的使用应该遵循标签的语义；
		
		> - p - 段落
		> - h1,h2,h3,h4,h5,h6 - 层级标题
		> - strong,em - 强调
		> - ins - 插入
		> - del - 删除
		> - abbr - 缩写
		> - code - 代码标识
		> - cite - 引述来源作品的标题
		> - q - 引用
		> - blockquote - 一段或长篇引用
		> - ul - 无序列表
		> - ol - 有序列表
		> - dl,dt,dd - 定义列表
	- 属性名使用小写字母；
	- 使用 HTML5 的`doctype`来启用标准模式，建议使用大写的`DOCTYPE`；
	- 在 html 标签上设置正确的 lang 属性：
	
		```html 
		<html lang="zh-CN">
		```
	- HTML 文件使用无 BOM 的 UTF-8 编码；
	- 布尔类型的属性，建议不添加属性值，例如： 
	
		```html
		<input type="text" disabled>
		<input type="checkbox" value="1" checked>
		```
	
参考CSS命名规范

* ### CSS

	使用[BEM](https://en.bem.info/)。
	
	了解更多：
	
	[如何看待 CSS 中 BEM 的命名方式？［知乎］](https://www.zhihu.com/question/21935157)
	
	[BEM教程](http://www.w3cplus.com/css/css-layers.html)


* ### JavaScript

	- 使用4格缩进；
	- 使用单引号；
	- 使用严格模式；
	- 声明提前；
	- 局部变量用下划线拼接单词 *（例如：`temp_data`）*；
	- 全局变量用驼峰拼接单词 *(例如：`getName`)*；
	- 名字最后方便可以加上预期的数据类型，如configMap, elt_list, elt_str等；
	- 换行：
		- json风格数组对象元素之间换行；
		- 逻辑运算符太多时换行；
		- 方法之间换行；
		- 语句块之间换行；
	- 空格：
		- `=`、`==`、`===`两边空格；
		- 属性冒号后空格；
		- 条件语句保留字后空格；
		- 逻辑运算符前后空格；
	- 字符串拼接使用数组和其方法`join`转换；


	**代码范例**：
	
	```javascript
	var configMap = {...},
		str = 'name',
		data = [
			{
				a: '1'
			},
			{
				b: '2'
			}
		],
		htmlStr = [
			'<input type="text" disabled>',
			'<input type="checkbox" value="1" checked>'
		].join('');
    
	function func() {
		'use strict';
		
		var obj = {
			foo: 'name',
				
			func1: function () {
				// 代码
			},
				
			func2: function () {
				// 代码
			}
		};
		
		if (bar && baz) {
			obj = {};
					
			switch (baz) {
				case '1':
				case '2':
				// 代码
				break;
				
				case '3':
				// 代码
				break;
				
				default:
				break;
			}
		} else {
			// 代码
		}
	}
	```

## 二、<span id="module">模块化工具</span>
  - 使用*AMD规范*的[require.js](http://requirejs.org/)作为前端模块化库

## 三、<span id="build">构建工具</span>
  - 使用[gulp](http://www.gulpjs.com.cn/)前端构建工具

## 四、<span id="structure">项目目录结构</span>
暂时参考 [angularJs项目实战！01：模块划分和目录组织](http://www.angularjs.cn/A08q)
后续可考虑Yoeman的目录结构


## 五、<span id="spaFramework">单页web框架的选定</span>
  - [Angular.js](https://docs.angularjs.org/api)
  - 版本： v1.3.9

## 六、<span id="tools">其他较常用的插件/工具选定</span>
  - css预编译器：sass
  - 滑动（slider）插件，选用 [**Swiper**](http://www.swiper.com.cn/), [Swiper API](http://www.swiper.com.cn/api/index.html)
  - 调试微信功能工具，选用 [**微信web开发者工具**](http://mp.weixin.qq.com/wiki/10/e5f772f4521da17fa0d7304f68b97d7e.html)

## 七、<span id="uiFrame">UI框架的可选项了解</span>
  - [微信UI--weui](http://mp.weixin.qq.com/wiki/2/ae9782fb42e47ad79eb7b361c2149d16.html)

## 八、<span id="doc">文档链接</span>
  - **Angular.js**
    - [官方API](https://docs.angularjs.org/api)
    - [中文API](http://docs.angularjs.cn/api)
  - **Gulp**: 
    - [官网](http://www.gulpjs.com.cn/)
    - [入门](http://www.gulpjs.com.cn/docs/getting-started/)
  - **Swiper**
    - [Swiper](http://www.swiper.com.cn/) 
    - [API](http://www.swiper.com.cn/api/index.html)
  - 微信相关   
    - [**微信web开发者工具**](http://mp.weixin.qq.com/wiki/10/e5f772f4521da17fa0d7304f68b97d7e.html)
    - [**微信JS-SDK**](http://mp.weixin.qq.com/wiki/11/74ad127cc054f6b80759c40f77ec03db.html)
    - [微信UI--weui](http://mp.weixin.qq.com/wiki/2/ae9782fb42e47ad79eb7b361c2149d16.html), [github链接](https://github.com/weui/weui)
  - [require.js]
    - [官网](http://requirejs.org/)
    - [API](http://requirejs.org/docs/api.html)
    - [入门指南](http://www.gulpjs.com.cn/docs/getting-started/)

## 九、<span id="books">学习书籍推荐</span>
  - 《AngularJS权威指南》
  - 《精通AngularJS》

## 十、<span id="websites">学习网站</span>
  - [thinkster](https://thinkster.io/a-better-way-to-learn-angularjs)
  - [AngularJS入门教程](http://www.ituring.com.cn/minibook/303)
  - [Angular中文文档](http://docs.ngnice.com/guide)
  - [AngularJs Tips](http://angular-tips.com/)
  - [Yeoman 快速教程](http://blog.jobbole.com/65399/)
  - [AngularJS 其他学习资源](http://www.cnblogs.com/hubcarl/p/4207909.html)
  - [AngularJS 学习资源](http://blog.vichamp.com/angularjs/2014/08/02/angularjs-guideline/)