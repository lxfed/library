# Yeoman + Angular用法小结

## 安装
```cmd
npm install -g grunt-cli bower yo generator-karma generator-angular
```

## 使用
1. 生成App项目目录
    - ``` yo angular [app-name] ```
    - 参数 --appPath： 生成客户端文件到指定目录
2. 生成器的使用
    - 语法： ``` yo angular:[generator-type] [name-generated] ```
    - angular = angular:app
    - angular:controller
        - 生成 *app/scripts/controllers/xxx.js*
    - angular:directive
        - 生成 *app/scripts/directives/xxx.js*
    - angular:filter
        - 生成 *app/scripts/filters/xxx.js*
    - angular:route
        - 可选参数： --uri=my/route
        - 自动配置 *app/scripts/app.js* 下路由
        - 生成 *app/scripts/controllers/xxx.js*
        - 生成 *app/views/xxx.html*
    - angular:service、 angular:provider、angular:factory、angular:value、angular:constant
        - 生成 *app/scripts/services/xxx.js*
    - angular:decorator
        - 生成 *app/scripts/decorators/xxxDecorator.js*
    - angular:view
        - 生成 *app/views/xxx.html*
3. Options
  - --coffee 生成coffee的.coffee文件
  - --typescript 生成typescript的.ts文件
  - --skip-add 跳过添加生成文件到index.html