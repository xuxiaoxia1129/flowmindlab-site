---
title: 我如何用 Quartz 发布数字花园
description: 从 Obsidian 笔记到 Quartz、GitHub Pages 和自定义域名的发布流程
date: 2026-06-20
created: 2026-06-20
modified: 2026-06-20
tags:
  - knowledge-management
  - quartz
  - digital-garden
  - publishing
---

# 我如何用 Quartz 发布数字花园

我选择 Quartz 发布数字花园，核心原因是它和 Obsidian 的工作方式足够接近：Markdown、双链、MOC、反向链接、搜索和静态网站。

发布这件事，不能理解成把私人笔记全部扔到网上。更合理的做法，是把已经整理过、适合公开的内容转成可阅读页面。

## 当前流程

当前站点的发布路径是：

Obsidian/Markdown 素材 -> Quartz `content/` -> GitHub 仓库 -> GitHub Pages -> 自定义域名

本项目已经配置了 GitHub Pages 部署。推送到 `v4` 分支后，GitHub Actions 会构建 Quartz，并把 `public` 目录发布出去。

当前线上域名是：

`https://www.flowmindlab.cn`

## 内容进入站点前要做什么

所有笔记进 `content/` 前，我会先检查一遍：

- 是否有明确标题
- 是否能独立阅读
- 是否包含私人信息
- Obsidian 双链是否能在 Quartz 中正常解析
- 图片是否能访问
- frontmatter 是否规范
- 是否挂到了合适的 MOC 或入口页

这也是为什么我先把旧素材放进 `imports/knowledge-management-source/`，再从中改写成正式页面。

## 为什么不整库发布

整库发布看起来省事，但会带来几个问题：

- 半成品会稀释站点质量
- 旧链接和旧路径容易失效
- 私人工作流会暴露太多噪音
- 读者找不到入口
- 未来维护成本会很高

更好的方式是分批发布：先做主题地图，再做核心文章，再逐步补充卡片和参考资料。

## 我的发布标准

一篇页面至少要满足三个条件：

- 能回答一个明确问题
- 能链接到站点中的其他页面
- 未来仍然值得维护

这也是数字花园和普通博客的区别。博客更像时间线，数字花园更像知识地图。

## 后续维护

每次新增页面后，需要同步更新：

- 对应主题入口页
- 对应 MOC
- 相关页面之间的双链
- 构建结果

本地验证通常使用：

```bash
npx quartz build
```

构建通过后，再提交并推送到 `v4` 分支触发发布。

## 相关页面

- [[personal-knowledge-management-overview|个人知识管理总览]]
- [[obsidian-fit-and-limits|Obsidian 适合什么，不适合什么]]
- [[obsidian-plugin-system|我的 Obsidian 插件体系]]
- [[publishing-checklist-from-source|从素材库到公开页面的发布检查清单]]
- [[knowledge-work-toolchain|辅助知识工作的工具链]]
