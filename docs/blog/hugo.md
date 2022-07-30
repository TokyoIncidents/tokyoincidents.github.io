# 使用 Hugo 在 GitHub 上部署博客

## 安装 Hugo 并创建网站

用 Scoop 安装：`scoop install hugo`，输入`hugo new site <name>`来创建一个新的网站。此时创建了多个文件夹，`content`是存放网站的资源，`themes`是存放网站的主题。

## 安装主题

`git init`将此文件夹初始化为 git 仓库。Hugo 没有自带主题，可以在 https://themes.gohugo.io/ 
获取。将主题文件夹放在`themes`下即可。我使用的是 [Paper](https://github.com/nanxiaobei/hugo-paper)，请阅读文档了解 Hugo 版本要求和安装方式，如安装 Paper：`git submodule add https://github.com/nanxiaobei/hugo-paper themes/paper`

## 修改配置文件

编辑`config.toml`来修改网站配置，在主题的文件夹里通常会有`exampleSite`文件夹，里面是默认的网站模板，可以参考进行修改。之后如果用 GitHub Pages 的时候指定`docs`目录，可以加入`publishDir = "docs"`以`docs`方式生成网站的文件，比较方便下面是我已经配置好的：

```toml
baseURL = "https://tokyoincidents.github.io/blog/" # 网址
languageCode = "en" # 语言
title = "Zen" # 标题
theme = "paper" # 主题
paginate = 5 # 每页文章个数
[params]
  github = 'TokyoIncidents' # 显示一个指向特定 GitHub 用户的 icon 
```

## 新建一篇文章并编译网站的文件

`hugo new post\myblog.md`来新建一个文章。文章开头会有以下字段：

```markdown
---
title: "使用 Hugo 在 GitHub 上部署博客"
date: 2021-11-27T13:49:11+08:00
---
```

`title`是文章标题，`date`是文章的时间，`hugo server`在本地预览网站，确认后`hugo`来编译网站。GitHub Pages 的设置里面会有`root`和`docs`模式两种选项，前者是读取根目录，通过建立两个分支使用 GitHub Actions 编译网站，后者是读取 docs 文件夹，直接把源码和编译后的网站都放在 GitHub 的仓库中。（在配置文件里加入一行`publishDir = "docs"`）

在 GitHub，新建一个名字是 blog 的仓库，推送到远程仓库。

## 使用 Actions 自动编译

在 GitHub 账户的开发者设置-Personal access tokens 中新建一个 token，勾选 repo 和 workflow，进入仓库设置-secrets，新建标题为 personal_token ，内容是刚创建的 tokens。新建一个分支 gh-pages 后再新建一个 Action，输入以下代码：

```
name: GitHub Pages

on:
  push:
    branches:
      - master

jobs:
  build-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v1
        with:
          submodules: true # 是否使用子模块
          fetch-depth: 0

      - name: Setup Hugo
        uses: peaceiris/actions-hugo@v2
        with:
          hugo-version: latest

      - name: Build 
        run: hugo

      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          personal_token: ${{ secrets.personal_token }}
          PUBLISH_BRANCH: gh-pages
          PUBLISH_DIR: ./public
          commit_message: ${{ github.event.head_commit.message }}

```
然后在仓库设置-Pages-Source 中的 Branch:master/(root)，中的 master 改为 gh-pages。这样网站就搭建完成了。

注意 git 子模块的使用


参考：

[使用 Hugo 从 0 到 1 搭建个人博客](https://sspai.com/post/64639)

[记——搭建 hugo+github 静态博客](https://segmentfault.com/a/1190000019823896)

[如何使用 Hugo 在 GitHub Pages 上搭建免费个人网站](https://zhuanlan.zhihu.com/p/37752930)
