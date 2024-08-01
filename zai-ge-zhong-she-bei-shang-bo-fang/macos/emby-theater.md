# Emby Theater

### 下载并安装 Emby Theater[​](https://embywiki.911997.xyz/docs/usage/macos/emby-theater/#%E4%B8%80%E3%80%81%E4%B8%8B%E8%BD%BD%E5%B9%B6%E5%AE%89%E8%A3%85-emby-theater) <a href="#yi-xia-zai-bing-an-zhuang-embytheater" id="yi-xia-zai-bing-an-zhuang-embytheater"></a>

下载 [EmbyTheater.zip](https://github.com/rartv/EmbyPublic/releases/download/0.0.33/EmbyTheater.zip) 解压出 `Emby Theater.app`，拖到 `应用程序` 文件夹里

> 应用源码：[https://github.com/thura10/emby-theater-electron](https://github.com/thura10/emby-theater-electron)

### 安装 mpv[​](https://embywiki.911997.xyz/docs/usage/macos/emby-theater/#%E4%BA%8C%E3%80%81%E5%AE%89%E8%A3%85-mpv) <a href="#er-an-zhuang-mpv" id="er-an-zhuang-mpv"></a>

Copy

```
brew install --HEAD mpv
```

### 替换 libass[​](https://embywiki.911997.xyz/docs/usage/macos/emby-theater/#%E4%B8%89%E3%80%81%E6%9B%BF%E6%8D%A2-libass) <a href="#san-ti-huan-libass" id="san-ti-huan-libass"></a>

由于上面安装的 `libmpv` 对于某些中文字幕会乱码，所以下面给出一个解决办法。（原因：[https://zrstea.com/261/](https://zrstea.com/261/)）

**步骤**[**​**](https://embywiki.911997.xyz/docs/usage/macos/emby-theater/#%E6%AD%A5%E9%AA%A4)

1. 下载这个 [libass.rb](https://github.com/rartv/EmbyPublic/releases/download/0.0.33/libass.rb) 这个文件。比如我保存到了系统下载目录 `~/Downloads` 里；
2. 进入下载目录 `cd ~/Downloads`；
3.  卸载安装 `libmpv` 时安装的 `libass`，然后重新编译并安装，命令如下：bash

    Copy

    ```
    brew uninstall libass --ignore-dependencies && brew install fontconfig
    brew install -s libass.rb
    ```

> 以上三个步骤方案来自：[@PANINI](https://t.me/PAN1N1) 和 [@xinzhe he](https://t.me/hexinzhe)

### 客户端解锁[​](https://embywiki.911997.xyz/docs/usage/macos/emby-theater/#%E5%9B%9B%E3%80%81%E5%AE%A2%E6%88%B7%E7%AB%AF%E8%A7%A3%E9%94%81) <a href="#si-ke-hu-duan-jie-suo" id="si-ke-hu-duan-jie-suo"></a>

1. 在 `应用程序` 文件夹中找到 `Emby Theater.app`，右键 `显示包内容`。找到 `Contents/Resources/app/main.js` 文件，用文本编辑器打开；
2. 搜索找到

Copy

```
function getAppBaseUrl() {

    var url = 'https://tv.emby.media';

    //url = 'http://localhost:8088';
    return url;
}
```

替换为

Copy

```
function getAppBaseUrl() {

    var url = 'https://happyemby.911997.xyz';

    //url = 'http://localhost:8088';
    return url;
}
```

保存即可

> 解锁方法来源：[https://neko.re/archives/225.html](https://neko.re/archives/225.html)
