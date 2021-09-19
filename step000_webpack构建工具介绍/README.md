## 前端构建工具

### webpack
* 理解
```
webpack是一个静态的模块化文件的前端构建工具，

它可以将各类js、css、png等文件进行组装打包，

然后交付给浏览器直接使用。

它依赖于node环境！！！

而前端模块化、工程化的基础大部分都基于node环境！

而node环境是基于commonjs规范的，

所以webpack相关配置也是采用commonjs规范的语法。
```
* 安装

```
1. 全局安装
npm install webpack webpack-cli -g
2. 局部安装
npm install webpack webpack

注意事项：
1. webpack的安装和使用一般需要用到webpack-cli，
否则会报错，
为了正常使用webpack通常都会同时安装webpack-cli 。

2. 当局部安装webpack时，
若不借助webstorm等IDE在项目路径下打开终端，
则无法直接使用webpack命令，
因为它只会从全局去找webpack命令（ubuntu下亲测结论），
此时想在终端使用webpack命令的话，
一是使用npx webpack xxx，
它会首先去项目路径下找webpack命令，
找不到才去找全局的webpack，
所以适用局部安装webpack的使用。
二是把局部安装的webpack指明具体命令路径，
该路径是./node_modules/.bin/webpack 。
执行webpack之后，
它默认会在当前路径下以 ./src/index.js 为入口文件进行js的打包编译，
以 ./dist/ 为输出目录(可自行定义或更改)！！！
以 main.js 为js输出文件名（暂未找到可更改的方法）！！！

若要自定义入口文件名和输出目录，
需要配置命令参数，如： npx webpack --entry ./src/main.js -o ./build 

```

* 配置及使用
```
在安装步骤中已介绍过在终端使用webpack的基本命令，
但webpack的高级用法一般都在配置文件中进行配置。
该配置文件默认名为 webpack.config.js ，
若要自定义配置文件名需在终端添加参数 webpack --config filename 。
具体文件中的一些配置选项，
请查询官网！
```
