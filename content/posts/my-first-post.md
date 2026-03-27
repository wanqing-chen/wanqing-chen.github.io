+++
date = '2026-03-27T13:26:24+08:00'
draft = false
title = "我的第一篇文章"

+++

这是我的第一篇 Hugo 文章！ 

## 标题

Hugo 使用 CommonMark Markdown 规范，支持各种 Markdown 语法。 

- 列表项 1
- 列表项 2
- 列表项 3

**粗体文本** 和 *斜体文本*。

## Hugo 博客更新：标准三步走
### 第一步：创作阶段（在本地 VS Code）
- 新建文章：在 content/posts/ 目录下新建一个 .md 文件（或者复制旧的改名）
- 检查 date 日期（不要早于当前时间太久，也不要晚于当前时间）。
- 在终端运行 hugo server。
- 打开浏览器访问 http://localhost:1313 检查排版。
- 满意后按下 Ctrl + C 停止服务。

### 第二步：推送阶段（在终端敲 3 行命令）
- git add .
- git commit -m "feat: 新增一篇文章"
- git push origin main

⚠️ 特别提醒（新手易错点）：
不要管 public 文件夹：如果以后看到 public 文件夹里有一堆 HTML，不用去理会它，更不要手动改里面的代码，因为 GitHub Actions 每次都会重新生成并覆盖它。

自动保存：既然你开启了 VS Code 自动保存，写完代码直接去终端执行 git push 即可，不用担心没存上。

图片处理：如果你要在文章里插图，把图片放在 static/images/ 目录下，然后在 Markdown 里引用 /images/xxx.jpg 即可。

