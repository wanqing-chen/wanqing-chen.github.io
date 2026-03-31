---
title: "从 0 到 1： Hugo 自动化博客构建指南"
date: 2026-03-30T20:00:00+08:00
draft: false
description: "记录基于 Hugo + PaperMod + GitHub Actions 搭建个人技术博客的标准工作流。"
categories: ["技术工程"]
tags: ["Hugo", "CI/CD", "Workflow"]
---

作为一名大数据工程师，构建高效的知识沉淀体系与构建数据中台同样重要。本站基于 Hugo 构建，旨在记录关于 Flink、Paimon 及 AI 架构的思考。

## 🛠️ 博客维护：标准三步走

### 1. 创作与预览
在本地环境（VS Code）进行内容产出：
- **新建文章**：在 `content/posts/` 目录下创建 `.md` 文件。
- **本地预览**：运行 `hugo server -D` 并在浏览器查看效果。

### 2. 推送更新
通过 Git 将源码推送到 GitHub：
```bash
git add .
git commit -m "feat: content update"
git push origin main