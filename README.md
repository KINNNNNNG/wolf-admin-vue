<h1 align="center">Wolf Admin Vue</h1>
<div align="center">
根据<a hreg="https://github.com/sendya/ant-design-pro-vue">ant design pro vue </a>改造成适合的admin后台。
</div>
<!-- 
<div align="center">

[![Backers on Open Collective](https://opencollective.com/ant-design-pro-vue/backers/badge.svg)](#backers) [![Sponsors on Open Collective](https://opencollective.com/ant-design-pro-vue/sponsors/badge.svg)](#sponsors) [![License](https://img.shields.io/npm/l/package.json.svg?style=flat)](https://github.com/sendya/ant-design-pro-vue/blob/master/LICENSE)
[![Release](https://img.shields.io/github/release/sendya/ant-design-pro-vue.svg?style=flat)](https://github.com/sendya/ant-design-pro-vue/releases/latest)
[![Travis branch](https://travis-ci.org/sendya/ant-design-pro-vue.svg?branch=master)](https://travis-ci.org/sendya/ant-design-pro-vue)

</div> -->

<!-- - 预览: https://preview.pro.loacg.com -->
<!-- - 首页: https://pro.loacg.com -->
<!-- - 文档: https://pro.loacg.com/docs/getting-started -->
<!-- - 更新日志: https://pro.loacg.com/docs/changelog -->
<!-- - 常见问题: https://pro.loacg.com/docs/faq -->


概览
----

<!-- 基于 [Ant Design of Vue](https://vuecomponent.github.io/ant-design-vue/docs/vue/introduce-cn/) 实现的 [Ant Design Pro](https://pro.ant.design/) 

![工作台-多标签模式](https://static-2.loacg.com/open/static/github/20190224163345.jpg)

![工作台+设置菜单](https://static-2.loacg.com/open/static/github/20181126112124.png)

![个人设置](https://static-2.loacg.com/open/static/github/20180916-134251.png) -->

暂无

环境和依赖
----

- node
- yarn
- webpack
- eslint
- @vue/cli ~3
- [ant-design-vue](https://github.com/vueComponent/ant-design-vue) - Ant Design Of Vue 实现
- [vue-cropper](https://github.com/xyxiao001/vue-cropper) - 头像裁剪组件
- [@antv/g2](https://antv.alipay.com/zh-cn/index.html) - Alipay AntV 数据可视化图表
- [Viser-vue](https://viserjs.github.io/docs.html#/viser/guide/installation)  - antv/g2 封装实现

> 请注意，我们强烈建议本项目使用 [Yarn](https://yarnpkg.com/) 包管理工具，这样可以与本项目演示站所加载完全相同的依赖版本 (yarn.lock) 。由于我们没有对依赖进行强制的版本控制，采用非 yarn 包管理进行引入时，可能由于 Pro 所依赖的库已经升级版本而引入了新版本所导致的问题。作者可能会由于时间问题无法及时排查而导致您采用本项目作为基项目而出现问题。



项目下载和运行
----

- 拉取项目代码
```bash
git clone https://github.com/KINNNNNNG/wolf-admin-vue
cd wolf-admin-vue
```

- 安装依赖
```
yarn install
```

- 开发模式运行
```
yarn run serve
```

- 编译项目
```
yarn run build
```

- Lints and fixes files
```
yarn run lint
```



其他说明
----

- **关于 Issue 反馈 (重要!重要!重要!) 请在开 *Issue* 前，先阅读该内容：[Issue / PR 编写建议](https://github.com/sendya/ant-design-pro-vue/issues/90)** 

- 项目使用的 [vue-cli3](https://cli.vuejs.org/guide/), 请确保你所使用的 vue-cli 是新版，并且已经学习 cli 官方文档使用教程

- 关闭 Eslint (不推荐) 移除 `package.json` 中 `eslintConfig` 整个节点代码, `vue.config.js` 下的 `lintOnSave` 值改为 `false`

- 开启组件按需加载 `/src/main.js` L14 修改为 `import './core/lazy_use'`

- [修改 Ant Design 配色 (@kokoroli)](https://github.com/kokoroli/antd-awesome/blob/master/docs/Ant_Design_%E6%A0%B7%E5%BC%8F%E8%A6%86%E7%9B%96.md)

- I18n: [多语言支持 (@musnow)](./src/locales/index.js)

- 生成环境默认不加载 `mock`，更多详情请看 `src/mock/index.js`

- **用于生产环境，请使用 `release` 版本代码，使用 master 代码出现的任何问题需要你自行解决**

## 浏览器兼容

Modern browsers and IE10.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png" alt="Opera" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Opera |
| --- | --- | --- | --- | --- |
| IE10, Edge | last 2 versions | last 2 versions | last 2 versions | last 2 versions |

---

## 项目解析

### 文件说明

~/api 请求后端的api

|文件名|说明|
|---|---|
---
~/component 组件文件夹

|文件名|说明|
|---|---|
---
~/layouts 页面布局文件夹

|文件名|说明|
|---|---|
---
~/mock 模拟数据文件夹

|文件名|说明|
|---|---|
---
~/router 路由文件夹

|文件名|说明|
|---|---|
---
~/store Vuex 文件夹

|文件名|说明|
|---|---|
|index.js| Vuex 主文件，使用modules分模块进行状态管理|
---
~/utils 工具类文件夹

|文件名|说明|
|---|---|
---
~/views 页面文件夹

|文件名|说明|
|---|---|


### 流程说明

#### - 登录

* 文件|~/store/modules/user.js
~/api/login.js 
~/mock/service/user.js 模拟数据

|文件名|说明|
|---|---|
|~/views/user/Login.vue|登录页面|
|~/api/login.js |登录api|
|~/store/modules/user.js|stroe user模块 请求api，获取数据后更新token|
|~/mock/service/user.js| |


> user.js:Login() --> 获取后台数据，更新token

<!-- ```flow

st=>start: Login.vue:handleSubmit()
validate=>operation: Login.vue:validateFields()
cond=>condition: user.js:Login()
Suc=>operation: Login.vue:loginSuccess()
Fail=>operation: Login.vue:requestFailed()
e=>end
st->validate->cond
cond(yes)->Suc
cond(no)->Fail
Suc->e
Fail->e
``` -->
![登录流程图](/docs/img/login.svg)