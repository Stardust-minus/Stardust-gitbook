---
description: 支持QQ音乐、酷狗、千千、网易、网易电台、B站音频等平台。
---

# 点歌

{% embed url="https://github.com/khjxiaogu" %}
作者
{% endembed %}

{% embed url="https://github.com/khjxiaogu/MiraiSongPlugin" %}
项目地址
{% endembed %}

## 点歌默认以XML卡片方式发送，请不要过度使用，避免星尘被封。

## 默认指令列表

### “#音乐 关键词”

自动搜索所有源以找出来找最佳音频来源

### “#语音 关键词”

自动搜索所有源，以语音信息的形式发出

### “#外链 关键词”

自动搜索所有源，以外链信息的形式发出

### “#QQ 关键词”

搜索QQ音乐

### “#网易 关键词”

搜索网易云音乐

### “#网易电台 关键词”

搜索网易云电台，一般来说是直接选择找到的第一个节目，但是关键词可以以 “电台名称|节目名称”的格式指定电台节目

### “#酷狗 关键词”

搜索酷狗音乐

### “#千千 关键词”

搜索千千音乐（百度音乐）

### “#点歌 来源 外观 关键词”

实验性API\
高度自定义的点歌方法

| 参数 | 值范围                                                                                                                                                                                                                                                                                   | 用途           |
| -- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| 来源 | <p>QQ音乐<br>酷狗<br>千千<br>喜马拉雅<br>网易<br>网易HQ<br>网易电台<br>网易电台节目<br>Bilibili<br>本地</p>                                                                                                                                                                                                     | 设定搜索歌曲的来源    |
| 外观 | <p>LightApp:小程序分享<br>Mirai:采用Mirai的MusicShare卡片，如果不存在则fallback为XML卡片<br>XML:卡片分享<br>Share:普通分享(不能播放)<br>Message:以纯信息形式分享，可以很方便取得音乐的各种链接。<br>AMR:AMR语音，需要配置好<code>ffmpeg_path</code><br>Silk:SILK语音，需要同时配置好<code>silkenc_path</code>和<code>ffmpeg_path</code>，由于tx限流，质量可能很差（不推荐使用）</p> | 设定分享出来的音乐的外观 |

## 歌曲API说明

* 网易电台和网易电台节目的区别是网易电台不能用“电台名称|节目名称”的格式。
* 网易HQ的API和QQ音乐API均可能有时间限制，长时间后播放链接会失效。
* bilibili的API由于有请求校验，所以只支持语音播放，卡片分享只支持点击卡片打开网页进行播放。
