## 介绍

1. 这是 vuepress-theme-reco 的一个修改版本
2. 修改后的主题效果：[ImCaO's Blog](https://www.imcao.cn)
3. 原仓库为 [vuepress-theme-reco](https://github.com/vuepress-reco/vuepress-theme-reco)，作者为 recoluan

## 使用方法

1. 请确保你的项目已经使用 vuepress-theme-reco@1.6.6 为主题，以免产生不可预知的错误
2. 下载本仓库文件到本地
3. 将所有文件覆盖至项目下 \node_modules\vuepress-theme-reco 目录中

## 版本特性

### 页脚修改

* 移除了页脚的版本号，使其变得更加美观
* 调换了版权与备案的顺序，使其变得更加美观

### 首页文章配图

增加首页文章配图功能

使用方法：

在 Markdown 文件中添加 pic 的 frontmatter，示例：

```
---
title: 暑假摸的鱼
date: 2021-09-13
tags:
  - 暑假
  - 折腾
categories:
  - 随笔
pic: /img/2021/summer.jpg
---
```

其中，pic 的路径基于项目的 public 文件夹，因此需要将 summer.jpg 放置于 .vuepress/public/img/2021 目录下

### 文章页头图

文章页头图与首页配图一致，无需额外配置

### bug 修复

* 修复了首页背景图过长的情况下返回首页页面自动下滚的bug