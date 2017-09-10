# Nodejs安装步骤(2017-09-11)

1. instill nodejs
2. mkdir `node_cache`, `node_global`
3. 配置路径
```
npm config set prefix "__DIR__/node_global"
npm config set cache "__DIR__/node_cache"
```
4. cmd npm 查看安装是否成功
```
npm
```
5. 配置全局环境变量: `__DIR__/node_global;`
6. 安装cnpm
```
npm install -g cnpm --registry=https://registry.npm.taobao.org
```
7. 检查cnpm是否安装成功
```
cnpm
```
8. 安装vscode插件: `ESLint`
9. 全局安装npm模块`ESLint`
```
npm install -g eslint
```
10. 新建项目文件夹，进入文件夹  
vscode进入终端快捷键Ctrl+`
11. 初始化eslint配置
```
eslint --init

? How would you like to configure ESLint?
Answer questions about your style
? Are you using ECMAScript 6 features?
Yes
? Are you using ES6 modules?
Yes
? Where will your code run?
Browser, Node
? Do you use CommonJS?
Yes
? Do you use JSX?
No
? What style of indentation do you use?
Tabs
? What quotes do you use for strings?
Double
? What line endings do you use?
Windows
? Do you require semicolons?
Yes
? What format do you want your config file to be in?
JavaScript
```
12. vscode自动格式化代码快捷键`Ctrl + Shift + F`
