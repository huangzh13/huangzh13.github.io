+++
title = "创建 Posts 的模板"
date = "2026-01-03T14:44:42+08:00"
lastmod = "2026-01-03T14:44:42+08:00"

draft = false

description = ""
tags = []
categories = []

toc = true
math = false
comments = true

readingTime = true
showDate = true
showAuthor = true
showReadingTime = true

image = "cover.png"

slug = ""
+++

## 创建新文章
```bash
hugo new posts/hello-hugo/index.md
```

### 结构
```
content/posts/hello-hugo/
├── index.md
├── cover.png      # 可选
└── images/        # 可选
```

### tags/categories
```
tags：技术点（hugo / kde / arch）
categories：文章类型（notes / config / review）
```

### image
这是 卡片头图 / OpenGraph 图：
image = "cover.png"

对应路径：
```
content/posts/xxx/
├── index.md
└── cover.png
```
👉 推荐 bundle 模式（而不是单 md）

## 发布流程
```bash
# 1. 看是否还有 draft
hugo list drafts

# 2. 本地以“发布模式”预览
hugo server

# 3. 确认 OK 再 push
git push
```

