# Vue.js

> Vue.js（读音 /vjuː/, 类似于 view） 是一套构建用户界面的渐进式框架。
>
> Vue 只关注视图层， 采用自底向上增量开发的设计。
>
> Vue 的目标是通过**尽可能简单的 API 实现响应的数据绑定和组合的视图组件**。
>
> Vue 学习起来非常简单，本教程基于 Vue 2.1.8 版本测试。

## 安装

#### 1. 独立版本

我们可以在 Vue.js 的官网上直接下载 vue.min.js 并用 **<script>** 标签引入。

#### 2. 使用CDN

- **BootCDN（国内）** : <https://cdn.bootcss.com/vue/2.2.2/vue.min.js>
- **unpkg**：<https://unpkg.com/vue/dist/vue.js>, 会保持和 npm 发布的最新的版本一致。
- **cdnjs** : <https://cdnjs.cloudflare.com/ajax/libs/vue/2.1.8/vue.min.js>

```
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>Vue 测试实例 - 菜鸟教程(runoob.com)</title>
<script src="https://cdn.bootcss.com/vue/2.2.2/vue.min.js"></script>
</head>
<body>
<div id="app">
  <p>{{ message }}</p>
</div>

<script>
new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue.js!'
  }
})
</script>
</body>
</html>
```

#### 3. NPM方法

由于 npm 安装速度慢，本教程使用了淘宝的镜像及其命令 cnpm，安装使用介绍参照：[使用淘宝 NPM 镜像](http://www.runoob.com/nodejs/nodejs-npm.html#taobaonpm)。

npm 版本需要大于 3.0，如果低于此版本需要升级它：

```
# 查看版本
$ npm -v
2.3.0

#升级 npm
cnpm install npm -g
```

在用 Vue.js 构建大型应用时推荐使用 NPM 安装：

```
# 最新稳定版
$ cnpm install vue
```

##### 命令行工具

Vue.js 提供一个官方命令行工具，可用于快速搭建大型单页应用。

```
# 全局安装 vue-cli
$ cnpm install --global vue-cli
# 创建一个基于 webpack 模板的新项目
$ vue init webpack my-project
# 这里需要进行一些配置，默认回车即可
This will install Vue 2.x version of the template.

For Vue 1.x use: vue init webpack#1.0 my-project

? Project name my-project
? Project description A Vue.js project
? Author runoob <test@runoob.com>
? Vue build standalone
? Use ESLint to lint your code? Yes
? Pick an ESLint preset Standard
? Setup unit tests with Karma + Mocha? Yes
? Setup e2e tests with Nightwatch? Yes

   vue-cli · Generated "my-project".

   To get started:
   
     cd my-project
     npm install
     npm run dev
   
   Documentation can be found at https://vuejs-templates.github.io/webpack
```

进入项目，安装并运行：

```
$ cd my-project
$ cnpm install
$ cnpm run dev
 DONE  Compiled successfully in 4388ms

> Listening at http://localhost:8080

```

成功执行以上命令后访问 http://localhost:8080/，输出结果如下所示：

![img](http://www.runoob.com/wp-content/uploads/2017/01/56219E04-D156-43EC-AC59-BFE7E38A62C3.jpg)

  

## 目录结构

安装项目后打开目录、结构如下

![img](http://www.runoob.com/wp-content/uploads/2017/01/B6E593E3-F284-4C58-A610-94C6ACDAD485.jpg)

