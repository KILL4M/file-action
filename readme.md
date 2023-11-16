一 功能

文件上传下载 包括前后端 前端vue2 后端nodejs

二 运行

1) 切换源 安装依赖

nrm use tb  => npm切换到淘宝源

pnpm i => pnpm安装依赖

npm i -g pnpm => 如果pnpm i报错 没有安装pnpm 需要先用npm安装


2) 启动项目

在idea或者vscode中开两个终端 一个终端中运行一个项目 同时启动前端项目和后端项目

pnpm run dev 启动前端项目

pnpm run dev:server 启动后端项目

如果启动失败 可能是版本不对

当前版本:
nodejs: 14.18.2
npm: 6.14.15
pnpm 6.30.1
"axios": "^1.6.0",
"core-js": "^3.6.5",
"element-ui": "^2.15.14",
"express": "^4.18.2",
"fs-extra": "^11.1.1",
"multer": "^1.4.5-lts.1",
"uuid": "^9.0.1",
"vue": "^2.6.11"

3) 查看项目效果

打开浏览器输入终端中前端项目的Local: localhost:8080 就可以看到前端项目的运行效果

打开浏览器输入终端中后端项目的Local: localhost:8081 就可以看到后端项目的运行效果 (不需要查看后端项目 前端项目已经实现了文件下载功能)

五 项目打包
4) 打包前端项目

pnpm build

三 项目功能 && 运行效果

具体功能:
1. 多种方式实现文件上传
2. 文件下载
3. 查看已上传文件列表
4. 上传文件大小限制 类型限制 数量限制

前端项目: 点击前端项目终端运行完成生成的url 可以点击选择文件上传文件 然后刷新列表 能看到刚才已经上传的文件 然后点击文件列表中有下划线的部分 就能下载文件
或者复制文件列表中一个文件的前面浅蓝色的部分 放到下面的uuid输入框中 点击下载 就能下载这个文件

后端项目: 后端项目中也有写页面 点击后端项目终端运行完成生成的url 能看到后端项目中写的页面


四 代码解析

后端项目只有一个文件 就是server中的main.js文件

前端项目是除了server文件夹之外的其他文件夹




