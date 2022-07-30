# 记事本

此处记录下不足以单独成文的内容。

开启了 Lenovo Vantage 中的 电源管理-节电模式，最大充电容量只到 60%

关闭背后的大 Y 灯：`Fn+L`

切换屏幕刷新率：`Fn+R`

开关键盘背光：`Fn+Space`

部署 docsify 遇到的问题

侧边栏无法隐藏或打开 - 将这一行删除 `<script src="//cdn.jsdelivr.net/npm/docsify@4"></script>`

页面无法滚动 - 添加以下代码：

```html
<style type="text/css">
  body {
    overflow: auto !important;
  }
</style>
```

复制代码按钮 - 引入`<script src="//cdn.jsdelivr.net/npm/docsify-copy-code"></script>`

翻页 - [docsify-pagination](https://github.com/imyelo/docsify-pagination)

参考：

- [docsify](https://github.com/docsifyjs/docsify)
- [docsify 中文文档](https://docsify.js.org/#/zh-cn/)
- [Github+docsify 打造在线文档网站 - XiaoJ_c - 博客园](https://www.cnblogs.com/XiaoJ-cs/p/15176475.html)
- [进入多页面后完全无法滚动](https://github.com/docsifyjs/docsify/issues/411)
- [Docsify README page not scrolling](https://stackoverflow.com/questions/63676806/docsify-readme-page-not-scrolling)
- [Wiki 系列（一）：Wiki 系统选择](https://sspai.com/post/60382)
- [Wiki 系列（二）：docsify 部署及配置](https://sspai.com/post/60534)
- [Wiki 系列（三）：我的 Wiki](https://sspai.com/post/60635)

优先使用 val 声明变量，需要时再用 var

`cd docs && python -m SimpleHTTPServer 3000`

`cd docs && python -m http.server 3000`

Run the local server with docsify serve. You can preview your site in your browser on http://localhost:3000.

docsify serve docs

VS Code：让文本超出屏幕自动换行`Editor:Word Wrap`设为 on 将在视口宽度换行，设为 off 则永不自动换行

yt-dlp 选择分辨率：`yt-dlp -S "height:1080"`

Jellyfine