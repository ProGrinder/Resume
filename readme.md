# Resume

## Introduction

简历为仿写，原简历页面地址: [张秋怡 - 个人简历](https://joyeecheung.github.io/resume/) 【原主人已删除】

- 简历基于 Gulp+Scss+Jade。  
- 访问地址：[Lxxyx 的简历](https://resume.lxxyx.cn)



在原作者的基础上，修改了package.json，使gulp3和npm12能共用。

## 配置

将该项目下载到本地【git clone】或下载.zip解压

- Step1: 全局安装gulp

```
npm install -g gulp
```

- Step2:在项目根路径下安装puppeteer【有点久，耐心等待】

推荐使用淘宝chromium源安装，保证网络速度

```
npm config set puppeteer_download_host=https://npm.taobao.org/mirrors
npm i puppeteer
```

安装完puppeteer后

```
npm install
```

## 使用

### 编辑

修改info.json

待摸索

### 运行

项目根路径下:

```
npm pdf
```

在部署网页文件档 dist 中生成 PDF 的命令：

```
npm run pdf
```



本地部署

1. `npm install gulp --save-dev`
2. `npm install gulp-webserver --save-dev`
3. `gulp webserver`

即可以本地离线形式访问简历，默认访问端口为localhost:9000, 打印端口为9001



需要自动部署的，运行`gulp deploy`即可，需要在 gulpfile 中更改为你的地址（！会抹去你 github pages 内容，慎用！）

__注__：

生成的pdf可能会出现没有字体图标的问题

推荐使用chrome浏览器自带的打印机：

使用高级设置调整纸张大小，缩放比例，保持1页pdf效果最佳。



### 自定义域名

修改 CNAME 文件，替换为你的域名即可
