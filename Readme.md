# 视频弹幕终极解决方案

*标签：* 弹幕 解决方案 桌面弹幕 在线视频 离线视频 通用 无敌 牛逼

## 起因

常年游荡在B站的人，往往离不开使视频增色不少的**弹幕**。尤其是某些弹幕极具创造力与幽默感，使得原本空洞的视频展现出完全不同的魅力。

但是，弹幕文化起于B站而终于B站。至今在B站之外的地方，限于品牌定位，企业文化，以及受众人群，使得更多的视频资源缺少了这一乐趣。

而部分弹幕文件，仅适用于本地视频播放器(如Potplayer)。因此想要使用这部分弹幕文件，必须将视频完整下载下来。但鉴于版权问题，与网站流媒体的保护。相当数量的视频无法轻易的获取与下载。这使得这一方案难以实现。

本文立足于此，试图将弹幕以最通用的方式，引入所以平台。因此实现了基于桌面端（QT5）的弹幕程序。只需加载下载的xml/ass弹幕文件，即可同步**任意视频**（本地播放器、网页播放器、任意在线视频等等），享受多倍乐趣。

## 解决方案

实现方案分为两个部分。

第一，寻找弹幕。

弹幕当然来自于互联网群众的创造。大部分是来自于B站原本存在的视频弹幕，由于某些原因（比如周期清理弹幕，或者视频被撤除），而难以被享用。这些弹幕的保存，得益于特别互联网群体的备份，诸如[弹幕保存计划吧](http://tieba.baidu.com/弹幕保存计划)，[弹幕盒子](https://danmubox.github.io/)等。

这些网站提供了众多弹幕的XML格式文件。同时借助一些工具，可以轻易转化为ASS字幕文件，放入普通播放器中。只需下载搜索到的弹幕，便可轻松使用。

本程序目前基于开源[python-ass库](https://github.com/chireiden/python-ass)来解析ASS弹幕文件。

XML文件将在未来版本支持。~（若有需求）~

第二，渲染弹幕到屏幕

屏幕弹幕是目前被认为最佳的解决方案。不依赖于浏览器的版本、内核与播放器种类(HTML5或Flash)。使得弹幕可以在任何环境下轻松使用。同时基于Python+Qt5的渲染体制，使得在程序可以较容易拓展到多平台(Win+Linux+Mac)。

该方案唯一的问题是在于，本地弹幕与视频难以进行直接的匹配和校准。因此程序提供了直接的弹幕时间轴移动功能（暂无，赞请通过移动视频的方式来校准）。同时由于一个视频往往只需要进行一次校准，对于可以享受快乐弹幕的人们来说，不过是轻而易举。

## 使用步骤

0. 打开视频

1. 下载弹幕

2. 下载[最新版本](https://github.com/imhlq/Danmu-project/releases)

3. 打开并加载弹幕文件

4. 享受视频与弹幕


## 有问题请加入

> xhou水友群：294462443

> 关注 [xhou博客](https://xhou.me/)

---

*本权所有，禁止被用于商业用途。违者必究。*