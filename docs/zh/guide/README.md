# 介绍

D2Admin 是一个开源的管理系统前端集成方案

[Github仓库](https://github.com/FairyEver/d2-admin) - [预览地址](https://fairyever.gitee.io/d2-admin-preview)

<div>
  <iframe src="//ghbtns.com/github-btn.html?user=FairyEver&repo=d2-admin&type=star&count=true" allowtransparency="true" frameborder="0" scrolling="0" width="100" height="20"></iframe>
  <iframe src="//ghbtns.com/github-btn.html?user=FairyEver&repo=d2-admin&type=fork&count=true" allowtransparency="true" frameborder="0" scrolling="0" width="100" height="20"></iframe>
</div>

::: tip
因为现在集成了很多的插件和组件，首次加载会占用很多的时间，虽然已经做了首屏加载动画，但还是建议您在发布之前一定要删除没有用到的代码，比如项目没有用到图表、示例、插件组件。
:::

D2Admin 是完全开源免费的管理系统集成方案，由 [FairyEver](https://github.com/FairyEver) 在工作之余完全由兴趣驱动完成，如果你也一样喜欢前端开发，欢迎加入我们的讨论/学习群，群内可以`提问答疑`，`分享学习资料`或者随便扯淡

**QQ群 806395827**

<a target="_blank" href="//shang.qq.com/wpa/qunwpa?idkey=48323a4ed7a059a5d75f4a81586161ee60e495ab31905f8daaee8939ecacb363"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="D2Admin | js | vue 交流" title="D2Admin | js | vue 交流"></a>

**微信群**

作者微信 liyang1711467488

> 微信群需要先加群主才可以拉进群 PS 微信群交流不太方便，建议QQ群

::: tip Thanks
D2Admin 创建于2018年1月14日零点51分，在2018年5月26日正式发布，中间断断续续做了四个多月，发布一个月内收获将近 700star，在此对支持我的朋友表示感谢，D2Admin 将会保持更新，如果你有想法、建议、或者问题欢迎加群讨论

—— 2018年6月20日
:::

## 功能

* 首屏加载等待动画 避免首次加载白屏尴尬
* 简约主题
* 每个插件和组件都配有介绍文档
* 图片资源 sketch 源文件（ 可以在这个文件内重新生成所有图片资源 ）
* 登陆和注销
* 根据路由自动生成菜单
* 可折叠侧边栏
* 方便的菜单设置
* 多国语言支持
* 富文本编辑器
* Markdown 编辑器
* 全屏功能
* Fontawesome 图标库
* 图标选择器（组件）
* 自动引入下载的 SVG 图标
* 前端假数据支持（ mock ）
* 集成蚂蚁金服出品的 G2 图表
* 图表自适应可拖拽大小的卡片容器（示例）
* 简化剪贴板操作
* 简化Cookie操作
* 时间日期计算工具
* 导入 Excel （ xlsx 格式 + csv 格式 ）
* 数据导出 Excel （ xlsx 格式 + csv 格式 ）
* 数据导出文本
* 数字动画
* 可拖拽调整大小的切分布局
* 可拖拽调整大小和位置的网格布局
* 提供三种方便的页面容器组件（正常卡片，隐形容器，填满页面）
* 代码高亮显示
* 加载并解析（或者直接指定资源） markdown 文件
* GitHub 样式的 markdown 显示组件
* markdown 内代码高亮
* 为 markdown 扩展了百度云链接解析和优化显示
* 右键菜单组件
* 自定义滚动条和滚动控制
* 内置4种主题
* 公用样式抽离，方便的主题定制
* 支持百万级数据量的表格组件
* 打包后随意目录部署（已经做好兼容设置）

## TODO

D2Admin 仍然处于开发中，这里有一些暂时的计划：

* 分离出简化版本
* 推出基于 [ice](https://alibaba.github.io/ice) 平台的版本
* 增加右上角通知中心
* 增加一些实例页面以提供业务页面布局建议
* 更换图表库
* 多 tab 页结构
* 面包屑导航
* 树型表格组件
* 更多类型的编辑器
* socket 连接
* 浏览器版本提示
* 日志控制台
* `1.1.0 完成` 抽离项目里的文档，集中存放在文档站点
* `1.1.0 完成` 对主界面进行一次完善，调整整体布局和颜色
* `1.1.0 完成` 切换主题功能

欢迎你为 D2Admin 的开发作出贡献（代码编写/文档翻译）。

## 目录结构

```
├─ build
├─ config
├─ docs // 文档
├─ src
│  ├─ assets // 资源
│  │  ├─ icons
│  │  ├─ image
│  │  ├─ library
│  │  └─ style
│  ├─ components // 组件
│  │  ├─ charts // 图表组件
│  │  ├─ core // 核心组件
│  │  └─ demo // 示例组件
│  ├─ i18n // 多国语
│  ├─ menu // 菜单
│  ├─ mock // 模拟数据
│  ├─ pages // 页面
│  ├─ plugin // 插件
│  ├─ router // 路由
│  ├─ store // vuex
│  ├─ utils // 通用函数
│  ├─ App.vue
│  └─ main.js
├─ static // 静态资源
├─ .babelrc
├─ .editorconfig
├─ .eslintignore
├─ .eslintrc.js
├─ .gitattributes
├─ .gitignore
├─ .postcssrc.js
├─ LICENSE
├─ README.md
├─ deploy.sh
├─ design.sketch // 设计文件
├─ index.html
└─ package.json

```

## 获取代码

有两种方式可以获得 D2Admin 的代码

* 在 [releases](https://github.com/FairyEver/d2-admin/releases) 页面下载最新的发行版。发行版一般是完成了某个大升级或者修复重要 bug 后发布的压缩包，你可以下载下来直接使用

* Fork 仓库到你的 github 然后克隆到本地，然后使用 master 分支继续你的开发。这种方式得到的是最新的代码，但是会有未完成的新功能。

## 使用

```
// 安装依赖
npm i

// 运行
npm run dev

// 打包
npm run build
```

> 如果上述步骤出现错误，建议您升级 node 版本 > 8，如果有其它疑问请参考[常见问题](/zh/guide/question.html)

## 书写文档

这里目前还有一个小遗憾，d2admin 使用的 webpack 版本不能符合 vuepress 的要求，所以如果你想在本地启动文档站点的服务，需要按下述步骤

首先将 vuepress 安装到全局

```
npm i -g vuepress
```

启动服务

```
npm run doc:dev
```

::: tip
你可能会发现项目目录中有一个 deploy.sh 文件，这个文件是为了方便发布文档用的，通常你并不需要使用它
:::