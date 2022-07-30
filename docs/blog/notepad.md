# 记事本

此处记录下不足以单独成文的内容。

## Git 和 GitHub

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

## 修复 Windows

### 修复任务栏图标变成“白纸”

有两种解决方案，通常第二种有用，建议两种同时使用，执行后都需要重启。

第一种：打开文件夹的隐藏项目，`WIN+R` 输入 `%USERPROFILE%\AppData\Local` ，删除名为 `IconCache.db` 的文件。

第二种：`WIN+R` 输入 `%USERPROFILE%\AppData\Roaming\Microsoft\Internet Explorer\Quick Launch\User Pinned\TaskBar` ，把变成白纸的程序的快捷方式粘贴到这个文件夹里面。

使用 Electron 程序时把它固定到任务栏取消固定就大概率会发生这种情况，建议不要固定 Electron 程序到任务栏。

### 让特定程序开机自启动

将快捷方式放入`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp`

## 其他

开启了 Lenovo Vantage 中的 电源管理-节电模式，最大充电容量只到 60%

关闭背后的大 Y 灯：`Fn+L`

切换屏幕刷新率：`Fn+R`

开关键盘背光：`Fn+Space`

优先使用 val 声明变量，需要时再用 var

`cd docs && python -m SimpleHTTPServer 3000`

`cd docs && python -m http.server 3000`

VS Code：让文本超出屏幕自动换行`Editor:Word Wrap`设为 on 将在视口宽度换行，设为 off 则永不自动换行

yt-dlp 选择分辨率：`yt-dlp -S "height:1080"`

Jellyfine