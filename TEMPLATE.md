---
title: 文章标题
layout: post
date: 2026-01-01 12:00:00 +0800
categories: post
---

> **使用说明**（写完后删除这一段）
>
> 1. 把本文件复制/重命名为 `_posts/YYYY-MM-DD-文章标题.md`（文件名必须以日期开头）。
> 2. 上面 YAML 头只需改 `title` 和 `date`；`layout` 和 `categories` 保持不变。
> 3. 正文使用 GitHub 风格 Markdown（GFM）：表格、删除线（~~划掉~~）、任务列表、
>    自动链接都支持，与 docs 站的书写体验一致。
> 4. 摘要分隔：正文里想控制列表页摘要截断的位置，插入一行 `<!--more-->`。
> 5. 推送到 GitHub 后自动发布，无需其他操作。

## 一级小节

正文从这里开始。行内代码 `like this`，代码块如下：

```bash
export PS1='\u@\h:\w\$ '
```

### 表格

| 语法 | 支持情况 |
| ---- | :------ |
| GFM 表格 | ✅ |
| ~~删除线~~ | ✅ |
| - [ ] 任务列表 | ✅ |

### 数学公式

行内公式 $E = mc^2$，块级公式：

$$
\int_0^\infty e^{-x^2}\,dx = \frac{\sqrt{\pi}}{2}
$$

### 引用与脚注

> 引用一段话。

带边注（marginnote/sidenote）是本主题的特色，直接使用 Tufte 语义即可。
