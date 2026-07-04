---
title: 从素材库到公开页面的发布检查清单
description: 知识管理素材进入 Quartz content 前需要检查什么
date: 2026-06-22
created: 2026-06-22
modified: 2026-06-24
tags:
  - knowledge-management
  - quartz
  - publishing
  - checklist
---

# 从素材库到公开页面的发布检查清单

素材库里的笔记可以粗糙，公开页面要多一道检查。

这道检查不用追求完美，主要是避免读者打开以后完全摸不到入口。

## 内容检查

先看内容本身：

- 标题是否清楚
- 页面是否只处理一个核心问题
- 第一屏能否说明这页在讲什么
- 是否有过时软件、旧平台、旧流程
- 是否包含私人信息
- 是否还保留太多内部口吻

如果一页内容只对自己当时有意义，先别急着发布。

## 结构检查

再看结构：

- 是否有小标题
- 是否有进入下一页的链接
- 是否能回到 MOC
- 是否和已有页面重复
- 是否需要拆分成多篇
- 是否只是素材，暂时放在 `imports/`

公开页面最好能独立阅读，也能接回知识地图。

## 链接检查

Obsidian 里的链接迁移到 Quartz 前，要检查：

- `[[wikilink]]` 是否能解析
- 别名链接是否清楚
- 指向的页面是否已经发布
- 图片是否能访问
- 外部链接是否还有效
- 旧路径是否需要改成新路径

断链会明显影响阅读体验。

## frontmatter 检查

我会统一检查：

```yaml
title:
description:
date:
created:
modified:
tags:
```

这批知识管理页面的时间统一落在 2026 年 4 月到 6 月之间，方便形成一个清晰的整理周期。

## 发布后检查

本地构建通过后，再打开本地预览：

```bash
npm run quartz -- build
```

需要检查：

- 页面能否打开
- 入口页是否出现新链接
- MOC 是否更新
- 移动端阅读是否还算顺
- 是否还有明显 AI 味句式

## 相关页面

- [[quartz-digital-garden-publishing|我如何用 Quartz 发布数字花园]]
- [[personal-knowledge-management-overview|个人知识管理总览]]
