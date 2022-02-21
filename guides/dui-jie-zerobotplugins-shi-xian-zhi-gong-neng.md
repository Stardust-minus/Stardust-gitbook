---
description: 发送 /服务列表 来查看星尘所启用的功能。
---

# 对接ZeroBot-Plugin实现之功能

{% embed url="https://github.com/FloatTech/ZeroBot-Plugin" %}
使用Onebot-kotlin对接ZeroBot-Plugin实现。
{% endembed %}

{% hint style="info" %}
星尘的ZeroBot-Plugin会**不定期**同步上游更新。并且某些功能不会启用。
{% endhint %}

星尘的大部分自定义回复依托于ZeroBot-Plugin的chat，atri插件。如果您不需要这些回复的话请分别在群内使用以下指令:

### /禁用 atri    /禁用 chat

由于Api服务器故障，coser，图片放大功能不可用。

以下是目前启用的服务列表（行首使用//注释的为未启用）

![](../.gitbook/assets/5\_5}RFSAPBV\(IS\[\`DOF0O1G.png)

![](../.gitbook/assets/@0VDHIKZ{QDW$M\(1H\~L\[\)KA.png)





从Github复制来的

* **插件控制**
  * [x] &#x20;/启用 xxx (在发送的群/用户启用xxx)
  * [x] &#x20;/禁用 xxx (在发送的群/用户禁用xxx)
  * [x] &#x20;/全局启用 xxx
  * [x] &#x20;/全局禁用 xxx
  * [x] &#x20;/还原 xxx (在发送的群/用户还原xxx的开启状态到初始状态)
  * [x] &#x20;/禁止 service qq1 qq2... (禁止 qqs 使用服务 service)
  * [x] &#x20;/允许 service qq1 qq2... (重新允许 qqs 使用服务 service)
  * [x] &#x20;/封禁 qq1 qq2... (禁止 qqs 使用全部服务)
  * [x] &#x20;/解封 qq1 qq2... (允许 qqs 使用全部服务)
  * [x] &#x20;/用法 xxx
  * [x] &#x20;/服务列表
  * [x] &#x20;/服务详情
  * [x] &#x20;@Bot 插件冲突检测 (会在本群发送一条消息并在约 1s 后撤回以检测其它同类 bot 中已启用的插件并禁用)
* **聊天** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_chat"`
  * [x] &#x20;\[BOT名字]
  * [x] &#x20;\[戳一戳BOT]
  * [x] &#x20;空调开
  * [x] &#x20;空调关
  * [x] &#x20;群温度
  * [x] &#x20;设置温度\[正整数]
* **词典匹配回复** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_thesaurus"`
  * [x] &#x20;@Bot 关键词
* **ATRI** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_atri"`
  * [x] &#x20;具体指令看 /用法 atri
  * [ ] 注：本插件基于 [ATRI](https://github.com/Kyomotoi/ATRI) ，为 Golang 移植版
* **群管** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_manager"`
  * [x] &#x20;禁言\[@xxx]\[分钟]
  * [x] &#x20;解除禁言\[@xxx]
  * [x] &#x20;我要自闭 | 禅定 x \[分钟 | 小时 | 天]
  * [x] &#x20;开启全员禁言
  * [x] &#x20;解除全员禁言
  * [x] &#x20;升为管理\[@xxx]
  * [x] &#x20;取消管理\[@xxx]
  * [x] &#x20;修改名片\[@xxx]\[xxx]
  * [x] &#x20;修改头衔\[@xxx]\[xxx]
  * [x] &#x20;申请头衔\[xxx]
  * [x] &#x20;踢出群聊\[@xxx]
  * [x] &#x20;退出群聊\[群号]@Bot
  * [x] &#x20;\*入群欢迎
  * [x] &#x20;\*退群通知
  * [x] &#x20;设置欢迎语\[欢迎\~]
  * [x] &#x20;在\[MM]月\[dd]日的\[hh]点\[mm]分时(用\[url])提醒大家\[xxx]
  * [x] &#x20;在\[MM]月\[每周 | 周几]的\[hh]点\[mm]分时(用\[url])提醒大家\[xxx]
  * [x] &#x20;取消在\[MM]月\[dd]日的\[hh]点\[mm]分的提醒
  * [x] &#x20;取消在\[MM]月\[每周 | 周几]的\[hh]点\[mm]分的提醒
  * [x] &#x20;在"cron"时(用\[url])提醒大家\[xxx]
  * [x] &#x20;取消在"cron"的提醒
  * [x] &#x20;列出所有提醒
  * [x] &#x20;翻牌
  * [x] &#x20;\[开启 | 关闭]入群验证
  * [x] &#x20;\[开启 | 关闭]gist加群自动审批
  * [ ] &#x20;同意好友请求
  * [ ] &#x20;撤回\[@xxx] \[xxx]
  * [ ] &#x20;警告\[@xxx]
  * [x] &#x20;run\[xxx]
  * [ ] 注：使用gist加群自动审批，请在群介绍添加以下说明，同时开启`需要回答问题并由管理员审核`：加群请在github新建一个gist，其文件名为本群群号的字符串的md5(小写)，内容为一行，是当前unix时间戳(10分钟内有效)。然后请将您的用户名和gist哈希(小写)按照username/gisthash的格式填写到回答即可。
* **GitHub仓库搜索** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_github"`
  * [x] &#x20;\>github \[xxx]
  * [x] &#x20;\>github -p \[xxx]
* **在线代码运行** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_runcode"`
  * [x] &#x20;\> runcode \[language] help
  * [x] &#x20;\> runcode \[language] \[code block]
* **点歌** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_music"`
  * [x] &#x20;点歌\[xxx]
  * [x] &#x20;网易点歌\[xxx]
  * [x] &#x20;酷我点歌\[xxx]
  * [x] &#x20;酷狗点歌\[xxx]
* **shindan** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_shindan"`
  * [x] &#x20;今天是什么少女\[@xxx]
  * [x] &#x20;异世界转生\[@xxx]
  * [x] &#x20;卖萌\[@xxx]
  * [x] &#x20;抽老婆\[@xxx]
* **AIWife** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_aiwife"`
  * [x] &#x20;waifu | 随机waifu(从[100000个AI生成的waifu](https://www.thiswaifudoesnotexist.net)中随机一位)
* **gif** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_gif"`
  * [x] &#x20;爬\[@xxx]
  * [x] &#x20;摸\[@xxx]
  * [x] &#x20;搓\[@xxx]
  * [ ] 注：更多指令见项目 --> [https://github.com/FloatTech/ZeroBot-Plugin-Gif](https://github.com/FloatTech/ZeroBot-Plugin-Gif)
* **base16384加解密** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_b14"`
  * [x] &#x20;加密xxx
  * [x] &#x20;解密xxx
  * [x] &#x20;用yyy加密xxx
  * [x] &#x20;用yyy解密xxx
* **摸鱼** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_moyu"`
  * [x] &#x20;/启用 moyu
  * [x] &#x20;/禁用 moyu
* **涩图** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_setutime"`
  * [x] &#x20;来份\[涩图/二次元/风景/车万]
  * [x] &#x20;添加\[涩图/二次元/风景/车万]\[P站图片ID]
  * [x] &#x20;删除\[涩图/二次元/风景/车万]\[P站图片ID]
  * [x] &#x20;\> setu status
* **本地涩图** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_nativesetu"`
  * [x] &#x20;本地\[xxx]
  * [x] &#x20;刷新本地\[xxx]
  * [x] &#x20;设置本地setu绝对路径\[xxx]
  * [x] &#x20;刷新所有本地setu
  * [x] &#x20;所有本地setu分类
  * [ ] 注：刷新文件夹较慢，请耐心等待刷新完成，会提示“成功”。
* **nsfw图片识别** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_nsfw"`
  * [x] &#x20;nsfw打分\[图片]
  * [x] &#x20;当图片属于非 neutral 类别时自动发送评价(默认禁用，启用输入 /启用 nsfwauto)
* **lolicon** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_lolicon"`
  * [x] &#x20;来份萝莉
* **搜图** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_saucenao"`
  * [x] &#x20;以图搜图 | 搜索图片 | 以图识图\[图片]
  * [x] &#x20;搜图\[P站图片ID]
* **搜番** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_tracemoe"`
  * [x] &#x20;搜番 | 搜索番剧\[图片]
* **随机图片与AI点评** `import _ github.com/FloatTech/ZeroBot-Plugin/plugin_acgimage`
  * [x] &#x20;随机图片(评级大于6的图将私发)
  * [x] &#x20;直接随机(无r18检测，务必小心，仅管理可用)
  * [x] &#x20;设置随机图片网址\[url]
  * [x] &#x20;太涩了(撤回最近发的图)
  * [x] &#x20;评价图片(发送一张图片让bot评分)
* **DeepDanbooru二次元图标签识别** `import _ github.com/FloatTech/ZeroBot-Plugin/plugin_danbooru`
  * [x] &#x20;鉴赏图片\[图片]
* **叔叔的AI二次元图片放大** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_scale"`
  * [x] &#x20;放大图片\[图片]
* **每日运势** `import _ github.com/FloatTech/ZeroBot-Plugin/plugin_fortune`
  * [x] &#x20;运势 | 抽签
  * [x] &#x20;设置底图\[车万 DC4 爱因斯坦 星空列车 樱云之恋 富婆妹 李清歌 公主连结 原神 明日方舟 碧蓝航线 碧蓝幻想 战双 阴阳师 赛马娘]
* **睡眠管理** `import _ github.com/FloatTech/ZeroBot-Plugin/plugin_sleep_manage`
  * [x] &#x20;早安 | 晚安
* **浅草寺求签** `import _ github.com/FloatTech/ZeroBot-Plugin/plugin_omikuji`
  * [x] &#x20;求签 | 占卜
  * [x] &#x20;解签
* **漂流瓶** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_drift_bottle"`
  * [x] &#x20;(在群xxx)丢漂流瓶(到频道xxx) \[消息]
  * [x] &#x20;(从频道xxx)捡漂流瓶
  * [x] &#x20;@BOT 创建频道 xxx
  * [x] &#x20;跳入(频道)海中
  * [x] &#x20;注：不显式限制时，私聊发送可在所有群抽到，群聊发送仅可在本群抽到，默认频道为 global
* **bilibili** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_bilibili"`
  * [x] &#x20;\>vup info \[名字 | uid]
  * [x] &#x20;\>user info \[名字 | uid]
  * [x] &#x20;/开启粉丝日报
* **嘉然** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_diana"`
  * [x] &#x20;小作文
  * [x] &#x20;发大病
  * [x] &#x20;教你一篇小作文\[作文]
  * [x] &#x20;\[回复]查重
* **鬼东西** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_wtf"`
  * [x] &#x20;鬼东西列表
  * [x] &#x20;查询鬼东西\[序号]\[@xxx]
  * [ ] 注：由于需要科学，默认注释。
* **AIfalse** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_ai_false"`
  * [x] &#x20;查询计算机当前活跃度: \[检查身体 | 自检 | 启动自检 | 系统状态]
  * [x] &#x20;清理缓存 (仅适用于 gocq 且需要 bot 的运行目录和 gocq 相同)
  * [ ] &#x20;简易语音
  * [ ] &#x20;爬图合成 \[@xxx]
* **抽wife** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_nativewife"`
  * [x] &#x20;抽wife\[@xxx]
  * [x] &#x20;添加wife\[名字]\[图片]
  * [x] &#x20;删除wife\[名字]
  * [x] &#x20;\[让 | 不让]所有人均可添加wife
  * [ ] 注：不同群添加后不会重叠
* **minecraft** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_minecraft"`
  * [x] &#x20;/mcstart xxx
  * [x] &#x20;/mcstop xxx
  * [x] &#x20;/mclist servername
  * [ ] 注：此功能实现依赖[MCSManager](https://github.com/Suwings/MCSManager)项目对服务器的管理api，mc服务器如果没有在该管理平台部署此功能无效
* **炉石** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_hs"`
  * [x] &#x20;搜卡\[xxxx]
  * [x] &#x20;\[卡组代码xxx]
  * [ ] 注：更多搜卡指令参数：[https://hs.fbigame.com/misc/searchhelp](https://hs.fbigame.com/misc/searchhelp)
* **人工智能回复** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_ai_reply"`
  * [x] &#x20;@Bot 任意文本(任意一句话回复)
  * [x] &#x20;设置回复模式\[青云客 | 小爱]
* **关键字搜图** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_image_finder"`
  * [x] &#x20;来张 \[xxx]
* **拼音首字母释义工具** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_nbnhhsh"`
  * [x] &#x20;?? \[缩写]
* **选择困难症帮手** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_choose"`
  * [x] &#x20;选择\[选择项1]还是\[选项2]还是\[更多选项]
* **投胎** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_reborn"`
  * [x] &#x20;reborn
  * [ ] 注：本插件来源于[tgbot](https://github.com/YukariChiba/tgbot/blob/main/modules/Reborn.py)
* **翻译** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_translation"`
  * [x] &#x20;\>TL 你好
* **vtb语录** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_vtb_quotation"`
  * [x] &#x20;vtb语录
  * [x] &#x20;随机vtb
  * [x] &#x20;更新vtb
* **书评** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_book_review"`
  * [x] &#x20;书评\[xxx]
  * [x] &#x20;随机书评
* **coser** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_coser"`
  * [x] &#x20;coser
* **小说** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_novel"`
  * [x] &#x20;小说\[xxx]
* **沙雕app插件** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_shadiao"`
  * [x] &#x20;哄我
  * [x] &#x20;渣我
  * [x] &#x20;来碗绿茶
  * [x] &#x20;发个朋友圈
  * [x] &#x20;来碗毒鸡汤
  * [x] &#x20;讲个段子
* **笑话** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_funny"`
  * [x] &#x20;讲个笑话\[@xxx] | 讲个笑话\[qq号]
* **抽象话** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_chouxianghua"`
  * [x] &#x20;抽象翻译\[xxx]
* **合成emoji** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_emojimix"`
  * [x] &#x20;\[emoji]\[emoji]
* **绝绝子** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_juejuezi"`
  * [x] &#x20;喝奶茶绝绝子 | 绝绝子吃饭
* **藏头诗** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_cangtoushi"`
  * [x] &#x20;藏头诗\[xxx]
  * [x] &#x20;藏尾诗\[xxx]
* **cp短打** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_cpstory"`
  * [x] &#x20;组cp\[@xxx]\[@xxx]
  * [x] &#x20;磕cp大老师 雪乃
* **签到得分** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_score"`
  * [x] &#x20;签到
  * [x] &#x20;获得签到背景\[@xxx] | 获得签到背景
* **骂人** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_curse"`
  * [x] &#x20;骂我
  * [x] &#x20;大力骂我
* **b站推送** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_bilibili_push"`
  * [x] &#x20;添加订阅\[uid]
  * [x] &#x20;取消订阅\[uid]
  * [x] &#x20;取消动态订阅\[uid]
  * [x] &#x20;取消直播订阅\[uid]
  * [x] &#x20;推送列表
* **网易云音乐热评** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_wangyiyun"`
  * [x] &#x20;来份网易云热评
* **b站视频链接解析** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_bilibili_parse"`
  * [x] &#x20;[https://www.bilibili.com/video/BV1xx411c7BF](https://www.bilibili.com/video/BV1xx411c7BF) | [https://www.bilibili.com/video/av1605](https://www.bilibili.com/video/av1605) | [https://b23.tv/I8uzWCA](https://b23.tv/I8uzWCA) | [https://www.bilibili.com/video/bv1xx411c7BF](https://www.bilibili.com/video/bv1xx411c7BF)
* **煎蛋网无聊图** `import _ "github.com/FloatTech/ZeroBot-Plugin/plugin_jandan"`
  * [x] &#x20;来份屌图
  * [x] &#x20;更新屌图
* **TODO...**
