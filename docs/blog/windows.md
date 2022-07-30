# 修复 Windows

## 修复任务栏图标变成“白纸“

有两种解决方案，通常第二种有用，建议两种同时使用，执行后都需要重启。

第一种：打开文件夹的隐藏项目，`WIN+R` 输入 `%USERPROFILE%\AppData\Local` ，删除名为 `IconCache.db` 的文件。

第二种：`WIN+R` 输入 `%USERPROFILE%\AppData\Roaming\Microsoft\Internet Explorer\Quick Launch\User Pinned\TaskBar` ，把变成白纸的程序的快捷方式粘贴到这个文件夹里面。

使用 Electron 程序时把它固定到任务栏取消固定就大概率会发生这种情况，建议不要固定 Electron 程序到任务栏。

## 让特定程序开机自启动：

将快捷方式放入`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp`