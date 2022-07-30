---
title: "Git 和 GitHub"
date: 2022-07-28
---

连接到 GitHub

使用 GitHub CLI`scoop install gh`
```
git add .
git commit -m "first"
git remote add origin https://github.com/TokyoIncidents/blog.git
git push -u origin master
```

[7.11 Git 工具 - 子模块](https://git-scm.com/book/zh/v2/Git-%E5%B7%A5%E5%85%B7-%E5%AD%90%E6%A8%A1%E5%9D%97)

> 你必须运行两个命令：`git submodule init` 用来初始化本地配置文件，而 `git submodule update` 则从该项目中抓取所有数据并检出父项目中列出的合适的提交。不过还有更简单一点的方式。 如果给 `git clone` 命令传递 `--recurse-submodules` 选项，它就会自动初始化并更新仓库中的每一个子模块， 包括可能存在的嵌套子模块。