---
title: 我的 Obsidian 插件体系
description: 插件如何围绕捕捉、连接、维护和发布服务，避免反过来制造复杂度
date: 2026-06-12
created: 2026-06-12
modified: 2026-06-20
tags:
  - knowledge-management
  - obsidian
  - plugins
---

# 我的 Obsidian 插件体系

Obsidian 插件很多，但数量一多，系统很容易开始反噬自己。

我更关心一个插件是否服务于稳定工作流：捕捉、编辑、连接、检索、维护、发布。如果一个插件只是新奇，或者让系统变得更难迁移，它就不应该进入核心配置。

## 核心判断

插件选择先看工作流，再看功能。

我会问：

- 它是否减少重复劳动
- 它是否增强链接、搜索或维护能力
- 它是否依赖太多私有语法
- 它是否会拖慢启动和编辑
- 它是否能被其他工具替代

如果一个插件只是“看起来很强”，但没有固定使用场景，最后大概率会变成维护负担。

## 核心插件方向

第一类是连接与检索。

反向链接、出链、搜索、图谱、Omnisearch、Dataview 这类能力，服务的是找回上下文。知识库规模越大，检索和聚合越重要。

第二类是编辑与整理。

Advanced Tables、Linter、Note Refactor、File Cooker、Tag Wrangler、Templater 这类工具，适合处理格式、拆分、批量维护和模板化输入。

第三类是捕捉与入口。

Daily Note、Quick Switcher、Commander、Another Quick Switcher、Advanced URL、auto-link-title 这类工具，解决的是快速进入、快速记录、快速链接。

第四类是视觉与空间。

Canvas、Excalidraw、Sliding Panes、Pane Relief、Style Settings 可以改善工作空间，但这类插件要克制使用。它们应该服务理解，不应该变成装饰。

第五类是同步与发布。

Remotely Save、Git、Quartz 相关流程、图片处理工具，服务的是跨设备和公开发布。这里我更看重稳定性，功能丰富度排在后面。

## 我不优先推荐的方向

任务管理插件不一定适合放在 Obsidian 里。复杂任务、提醒、看板和协作，通常有更专业的软件。

AI 插件也不一定要装在 Obsidian 内部。对于整个 vault 的批量整理、链接修复、改写和重构，能直接打开文件夹的代码编辑器或外部 AI 工作流往往更灵活。

过度美化也要谨慎。主题、CSS 和图标可以改善体验，但不应该影响 Markdown 的可迁移性。

## 最小可用组合

如果只保留一个轻量组合，我会优先保留：

- 反向链接和出链
- Daily Note
- 搜索或增强搜索
- Dataview 或类似聚合工具
- Templater
- Linter
- Note Refactor 或文件整理工具
- Quartz 发布流程

这套组合已经能支撑从记录到整理再到发布。

## 相关页面

- [[obsidian-fit-and-limits|Obsidian 适合什么，不适合什么]]
- [[obsidian-search-maintenance-workflow|Obsidian 搜索与维护工作流]]
- [[moc-para-access|MOC、PARA 与 ACCESS 如何分工]]
- [[quartz-digital-garden-publishing|我如何用 Quartz 发布数字花园]]
