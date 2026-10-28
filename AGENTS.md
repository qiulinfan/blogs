# blogs

- 本仓库只维护博客内容：Markdown 文章、文章元数据与图片。用户自行选择编辑方式，当前使用 Obsidian；不要引入 CMS、编辑器依赖、Astro 项目或网站构建流程。
- 文章放在 `posts/`，文章图片可放在篇内相对路径的附件目录。保留既有文件名、相对链接及文章地址；迁移或重命名可能改变网站 URL，须核对网站接入。
- `qiulinfan.github.io` 通过其 `docks.json` 和 `site/src/docks/blogs/` 接入本仓库，负责网页渲染、布局和部署；网站代码及预览在该仓库维护。
- 正文使用标准 Markdown；数学公式使用 `$...$` 或 `$$...$$`。引用公开论文或其他可访问来源，不把私人阅读库原文、译稿或本机绝对路径复制进公开文章。
- 保持作者自己的观点与文字；仅在明确要求时撰写或改写正文。不要把规划当成已经读完或掌握的知识。
- 不自动发布草稿。`draft: true` 的文章在网站开发预览中可见，在正式网页构建中排除；本仓库公开，Git 中的草稿源码仍可被读取。
- Obsidian 和其他编辑器的本机设置保留本地，不入库；忽略任意深度的 `.DS_Store`。
- 用户交流与交付使用用户的语言。

## 文章元数据

```yaml
---
title: "文章标题"
published: 2026-10-28
description: "一句话摘要"
image: ""
tags: []
category: ""
draft: true
lang: zh_CN
---
```

`published` 为文章发布日期；修订日期可用 `updated`。准备发表时再设置实际日期与 `draft: false`。网站负责校验元数据和渲染；本文库不绑定编辑器。

## 内容来源

既有文章及其内容历史从 `qiulinfan/qiulinfan.github.io` 的 `site/src/content/posts/` 提取，映射到本库 `posts/`，保留作者与提交信息。迁移来源为网站提交 `afdc06f1bef71b233d9a2bd8c79181ef082295c2`。
