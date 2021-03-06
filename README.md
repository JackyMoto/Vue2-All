# Vue2-All
Vue2 + Vue-router2 + Vuex + Webpack + Axios + jwt

采用官方Vue cli脚手架初始项目

目的：一步一步完善项目架构、添加常用组件、代码约束规范、添加常用第三方组件，使之能方便快速构建适合团队开发的项目架构。

下载：git clone https://github.com/liuweijw/Vue2-All.git

切换目录 cd Vue2-All

安装依赖到本地 npm install

运行 npm run dev

本地浏览器查看运行效果 http://localhost:8080

发布运行命令 npm run build

检查且规范代码 npm run lint

查看项目分析 npm run build --report

单元测试 npm run unit

# 学习知识
1、nodejs [docs for nodejs](http://www.runoob.com/nodejs/nodejs-tutorial.html)

2、webpack [guide](http://vuejs-templates.github.io/webpack/)

3、vue2 [guide](https://cn.vuejs.org/v2/guide/index.html)

4、vue-loader [docs for vue-loader](http://vuejs.github.io/vue-loader)

5、vuex [guide](https://vuex.vuejs.org/zh-cn/)

- vue-devtools 很方便的查看vuex，安装方法 [guide](https://github.com/liuweijw/Vue2-All/blob/master/VUE_DEV.md)

6、es6 [guide](http://es6.ruanyifeng.com/)

7、网络请求封装 axios [guide](https://github.com/axios/axios)

8、权限控制 jwt [后台配合springboot工程](https://github.com/liuweijw/fw-framework)

- jwt 不需要的可以跳过

# 开发工具
1、git [guide](http://www.runoob.com/git/git-tutorial.html)

2、vscode [guide](https://code.visualstudio.com/)

- vscode plugin install [guide](https://github.com/liuweijw/Vue2-All/blob/master/VSCODE.md)

# 开发规范

- vscode 开发环境配置更好的匹配eslint规则定义，方便快速开发、修复问题。 用户设置如下：
```
{
    // 自动保存
    "files.autoSave": "onFocusChange",
    // tab 自动缩进2个空格
    "editor.tabSize": 2,
    // 打开同类多个文件
    "workbench.editor.enablePreview": false,
    // Turns auto fix on save on or off.
    "eslint.autoFixOnSave": true,
    // 启用后，保存文件时在文件末尾插入一个最终新行。
    "files.insertFinalNewline": true,
    // 启用后，将在保存文件时剪裁尾随空格。
    "files.trimTrailingWhitespace": true,
    // 采用 atom key 风格
    "atomKeymap.promptV3Features": true,
    "editor.multiCursorModifier": "ctrlCmd",
    "editor.formatOnPaste": true,
    // theme
    "workbench.colorTheme": "One Dark Pro",
    "workbench.iconTheme": "vscode-icons"
}
```
- Eslint 规范定义 [点击查看介绍](.eslintrc.js) 更多的可以自行配置

# 项目待完成
- 集成weex
- 搭建weex-android 和 weex-ios
- 搭建demo工程

# 项目更新说明
- 2017-12-21 初始化项目提交
- 2017-12-25 完成Vue2 + Vue-router2 + Vuex + Webpack + Axios 集成并且配合[服务端](https://github.com/liuweijw/fw-framework)调试OK
- 2017-12-26 至 2017-12-31 集成jwt 并且完成权限验证、路由、登录、登出等功能调试OK。

# 问题和描述
- 使用Visual build软件的时候，编译05版本的VS项目，报错：error MSB3428: 未能加载Visual C++组建"VCBuild.exe"。要解决此问题，1）安装.NET Framework 2.0 SDK；2）安装Microsoft Visual Studio 2005；3）如果将该组件安装到了其他位置，请讲其位置添加到系统路径中；

- 此问题解决： npm install --global --production windows-build-tools  （全局安装windows构建工具）
