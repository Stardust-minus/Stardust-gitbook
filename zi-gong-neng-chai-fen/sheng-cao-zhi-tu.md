---
description: 基于Skiko的奇怪的图片生成器。
---

# 生草制图

{% embed url="https://github.com/cssxsh/meme-helper#readme" %}
仓库地址
{% endembed %}

本项目会长期不定时更新功能。

### 目前可用的生成器:



*   #### PornHub

    PornHub Login 生成

    示例: `#ph Git Hub`\
    [![pornhub](https://github.com/cssxsh/meme-helper/raw/main/example/pornhub.png)](https://github.com/cssxsh/meme-helper/blob/main/example/pornhub.png)

    #### PetPet

    摸摸头生成

    可以发送 `图片` 或者 `@某人` 或者 `QQ号` 确定卡片图片\
    示例: `#pet @群主`, `#pet 123456`\
    [![petpet](https://github.com/cssxsh/meme-helper/raw/main/example/petpet.gif)](https://github.com/cssxsh/meme-helper/blob/main/example/petpet.gif)

    #### Dear

    狂亲表情包生成

    可以发送 `图片` 或者 `@某人` 或者 `QQ号` 确定卡片图片\
    示例: `#dear @群主`, `#dear 123456`\
    [![dear](https://github.com/cssxsh/meme-helper/raw/main/example/dear.gif)](https://github.com/cssxsh/meme-helper/blob/main/example/dear.gif)

    #### 5000choyen

    5000choyen 表情包生成

    示例: `#choyen 我想吃 肯德基疯狂星期四套餐`\
    [![5000choyen](https://github.com/cssxsh/meme-helper/raw/main/example/5000choyen.png)](https://github.com/cssxsh/meme-helper/blob/main/example/5000choyen.png)

    #### zzkia

    诺基亚短信 表情包生成

    示例: `#pinyin 无内鬼，来点色图`\
    [![zzkia](https://github.com/cssxsh/meme-helper/raw/main/example/zzkia.png)](https://github.com/cssxsh/meme-helper/blob/main/example/zzkia.png)

    #### 游戏王

    游戏王 表情包生成 可以发送 `图片` 或者 `@某人` 或者 `QQ号` 确定卡片图片\
    可以使用 `xxx=yyy`, 指定属性，可选属性有：

    * 卡片名称: `name`
    * 怪兽属性: `attr` = `dark, divine, earth, fire, light, spell, trap, water, wind`
    * 怪兽等级: `level`
    * 怪兽种族: `race`
    * 怪兽攻击: `atk`
    * 怪兽防御: `def`
    * 卡片版权：`copyright`

    示例:

    ```
    #spell @Him188
    name=Welcome PR
    你可以PR
    ```

    [![spell](https://github.com/cssxsh/meme-helper/raw/main/example/spell.png)](https://github.com/cssxsh/meme-helper/blob/main/example/spell.png)

    ```
    #trap @Him188
    name=Useless PR
    这个还是由我们自己实现
    ```

    [![trap](https://github.com/cssxsh/meme-helper/raw/main/example/trap.png)](https://github.com/cssxsh/meme-helper/blob/main/example/trap.png)

    ```
    #monster @LaoLittle
    name=援交JD
    五元一次
    ```

    [![monster](https://github.com/cssxsh/meme-helper/raw/main/example/monster.png)](https://github.com/cssxsh/meme-helper/blob/main/example/monster.png)

    #### 随机表情包

    随机表情包一张（通过 Mirai Hibernate Plugin 插件 从消息中收集得到）

    示例: `#群友表情`

    #### Emoji合成

    Google Emoji Kitchen，两个 emoji 合成 一个

    示例: `😍+🥵`\
    [![u1f60d\_u1f975.png](https://camo.githubusercontent.com/a1d64191ba8951c6c62db23d5d491f60aee58a28a6eacb187f51df23f2ed97dd/68747470733a2f2f7777772e677374617469632e636f6d2f616e64726f69642f6b6579626f6172642f656d6f6a696b69746368656e2f32303230313030312f7531663630642f7531663630645f7531663937352e706e67)](https://camo.githubusercontent.com/a1d64191ba8951c6c62db23d5d491f60aee58a28a6eacb187f51df23f2ed97dd/68747470733a2f2f7777772e677374617469632e636f6d2f616e64726f69642f6b6579626f6172642f656d6f6a696b69746368656e2f32303230313030312f7531663630642f7531663630645f7531663937352e706e67)

    #### 幻影坦克

    需要 `mirai-skia-plugin` 版本 `1.1.9+`

    ```
    #tank
    [图片]
    [图片]
    ```

    [![tank](https://github.com/cssxsh/meme-helper/raw/main/example/tank.png)](https://github.com/cssxsh/meme-helper/blob/main/example/tank.png)
