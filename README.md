# <center>前端规范文档
## 索引
  - 规范
  - 风格
  - 模块化工具
  - 构建工具
  - 项目目录结构
  - 单页web框架的选定
  - 其他较常用的插件选定
  - UI框架的可选项了解
  - 文档链接
  - 学习书籍推荐

## 一、规范
* ### HTML

* ### CSS

* ### JavaScript

1. 4个字符缩进；
2. 使用单引号；
3. 使用严格模式；
4. 声明提前；
5. 换行：
	- json风格数组对象元素之间换行；
	- 逻辑运算符太多时换行；
	- 方法之间换行；
	- 语句块之间换行；
6. 空格：
	- `=`、`==`、`===`两边空格；
	- 属性冒号后空格；
	- 条件语句保留字后空格；
	- 逻辑运算符前后空格；


	
	```javascript
	function func() {
		'use strict';
		
		if (bar && baz) {
			var obj = {
				foo: 'name',
				
				func1: function () {
					// 代码
				},
				
				func2: function () {
					// 代码
				}
			};
			
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
	-
	-
	

## 二、风格
  - 说明：风格不强制要求，只作参考
  - css命名：
    - 名字拼接用 **-** *（中划线）*
    - 表示上下层级用 **__** *(两个下划线)*
    - 表示状态用 **--** *(两个中划线)*
    - 例子： ```home-header__banner--active```
  - js命名
    - 局部变量用下划线拼接单词 **_** *（下划线）*；
    - 全局变量用驼峰拼接单词 **-** *(中划线)*；
    - 名字最后方便可以加上预期的数据类型，如configMap, elt_list, elt_str等；
    - 例子：

```
    var configMap = {...};
    var str = 'name';
    
    function (...) {
        var config_map = {...};
    }
```

## 三、模块化工具
  - 使用*AMD规范*的[require.js](http://requirejs.org/)作为前端模块化库

## 四、构建工具
  - 使用[gulp](http://www.gulpjs.com.cn/)前端构建工具

## 五、项目目录结构
暂时参考 [angularJs项目实战！01：模块划分和目录组织](http://www.angularjs.cn/A08q)
后续可考虑Yoeman的目录结构


## 六、单页web框架的选定
  - [Angular.js](https://docs.angularjs.org/api)
  - 版本： v1.3.9

## 七、其他较常用的插件/工具选定
  - css预编译器：sass
  - 滑动（slider）插件，选用 [**Swiper**](http://www.swiper.com.cn/), [Swiper API](http://www.swiper.com.cn/api/index.html)
  - 调试微信功能工具，选用 [**微信web开发者工具**](http://mp.weixin.qq.com/wiki/10/e5f772f4521da17fa0d7304f68b97d7e.html)

## 八、UI框架的可选项了解
  - [微信UI--weui](http://mp.weixin.qq.com/wiki/2/ae9782fb42e47ad79eb7b361c2149d16.html)

## 九、文档链接
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

## 十、学习书籍推荐
  - 《AngularJS权威指南》
  - 《精通AngularJS》

## 十一、学习网站
  - [thinkster](https://thinkster.io/a-better-way-to-learn-angularjs)
  - [AngularJS入门教程](http://www.ituring.com.cn/minibook/303)
  - [Angular中文文档](http://docs.ngnice.com/guide)
  - [AngularJs Tips](http://angular-tips.com/)
  - [Yeoman 快速教程](http://blog.jobbole.com/65399/)
  - [AngularJS 其他学习资源](http://www.cnblogs.com/hubcarl/p/4207909.html)
  - [AngularJS 学习资源](http://blog.vichamp.com/angularjs/2014/08/02/angularjs-guideline/)