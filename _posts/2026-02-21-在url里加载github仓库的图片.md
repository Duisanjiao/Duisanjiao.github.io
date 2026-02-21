---
title: 在url里加载github仓库的图片
date: 2026-02-21 20:40:00 +0900
categories: [URL]
tags: [url_load, github]
author: TrianglePile(Duisanjiao)
---

在搭建我的笔记记录网站时，我要载入图片作为头像。

我开始直接尝试用图片的 *URL* 载入。

'''html
<img src="https://github.com/Duisanjiao/Duisanjiao.github.io/blob/main/assets/img/avatar.png" width="112" height="112" alt="avatar" onerror="this.style.display='none'" style="display: none;">
'''

但图片没有显示，如果直接在浏览器访问链接，打开的是github对该文件的预览，本质是一个 *html* 网页。

想要访问原始数据，可以用 **raw** 链接，比如上方的链接可以改为：

'''html
<img src="https://raw.githubusercontent.com/Duisanjiao/Duisanjiao.github.io/main/assets/img/avatar.png" width="112" height="112" alt="avatar" onerror="this.style.display='none'" style="display: none;">
'''

可以直接访问原始数据。

