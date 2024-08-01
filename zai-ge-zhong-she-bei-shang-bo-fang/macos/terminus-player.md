---
description: Terminus Player 介绍
---

# Terminus Player

本播放器是终点站大佬基于 [Jellyfin-media-player 项目](https://github.com/jellyfin/jellyfin-media-player) 修改的一款播放器，主要特点是：

* 对原项目不支持 Emby 进行了修改，使得绝大部分功能能够正常使用；
* 界面更加美观；
* 安装、使用轻盈方便，两键（双击）安装，即可使用。

> 这是一个修改版的软件，如果报木马，提示有害软件，自行验证是否可安装。设备爆炸不负责任。

### 软件安装[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E8%BD%AF%E4%BB%B6%E5%AE%89%E8%A3%85) <a href="#ruan-jian-an-zhuang" id="ruan-jian-an-zhuang"></a>

从本播放器的 [github release 页面](https://github.com/Terminus-Media/jellyfin-media-player/releases) 下载安装包，如下图所示。认准后缀为 `.app.zip` 的文件，点击下载。下载完成后解压得到 `Terminus Player.app` 文件，即完成。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_1.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=31e56b9d\&sv=1)

双击打开解压得到的文件，首次打开需要信任，单击打开选项。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_2.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=8bc74608\&sv=1)

### 安全性与隐私[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E5%AE%89%E5%85%A8%E6%80%A7%E4%B8%8E%E9%9A%90%E7%A7%81) <a href="#an-quan-xing-yu-yin-si" id="an-quan-xing-yu-yin-si"></a>

macOS 系统默认仅允许 AppStore 来源的 App 运行，打开前请确认 左上角苹果 logo -> 系统设置 -> 安全性与隐私 -> 通用 -> 允许从以下位置下载的App 中勾选的为任何来源。（**点击左下角锁头进行更改**）

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_3.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=d93d2b9b\&sv=1)

### 意外退出和闪退的解决方法[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E6%84%8F%E5%A4%96%E9%80%80%E5%87%BA%E5%92%8C%E9%97%AA%E9%80%80%E7%9A%84%E8%A7%A3%E5%86%B3%E6%96%B9%E6%B3%95) <a href="#yi-wai-tui-chu-he-shan-tui-de-jie-jue-fang-fa" id="yi-wai-tui-chu-he-shan-tui-de-jie-jue-fang-fa"></a>

部分比较干净的系统，由于缺少一些关键位置的文件夹，导致会出现 _意外退出_ 或 _闪退_ 的情况，解决方法如下：

* 在 _工具(Utilities)_ 中，找到并打开 _终端(Terminal)_

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_3.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=d93d2b9b\&sv=1)

*   在打开的 _终端(Terminal)_ 中，输入如下命令

    Copy

    ```
    sudo mkdir /usr/local/etc; sudo chown -R `id -un`:staff /usr/local/etc
    ```
*   输入命令后按下回车，会提示输入用户密码，此处输入密码不会显示，密码输入后回车确认

    ![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_4.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=c3b4b14e\&sv=1)
* 重新打开_Terminus Player_已经可以正常打开并进入下一步的使用环节了

### 软件使用[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E8%BD%AF%E4%BB%B6%E4%BD%BF%E7%94%A8) <a href="#ruan-jian-shi-yong" id="ruan-jian-shi-yong"></a>

#### 添加服务器[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E6%B7%BB%E5%8A%A0%E6%9C%8D%E5%8A%A1%E5%99%A8) <a href="#tian-jia-fu-wu-qi" id="tian-jia-fu-wu-qi"></a>

打开 App 后，进入如下界面。在红框处输入PiliPili给你的地址（**包含端口号，用英文冒号连接**），然后点击连接。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_5.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=a2be6109\&sv=1)

输入用户名和密码，点击登录。即可开始观影

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_6.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=3e1434a4\&sv=1)

#### 修改语言[​](https://embywiki.911997.xyz/docs/usage/macos/terminus-player/basic/#%E4%BF%AE%E6%94%B9%E8%AF%AD%E8%A8%80) <a href="#xiu-gai-yu-yan" id="xiu-gai-yu-yan"></a>

进入服务器后，点击右上角小人图标，选择 Display 项，单击进入。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_7.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=7320867\&sv=1)

单击 Display Language 下方单选框，选择需要修改的语言。简体中文为 `Chinese(Simplified)`。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_8.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=6f3002ca\&sv=1)

然后页面向下滑到底，点击底部 Save 按钮保存设置。左下角出现 Settings saved 字样即表示保存成功。此时关闭 App 重启，即可变为简体中文界面。

![](https://pilipili.gitbook.io/\~gitbook/image?url=https%3A%2F%2Fgithub.com%2Fhsuyelin%2FPiliPili%2Fblob%2Fmain%2Fsrc%2Fimages%2Fmacos\_terminus\_connect\_10.png%3Fraw%3Dtrue\&width=768\&dpr=4\&quality=100\&sign=8f1f8a09\&sv=1)

> 当你修改为简体中文界面之后，相信你已经可以自行玩转这个 App 了，其余设置与 Emby 官方客户端基本相同。
