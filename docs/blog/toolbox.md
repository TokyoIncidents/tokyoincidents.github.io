# 我的软件工具箱

![emiya_wp.webp](https://s2.loli.net/2022/07/22/CIjx9Ln2cXHmDEY.webp)

> 推荐观看《卫宫家今天的饭》

追求效率并不是探索工具的终极目的，寻找一个属于自己的数字生活方式才是。工具的利手会改变人对事物的感知，激发创作的源泉。我搭建的基于 Windows 和 Android 平台的软件工具箱就具有这样的意义。选择软件的标准是：简洁且功能强大，做好自己的本职工作而不作额外的打扰。

[Scoop](https://scoop.sh/) - 使用命令行搜索、下载和更新软件，建议用于便携化和命令行程序，能够自动配置环境变量。

## 基础工具

无论是任何用途的设备都可以安装使用的软件，提供了日常使用最基础的功能。

[IrfanView](https://www.irfanview.com/) - 老牌图片查看器，支持安装插件来扩展格式和语言

[PeaZip](https://peazip.github.io/) - 基于 7-zip 的解压缩工具，支持双击智能解压

[Snipaste](https://snipaste.com/) - 贴图和截图工具，可以自动选取窗口区域和进行简单的标注，适用于撰写软件教程时配图。

同类软件：[Sniptool](https://www.reasyze.com/sniptool/)、[ShareX](https://getsharex.com/)

[Geek Uninstaller](https://geekuninstaller.com/) - 卸载时清理残留，注意它可能采用关键词匹配，所以如果安装了同一开发者多个产品时请在卸载时仔细确认。

[uTools](https://www.u.tools/) - 启动器

## 浏览器

[Mozilla Firefox](https://www.mozilla.org/en-US/firefox/all/) - 无法替代的主力浏览器，Chromium 阵营外唯一的主流跨平台浏览器，专注于隐私保护和高度自定义化。推荐下载英文版使用，可在设置中切换中文。详见[Firefox 浏览器](https://tokyoincidents.github.io/#/blog/firefox)，可以使用 [Microsoft Edge](https://www.microsoft.com/en-us/edge) 作为备用，基于 Chromium 有性能和兼容性的保证。

### 扩展

浏览器许多进阶的功能都是通过扩展来提供的，它们就像安装在手机上的应用程序，不过范围仅限定在浏览器内。

[uBlock Origin](https://github.com/gorhill/uBlock) - 轻量高效的广告屏蔽插件，UI 略逊于 AdGuard，其核心就是订阅规则和自定义规则，它已经内置了数个规则，轻度用户用默认即可， 也可以订阅其他规则来增强广告屏蔽能力，你可以在 [FilterLists](https://filterlists.com/) 获取，以语言、软件等维度筛选规则，不限于 uBlock Origin。

[AdGuard](https://adguard.com/) - 广告屏蔽插件，带来开箱即用的体验

[uBlacklist](https://github.com/iorate/uBlacklist) - 屏蔽搜索引擎搜索结果中的特定条目。可以用正则表达式撰写规则，也可以订阅别人创建的规则。

参考：

- [内容农场网站清单](https://github.com/wdmpa/content-farm-list)

- [中文搜索结果黑名单](https://github.com/cobaltdisco/Google-Chinese-Results-Blocklist)

- [发现很多网友对「小搭百科网」的关注度比较高，于是……](https://www.v2ex.com/t/806684?p=1)

- [如何屏蔽“小搭百科网”？](https://github.com/cobaltdisco/Google-Chinese-Results-Blocklist/issues/50)

- [清理「内容农场」，还你清爽的 Google 中文搜索体验](https://sspai.com/post/69407)

[SingleFile](https://github.com/gildas-lormeau/SingleFile) - 可以完整地保存网页,包括样式和图片

[沙拉查词](https://saladict.crimx.com/) - 划词翻译，支持多种字典

### 脚本

用户脚本可以对网页的内容进行修改，实现网站没有提供的功能。

脚本管理器： [Tampermonkey](https://www.tampermonkey.net/)

脚本：

[Bilibili Evolved](https://github.com/the1812/Bilibili-Evolved)
[贴吧页面精简](https://greasyfork.org/zh-CN/scripts/23687-贴吧页面精简)

[CSDN 绿化](https://greasyfork.org/zh-CN/scripts/378351-持续更新-csdn广告完全过滤-人性化脚本优化-不用再登录了-让你体验令人惊喜的崭新csdn)

[AC-baidu-重定向优化](https://greasyfork.org/zh-CN/scripts/14178-ac-baidu-%E9%87%8D%E5%AE%9A%E5%90%91%E4%BC%98%E5%8C%96%E7%99%BE%E5%BA%A6%E6%90%9C%E7%8B%97%E8%B0%B7%E6%AD%8C%E5%BF%85%E5%BA%94%E6%90%9C%E7%B4%A2-favicon-%E5%8F%8C%E5%88%97)

## 视频播放

[mpv](https://mpv.io/) - 极致简洁的视频播放器，主打快捷键操作，以下表为例：

| 快捷键|功能|
|-|-|
|p 或 Space|暂停|
|f|全屏|
|q|退出|
|Q|记住播放位置并退出 |
|[ ]|加速 减速|
|Backspace|回到默认速度|
|s|截屏|

参考：[MPV 高手首选的跨平台全能视频播放器！开源、简约、键盘流、配置灵活](https://www.iplaysoft.com/mpv.html)

同类软件：[VLC](https://www.videolan.org/vlc/)、[MPC-BE](https://sourceforge.net/projects/mpcbe/)

## 文件管理

[XYplorer](https://www.xyplorer.com/free.php) - 文件管理器

[Syncthing](https://syncthing.net/) - 同步文件夹，速度有点慢，用来手机电脑同步

[Cloudreve](https://cloudreve.org/) - 自托管网盘服务，部署到了内网

[Everything](https://www.voidtools.com/zh-cn/) - 速度极快的本地文件搜索

## 编程开发

[Visual Studio Code](https://code.visualstudio.com/) - 有广泛插件支持的代码编辑器，配置插件后可以写 markdown，可以用简单的符号同时输入格式和内容，从而屏蔽样式对写作的干扰。推荐使用插件 [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)。亮色主题：[Atom One Light Theme](https://marketplace.visualstudio.com/items?itemName=akamud.vscode-theme-onelight)，暗色主题：[Dark Purple - WebStorm Edition](https://marketplace.visualstudio.com/items?itemName=rexebin.darkpurple)

[Windows Terminal](https://github.com/Microsoft/Terminal) - Windows 终端工具，可以高度自定义

终端美化方案：

[Starship](https://starship.rs/)

参考：[在所有终端中使用相同界面，Starship 帮助你自定义命令行](https://sspai.com/post/72888)

[Oh My Posh](https://ohmyposh.dev/)

参考：[Oh My Posh：全平台终端提示符个性化工具](https://sspai.com/post/69911)


[Android Studio](https://developer.android.com/studio)

[IntelliJ IDEA](https://www.jetbrains.com/idea/)

[JetBrains Toolbox](https://www.jetbrains.com/toolbox-app/) - 下载和管理 JetBrains 相关软件

## 字体

字体也是软件体验的一部分，设置时真正的名字是 Windows 设置中字体左上角标题。

[JetBrains Mono](https://www.jetbrains.com/lp/mono/) - 为代码编辑优化的字体，我使用 Bold 粗体

[Nerd Fonts](https://www.nerdfonts.com/) - 终端用字体

[霞鹜文楷](https://github.com/lxgw/LxgwWenKai) - 基于 FONTWORKS 出品字体 Klee One 衍生，另有[屏幕阅读版](https://github.com/lxgw/LxgwWenKai-Screen)

[975 圆体](https://github.com/lxgw/975maru) - 基于思源黑体/狮尾圆体的中文字体

[更纱黑体](https://github.com/be5invis/Sarasa-Gothic) - 基于 [Iosevka](https://github.com/be5invis/Iosevka) 和[思源黑体](https://github.com/adobe-fonts/source-han-sans) 的中文字体

## Android

[纯纯写作](https://writer.drakeet.com/) - 绝不丢失文本编辑器，电脑版可以在局域网下编辑手机里的文章，我把它作为共享文字的剪贴板

[Via](https://viayoo.com/en/) - 极简浏览器，基于系统 webview，可以在[这里](http://via-app.cn)安装插件扩展功能

[Material Files](https://github.com/zhanghai/MaterialFiles) - Material Design 文件管理器

[Kiwi Browser](https://github.com/kiwibrowser) - 浏览器，支持加载桌面扩展

## 在线服务

[Todoist](https://todoist.com/) - To-Do

[Notion](https://www.notion.so) - 笔记

[TinyPNG](https://tinypng.com/) - 图片压缩

[Squoosh](https://squoosh.app/) - 图片压缩

[Raindrop](https://raindrop.io/) - 书签

[SM.MS](https://sm.ms/)- 图床

# 其他

[qBittorrent](https://www.qbittorrent.org/) - BitTorrent 下载，有基于它的修改版本[qBittorrent Enhanced Edition](https://github.com/c0re100/qBittorrent-Enhanced-Edition)

[OBS Studio](https://obsproject.com/) - 直播和录屏，是做主播必备的推流软件，单纯用来录屏也可以

[DaVinci Resolve](http://www.blackmagicdesign.com/products/davinciresolve/) - 专业视频制作工具，影视飓风提供了入门的教程

[LosslessCut](https://github.com/mifi/lossless-cut) - 无损剪辑

[HandBrake](https://handbrake.fr/) - 视频压制

[GeForce Experience](https://www.nvidia.com/en-us/geforce/geforce-experience/) -    Nvidia 显卡独占的驱动支持软件，具有录屏和即时重放功能

[Moonlight](https://moonlight-stream.org/) - 游戏串流，需要 Nvidia 显卡

[Genymotion](https://www.genymotion.com/) - Android 模拟器，依赖 Virtual Box

[Virtual Box](https://www.virtualbox.org/) - 虚拟机

[KDE Connect](https://kdeconnect.kde.org/) - 支持全平台，不同设备之间传输文件和控制等功能

[waifu2x-caffe](https://github.com/lltcggie/waifu2x-caffe) - waifu2x 的 GUI，图像超分

[哔哔](https://www.microsoft.com/store/productId/9PP3TX824G8L) - B 站 UWP 客户端