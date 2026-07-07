# 母婴成分说 - 网站项目

## 项目简介
基于 Hugo 静态网站生成器搭建的母婴产品测评对比网站，部署在 Vercel 上。

## 项目结构
```
muyingchengfen/
├── config.toml              # 站点配置
├── vercel.json              # Vercel部署配置
├── content/
│   ├── about.md             # 关于页面
│   └── posts/
│       ├── _index.md        # 文章列表页
│       ├── feihe-vs-yili.md # 对比文（高流量词）
│       ├── baby-green-stool.md # 长尾痛点文
│       └── what-is-opo.md   # 成分解析文
├── layouts/                 # 页面模板
│   ├── index.html           # 首页
│   └── _default/
│       ├── baseof.html      # 基础模板
│       ├── list.html        # 列表页模板
│       └── single.html      # 文章详情页模板
├── static/
│   ├── css/style.css        # 样式文件
│   └── robots.txt           # 爬虫规则（已开放AI爬虫）
└── README.md
```

## 部署步骤

### 第1步：注册 GitHub 账号（如果还没有）
访问 https://github.com 注册

### 第2步：创建新仓库
1. 登录 GitHub 后，点击右上角 "+" → "New repository"
2. 仓库名填：muyingchengfen
3. 勾选 "Add a README file"
4. 点击 "Create repository"

### 第3步：上传文件
1. 在仓库页面点击 "Add file" → "Upload files"
2. 把本项目文件夹里的所有文件拖进去
3. 点击 "Commit changes"

### 第4步：注册 Vercel 账号
1. 访问 https://vercel.com
2. 点击 "Sign Up"，选择用 GitHub 账号登录

### 第5步：部署网站
1. 在 Vercel 控制台点击 "Add New..." → "Project"
2. 找到你的 muyingchengfen 仓库，点击 "Import"
3. Framework Preset 选择 "Hugo"
4. 点击 "Deploy"
5. 等待1-2分钟，部署完成！

### 第6步：访问你的网站
部署完成后，Vercel 会给你一个地址，类似：
`https://muyingchengfen.vercel.app`

恭喜，你的网站上线了！🎉

## 如何发布新文章

### 方法：直接在 GitHub 上操作
1. 进入 content/posts/ 目录
2. 点击 "Add file" → "Create new file"
3. 文件名用英文，如 `a2-milk-review.md`
4. 文件内容按以下格式开头：

```
---
title: "文章标题"
description: "文章摘要，会显示在列表页"
date: 2026-07-06
categories: ["奶粉对比"]
tags: ["标签1", "标签2"]
featured: false
toc: true
---

正文内容写在这里...
```

5. 点击 "Commit new file"
6. Vercel 会自动重新部署，1-2分钟后文章就上线了

## 后期优化
- 购买自己的域名（如 muyingchengfen.com），在 Vercel 设置中绑定
- 添加 Google Analytics 统计
- 添加百度统计
- 提交 sitemap 到百度站长平台和 Google Search Console
