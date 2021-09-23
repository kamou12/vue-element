<p align="center">
  <img width="320" src="https://wpimg.wallstcn.com/ecc53a42-d79b-42e2-8852-5126b810a4c8.svg">
</p>

<p align="center">
  <a href="https://github.com/vuejs/vue">
    <img src="https://img.shields.io/badge/vue-2.6.10-brightgreen.svg" alt="vue">
  </a>
  <a href="https://github.com/ElemeFE/element">
    <img src="https://img.shields.io/badge/element--ui-2.7.0-brightgreen.svg" alt="element-ui">
  </a>
  <a href="https://travis-ci.org/PanJiaChen/vue-element-admin" rel="nofollow">
    <img src="https://travis-ci.org/PanJiaChen/vue-element-admin.svg?branch=master" alt="Build Status">
  </a>
  <a href="https://github.com/PanJiaChen/vue-element-admin/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/mashape/apistatus.svg" alt="license">
  </a>
  <a href="https://github.com/PanJiaChen/vue-element-admin/releases">
    <img src="https://img.shields.io/github/release/PanJiaChen/vue-element-admin.svg" alt="GitHub release">
  </a>
  <a href="https://gitter.im/vue-element-admin/discuss">
    <img src="https://badges.gitter.im/Join%20Chat.svg" alt="gitter">
  </a>
  <a href="https://panjiachen.gitee.io/vue-element-admin-site/zh/donate">
    <img src="https://img.shields.io/badge/%24-donate-ff69b4.svg" alt="donate">
  </a>
</p>

## 一、简介

vue-element-admin 是一个后台前端解决方案，它基于 vue 和 element-ui实现。它使用了最新的前端技术栈，内置了 i18n 国际化解决方案，动态路由，权限验证，提炼了典型的业务模型，提供了丰富的功能组件，它可以帮助你快速搭建企业级中后台产品原型。相信不管你的需求是什么，本项目都能帮助到你。

### **最佳实践**

1.1 vue-element-admin 的本地开发

```bash
# 克隆项目
git clone https://github.com/PanJiaChen/vue-element-admin.git

# 进入项目目录
cd vue-element-admin

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装依赖，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 http://localhost:9527

1.2 vue-element-admin的线上网站发布

见下一章。

## 二、将vue-element-admin项目通过云开发平台，快速发布为网站

### **背景介绍**
云开发平台是阿里云面向广大开发者提供的免费云上研发工作平台，可以实现开发的全流程。关于云开发平台的介绍：https://help.aliyun.com/product/161245.html。

### **最佳实践**

**1.创建vue-element-admin代码项目**

直接fork本项目到自己的GitHub账号下。

**2.打开云开发平台，完成阿里云账号注册登陆，同意云开发平台服务协议** https://workbench.aliyun.com/application

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/sign.png" width="400">

**3.创建云开发平台-前端部署应用**

3.1 创建前端应用

依次点击「应用列表」「前端应用」「新建前端应用」按钮。首先绑定GitHub帐号，允许云开发平台构建、发布你的GitHub代码为可访问的网站。

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/create_0.png" width="200">

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/oauth.png" width="200">

选择第一步中的代码仓库、主干分支等，并点击下一步。主干分支一般指的是代码的master或main等分支。

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele1.png" width="300">

填写基本信息并点击「完成」。稍等片刻创建成功后，将进入到应用部署界面。

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele2.png" width="600">

3.2 开发部署配置

填写日常/线上环境的部署配置
按照"?"提示，依次填写部署配置信息。其中：
- 本项目资源路径应填写为"./website/dist",因为本项目静态资源默认存储在根目录下的website文件夹中的dist文件夹中

- 如需使用自定义域名访问，可将自定义域名填入对应位置，并在部署成功后，根据步骤3.4进行域名解析后实现自定义域名访问</br>
  <img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele3.png" width="400">

3.3 进行项目的部署和查看

依次点击「部署」「确定」，即可启动日常/线上环境的发布流程。对于每个代码分支，要求先发布日常环境，再发布线上。若不需多套环境，则可以只使用日常环境，或者发布一次日常环境后，仅使用线上环境即可。

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/deploy.png" width="300">

3.3.1 部署完成，查看部署结果

访问**测试域名**或者**自定义域名**，以下以测试域名为例

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele4.png" width="650">

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele5.png" width="650">

3.3.2 在部署完成后，部署状态会显示为“已部署”。且部署网站的记录和过程，也会被完整记录下来：

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/docs/create4.png" width="600">

3.3.3可点击部署记录的「查看结果」来查看部署到OSS存储中的静态资源。

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele6.png" width="400">

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/result_download.png" width="350">

3.3.4 可点击部署记录的「查看日志」查看部署的详细过程，并在部署发生错误时，精确定位学习错误情况。

<img src="https://readme-img-2.oss-us-west-1.aliyuncs.com/feApp/github/vue_element/vue_ele7.png" width="400">

部署操作可以在每次更新内容并push后再次进行，实现静态网站内容的按需实时更新。

3.4 将OSS存储中的项目发布为网站链接

3.4.1 解析自己的域名到OSS Bucket的访问域名上

打开自己域名的DNS解析控制台，使用阿里云域名或其它提供商的域名均可，此处以阿里云为例：

首先，找到自己要解析的域名，添加/修改一条解析记录：

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/cname.png" width="650">

如下图所示，配置CNAME、自己的域名、记录值：

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/cname_2.png" width="400">

记录值查看方法示意图：

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/oss_domain.png" width="600">

完成配置后，稍等片刻，确定使用https://zijian.aliyun.com/ ，或者ping/dig/nslookup等指令可以查找到本域名的解析情况。

3.4.2 当URL仅访问目录而非目录下的HTML文件时，由OSS托管路由自动定向至目录下的指定HTML文件

某些前端项目生成的静态代码，其HTML中嵌入的链接地址是不含index.html的。这要求放置HTML文件的存储，或NGINX服务器等，有将裸访问路径自动对应到具体HTML文件的能力。

OSS Bucket具有该托管能力，需要在使用的OSS Bucket内，选择「基础设置」「静态页面」，并如下图所示，填写默认首页为index.html，开通子目录首页功能，并点击「保存」。

<img src="https://ecoboost-readme-image.oss-cn-shanghai.aliyuncs.com/feApp/github/hexo/oss_index.png" width="350">

3.5 （可选）使用CDN加速域名访问，节约流量费用

可点击「部署配置」中的「如何配置CDN加速」，将自己的域名与CDN加速绑定，从而加速网站访问。
