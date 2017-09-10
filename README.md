# Nodejs与git安装与配置(2017-09-11)

## Nodejs

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

## git

1. 任何位置右键，选中 `Git Gui Here`
2. `Help` ---  `show ssh ke`
3. `generate key` -- key is empty
4. 复制到GitHub，添加Title -- add ssh key
5. 进入`C:\Users\Administrator\.ssh`文件夹找到ssh文件
6. 使用`PuTTYgen`创建私钥
    1. `load`
    2. 打开`C:\Users\Administrator\.ssh`
    3. 选择`all Files`
    4. 打开`id_rsa`
    5. 重命名`key comment`: `v480s`
    6. save privite key
    7. 重命名 `v480s.ppk`
7. github上新建仓库
8. 使用ssh协议
9. 进入项目文件夹
10. vscode关联远程仓库
```
git remote add origin __URL__
```
11. 第一次使用ssh key需要手动使用cmd进行推送
```
git push -u origin master
```