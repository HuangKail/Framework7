[![Stories in Ready](https://badge.waffle.io/nolimits4web/framework7.png?label=ready&title=Ready)](https://waffle.io/nolimits4web/framework7)
[![Build Status](https://travis-ci.org/nolimits4web/Framework7.svg?branch=master)](https://travis-ci.org/nolimits4web/Framework7)
[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=nolimits4web&url=https://github.com/nolimits4web/framework7/&title=Framework7&language=JavaScript&tags=github&category=software)

Framework7
==========


# 一 环境

## 环境安装

F7使用Grunt编译代码，如果你没有使用过，请参考这里 [grunt getting started](http://gruntjs.com/getting-started)。在安装Grunt之前你可能还需要安装nodejs环境。

Grunt安装完成之后，在根目录下执行 `npm install` 即可。

## 使用Grunt

grunt 中配置了如下几个任务：

* `grunt` 默认任务，会编译js,css和示例到build目录下，等价于 `grunt build`
* `grunt watch` watch模式，开发的时候启动这个命令即可
* `grunt test` 运行测试
* `grunt server` 启动服务器,启动之后可以直接访问 [http://localhost:3000/docs/](http://localhost:3000/docs/)
* `grunt kitchen` 编译 kitchen
* `grunt apps` 编译 apps
* `grunt examples` 编译 examples


# 二 文件结构说明

下面是重要的文件说明

* Framework7/: 根目录
  * src/: 源码
    * img/: 图片
    * js/: js源码
    * less/: 使用less编写的css源码
    * my-app/: 示例使用的js和css
    * templates/: 示例的html模板，使用jade编写

  * build/: 编译后css、js、图片和示例，用来发布到CDN，用在生产环境
    * css/: 编译后的css文件
    * js/: 编译后的js文件
    * img/: 图片
    * *.html: 示例

  * docs/:  文档
    * templates/：使用jade编写的文档模板
    * docs-demos/:  文档中使用的示例，用在文档右侧的设备模拟器中

  * apps/: 示例
  * examples/: 示例
  * kitchen-sink/: 示例
  * Gruntfile.js: grunt配置文件
