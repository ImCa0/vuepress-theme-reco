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

在 Markdown 文件中添加 abs_img 的 frontmatter，示例：

```
---
title: 暑假摸的鱼
date: 2021-09-13
tags:
  - 暑假
  - 折腾
categories:
  - 随笔
abs_img: /img/2021/summer.jpg
---
```

其中，abs_img 的路径基于项目的 public 文件夹，因此需要将 summer.jpg 放置于 .vuepress/public/img/2021 目录下

### 文章页头图

与首页文章配图类似，只需在 frontmatter 中添加 head_img 即可，文件路径基于项目的 public 文件夹

### 子侧边栏与头图适配

取消了显示子侧边栏时页面与右侧的边距增大；子侧边栏现在只会在页面滚动到头图之下（如果有的话）时显示。

### bug 修复

* 修复了首页背景图过长的情况下返回首页页面自动下滚的bug