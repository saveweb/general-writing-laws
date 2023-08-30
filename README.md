# 通用写作律法

```yaml
标题: 通用写作律法
创建时间: 2023年8月26日
版本: 0.0.13-beta
```

<ruby>通用写作律法<rp>(</rp><rt>General Writing Laws</rt><rp>)</rp></ruby>是由
[Save The Web Project][] 设计的开放律法（标准），后文简称为《律法》。

[Save The Web Project]: https://github.com/saveweb

《律法》有多种设想的使用场景，分别是：

1.  阅读：寻找适合自己的写作规则。
2.  使用：完善自己的写作规则，不再模棱两可。
3.  共享：将精心选配的《律法》规则作为团队的写作规范。

《律法》出现的根本原因，是在不使用专业排版工具的情况时，以及无 CSS 自动优化的时候，
比如在 Twitter, Facebook 以及 Telegram 等地，纯粹的使用文本、符号和空格来让文字排版得美观易读。

并且每个人都有自己的习惯以及美学，要求他人使用某种固定的规范是不太现实的，
所以不如每个人遵守自己精心选配的《律法》，如果团队写作有需求使用相同的规范，
那么使用《律法》模块化的搭建一套规范，也能减少模棱两可的情况。

## 当前《律法》状态

其他书写系统的完整支持，以及《律法》翻译尚未完成。

Full support for other writing system, and _General Writing Laws_ translations are not yet complete.

目前暂未完成各项模块的情况，一定会有编号变动，甚至重构的情况。

## 简介

《律法》是为了将各种书写规范模块化，而诞生的规则，借鉴了一些 [BEP 0000][]（BitTorrent 增强建议索引）的设计。

[BEP 0000]: https://www.bittorrent.org/beps/bep_0.html

并且《律法》兼容多种书写系统，不仅仅是中文主体，而是要打造一套各种书写系统都通用的写作规则，
并且减少特例、例外的情况，让规范简单易懂。

因为《律法》是模块化的，所以可以选配各种不同的规范，然后生成仅包含这些规范的个性化《律法》。

## GWLM 0 通用写作律法模块

```yaml
标题: 通用写作律法模块
创建时间: 2023年8月26日
```

GWLM 0 是收录通用写作律法模块的清单，会收录所有的 GWLM（General Writing Laws Module，
通用写作律法模块）内容，并对可行性进行评议，每条 GWLM 都会被分类，分别是「正式」
「草案」「延期」和「拒绝」。[^bep0]

[^bep0]: 借用了许多 [BEP 0000][]（BitTorrent 增强建议索引）的设计。

### 正式的 GWLM

| 序号        | 标题                       |
| ----------- | -------------------------- |
| [0][gwlm-0] | [通用写作律法模块][gwlm-0] |
| [1][gwlm-1] | [词汇表][gwlm-1]           |
| [2][gwlm-2] | [书写系统空间][gwlm-2]     |
| [3][gwlm-3] | [书写系统规范][gwlm-3]     |
| [4][gwlm-4] | [兼容性][gwlm-4]           |
| [5][gwlm-5] | [表情][gwlm-5]             |

[gwlm-0]: #gwlm-0-通用写作律法模块
[gwlm-1]: #gwlm-1-词汇表
[gwlm-2]: #gwlm-2-书写系统空间
[gwlm-3]: #gwlm-3-书写系统规范
[gwlm-4]: #gwlm-4-兼容性
[gwlm-5]: #gwlm-5-表情

### 草案的 GWLM

| 序号                | 标题                                     |
| ------------------- | ---------------------------------------- |
| [15834][gwlm-15834] | [简体中文标点符号用法模块化][gwlm-15834] |

[gwlm-15834]: #gwlm-15834-简体中文标点符号用法模块化

### 延期的 GWLM

| 序号 | 标题 |
| ---- | ---- |
| 暂无 | 暂无 |

### 拒绝的 GWLM

| 序号 | 标题 |
| ---- | ---- |
| 暂无 | 暂无 |

## GWLM 1 词汇表

```yaml
标题: 词汇表
创建时间: 2023年8月27日
```

为了精确的描述以及理解，此章节用于定义／解释 GWLM 内的词汇。

### 书写系统词汇表

+   GWLM 1-0：书写系统 (writing system)、字符 (character)

    指 Unicode 字符集中的所有字符，包含数字、文字（字母文字、象形文字）、标点符号和其他符号。

    使用方式：描述指向的是某一地区的字符，那么使用书写系统，比如「中文书写系统」「英文书写系统」，
    描述指向的的字符没有地区性质，那么使用字符，比如「全角字符」「半角字符」「所有的字符」「表意字符」

+   GWLM 1-1：数字

    这里是指狭义上的阿拉伯数字，包括半角 0123456789 以及全角０１２３４５６７８９。

+   GWLM 1-2：文字

    这里是指狭义上的文字，属于字符的子集，仅包含字母文字、象形文字等直接表意字符，即字典、
    词典收录的文字。

    使用方式：这里仅对书写系统进行规范，不会涉及狭义的语言，即口语，所以尽量减少「语言」一词，
    比如使用「英文」替代「英语」。

+   GWLM 1-3：标点符号

    详见 [GWLM 15834-2-1 标点符号 (punctuation)](#gwlm-15834-2-1-标点符号-punctuation)。

+   GWLM 1-4：点号（点符号）

    详见 [GWLM 15834-2-6 点号](#gwlm-15834-2-6-点号)。

+   GWLM 1-5 标号（标示符号）

    详见 [GWLM 15834-2-7 标号](#gwlm-15834-2-7-标号)。

## GWLM 2 书写系统空间

```yaml
标题: 书写系统空间
创建时间: 2023年8月26日
```

「书写系统空间」是为文字的不同书写系统划分空间，并为各种部分指定「书写系统属地规范」。

### 划分空间

1.  标示「书名」「数字」以及「计量单位符号」等特殊的情况。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    ```

    备注：GitHub 的代码块并没有严格调用浏览器默认的等款字体，结果会造成排版错位，
    需要回到 GitHub 顶部，然后点击右上角的 Raw 按钮查看原始的等宽内容。

    关于特殊环境的详细处理方式，请参照 GWLM 3-5。

2.  标示外文的「片段环境」：

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

    这些外文片段的书写系统环境被称为「片段环境」。

3.  定义「书写系统环境」：

    通过标题和表意文字都是中文，能够给文章整体设下「简体中文」的「书写系统环境／环境变量」。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    书写系统环境    ·          ·          ·zh-Hans       ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

### 文字属地规范

+   「片段环境」没有占满一句话时，不应该使用「片段环境」的属地语法，比如英语的句首大写。

+   在并列外语词语时，使用「书写系统环境」的属地语法的顿号，比如：

    > 我们的客户有 Yahoo、Facebook, Inc.、Microsoft Corporation 和 Google。

    > Our clients include “百度”, “腾讯”, “金山” and “奇虎360”.

    备注：是否使用引号包围外语，请参考《GWLM 3 兼容性》的〈[各种文字的兼容性](#各种文字的兼容性)〉
    章节。

## GWLM 3 书写系统规范

```yaml
标题: 书写系统规范
创建时间: 2023年8月26日
```

书写系统规范由词典、语法、正字法、标点符号用法标准以及其他细节组成。

+   简体中文以《[GB/T 15834-2011 标点符号用法标准][]》作为标点符号用法标准。

+   繁体中文以《[重訂標點符號手冊][]》作为标点符号用法标准。

[GB/T 15834-2011 标点符号用法标准]: http://www.moe.gov.cn/ewebeditor/uploadfile/2015/01/13/20150113091548267.pdf
[重訂標點符號手冊]: https://language.moe.gov.tw/001/Upload/FILES/SITE_CONTENT/M1/HAU/haushou.htm

其他地区的书写系统基本没有硬性规定的正字法、标点符号用法标准，所以暂不进行定义。

### 可选模块

+   GWLM 3-0：尊重产品名词等专有名词的书写规范。[^ccg_108]

    [^ccg_108]: sgalal, 《[關於中文與英文、中文與數字間添加間距的疑問 · Issue #108 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/108)》, GitHub, 2020-01-27. (参照 2023-08-27).

    产品名词可以参考官方网站、印刷品或者含有名称的地方，然后检查间距或书写情况，如果官方的使用混乱，
    视作没有规范。

    没有作者定义的专有名词，比如「维生素C」「U盘」「USBフラッシュドライブ」这类翻译而来的专有名词，
    视作没有规范。

+   GWLM 3-1：各书写系统的写作方法在能在片段环境中完整生效，例外：

    +   GWLM 3-1-1：句首大写。

+   GWLM 3-2：片段环境会影响首尾有成对的符号，例外：

    +   GWLM 3-2-1：括号。

    +   GWLM 3-2-2：引号。

    +   GWLM 3-2-4：书名号（包括使用斜体标示书名）。

+   GWLM 3-3：单位符号与数字之间需要增加空格，例外：

    +   GWLM 3-3-1：度数，例如 ° ℃ °C。

    +   GWLM 3-3-2：百分号、千分号和万分号，例如 % ％ ‰ ‱。

+   GWLM 3-4：全角与半角字符之间需要增加空格，例外：

    +   GWLM 3-4-1：全角阿拉伯数字。

    +   GWLM 3-4-2：全角标点符号，例如 ， 。 ； 《 等。

    +   GWLM 3-4-4：全角特殊符号，例如 ％ ＊ ￥ ／ 等。

+   GWLM 3-5：「特殊环境」的特殊处理：

    +   GWLM 3-5-0-1：对时间特殊处理（一）：

        将时间视作整体，不为「YYYY」「年」「MM」「月」「DD」「日」之间添加空格，并在前后添加空格，
        演示如下：[^ccg_102]

        [^ccg_102]: undeadway, 《[是否可以明确一下日期的书写格式 · Issue #102 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/102)》, GitHub, 2019-12-25. (参照 2023-08-27).

        > 有条 issues 在 2019 年 12 月 25 日 23 时 20 分 30 秒发布。

        > 有条 issues 在 2019年12月25日 23时20分30秒 发布。

        规则是「年月日」「时分秒」各为一组，如果缺少一个时间单位，依然特殊处理：

        > 有条 issues 在 12月25日 23时20分 发布。

        如果仅有一个时间单位，那么就不进行特殊处理：

        > 有条 issues 在 25 日 23 时发布。

        > 有条 issues 在 12月25日 23 时发布。

    +   GWLM 3-5-0-2：对时间特殊处理（二）：暂未使用的保留编号。

    +   GWLM 3-5-1-1：对链接特殊处理（一）：

        为链接的前后添加空格：

        > 埃佩克斯是位于 [北卡罗来纳州](#/) [韦克县](#/) 的一个镇，属于 [罗利](#/) [郊区](#/) 的一部份。

+   GWLM 3-6：CJK 标点符号替换：

    +   GWLM 3-6-1：替换「简体中文的弯引号」为「全角直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |   “   | `U+201C` |   「   | `U+300C` |
        |   ”   | `U+201D` |   」   | `U+300D` |
        |   ‘   | `U+2018` |   『   | `U+300E` |
        |   ’   | `U+2019` |   』   | `U+300F` |

    +   GWLM 3-6-2：替换「半角间隔号」为「全角间隔号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |   /   | `U+002F` |   ／   | `U+FF0F` |

    +   GWLM 3-6-4：替换「CJK 通用全角括号」为「英文半角括号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  （   | `U+FF08` |   (    | `U+0028` |
        |  ）   | `U+FF09` |   )    | `U+0029` |

    +   GWLM 3-6-8：替换「中日通用全角逗号」为「英文的半角逗号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  ，   | `U+FF0C` |   ,    | `U+002C` |

    +   GWLM 3-6-16：替换「CJK 通用全角句号」为「CJK 通用半角句号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  。   | `U+3002` |   ｡    | `U+FF61` |

    +   GWLM 3-6-32：替换「CJK 通用全角句号」为「英文的半角句号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  。   | `U+3002` |   .    | `U+002E` |

    +   GWLM 3-6-64：替换「全角单层直角引号」为「半角单层直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  「   | `U+300C` |   ｢    | `U+FF62` |
        |  」   | `U+300D` |   ｣    | `U+FF63` |

+   GWLM 3-7：英语标点符号替换：

    +   GWLM 3-7-1：替换「英语的弯引号」为「全角直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |   “   | `U+201C` |   「   | `U+300C` |
        |   ”   | `U+201D` |   」   | `U+300D` |
        |   ‘   | `U+2018` |   『   | `U+300E` |
        |   ’   | `U+2019` |   』   | `U+300F` |

备注：启用 GWLM 3-2 表示同时启用了 GWLM 3, GWLM 3-2；
启用 GWLM 3-4-7，就表示同时启用了 GWLM 3, GWLM 3-4, GWLM 3-4-1, GWLM 3-4-2, GWLM 3-4-4，
原理是部分模块使用 1, 2, 4, 8… 这样的序列递增，其实是二进制的位关系，所以可以相加。

| 十进制 | 二进制 | 含义（启用的模块） |
| ------ | ------ | ------------------ |
| 1      | 1      | 1                  |
| 2      | 10     | 2                  |
| 3      | 11     | 1, 2               |
| 4      | 100    | 4                  |
| 5      | 101    | 1, 4               |
| 6      | 110    | 1, 2               |
| 7      | 111    | 1, 2, 4            |

GWLM 3-6-1 与 GWLM 3-7-1 的结果看起来相同，当其作用的领域不同。GWLM 3-6 作用于 CJK 的标点符号，
即中日韩统一表意文字的标点符号。而 GWLM 3-7 作用于英语的标点符号。

### 示例

下面是启用一些模块后的效果：

| 启用的模块                     | 效果               | 效果                           |
| ------------------------------ | ------------------ | ------------------------------ |
| 原始                           | 用户打开qq音乐     | apple在传记steve jobs          |
| GWLM 3                         | 用户打开qq音乐。   | apple在传记《steve jobs》。    |
| GWLM 3-0                       | 用户打开QQ音乐。   | apple在传记《Steve Jobs》。    |
| GWLM 3-1                       | 用户打开Qq音乐。   | Apple在传记《Steve jobs》。    |
| GWLM 3-2                       | 用户打开qq音乐。   | apple在传记<i>steve jobs</i>。 |
| GWLM 3-4                       | 用户打开 qq 音乐。 | apple 在传记《 steve jobs 》。 |
| GWLM 3-4-3                     | 用户打开 qq 音乐。 | apple 在传记《steve jobs》。   |
| GWLM 3-2, GWLM 3-4-3           | 用户打开 qq 音乐。 | apple 在传记 _steve jobs_。    |
| GWLM 3-0, GWLM 3-2, GWLM 3-4-3 | 用户打开 QQ音乐。  | apple 在传记 _Steve Jobs_。    |

---

如果更改模块的排序，也会导致优先级改变，比如：

| 启用的模块         | 效果               |                              |
| ------------------ | ------------------ | ---------------------------- |
| 原始               | 用户打开qq音乐     | apple在传记steve jobs        |
| GWLM 3             | 用户打开qq音乐。   | apple在传记《steve jobs》。  |
| GWLM 3-0           | 用户打开QQ音乐。   | apple在传记《Steve Jobs》。  |
| GWLM 3-4           | 用户打开 qq 音乐。 | apple 在传记《Steve Jobs》   |
| GWLM 3-0, GWLM 3-4 | 用户打开 QQ音乐。  | apple 在传记《Steve Jobs》。 |
| GWLM 3-4, GWLM 3-0 | 用户打开 QQ 音乐。 | apple 在传记《Steve Jobs》。 |

---

启用 GWLM 3-2 后，如果提到了不同书写系统的作品名，那么需要使用当地书写系统的书名表达方式：

> 我听说过« Beispiel in Frankreich » «Beispiel in der Schweiz» »Beispiel in Deutschland und Österreich«
> 《十万个为什么》『吾輩は猫である』_Steve Jobs_ 这些书名。

分别是法文、瑞士、德国／奥地利、中文、日文和英文的书名号表示方式。[^53627]

[^53627]: 德语世界, 《[【学生园地】德语的引号问题](https://www.sohu.com/a/www.sohu.com/a/289535110_653627)》, 搜狐新闻／搜狐号, 2019-01-16. (参照 2023-08-26).

## GWLM 4 兼容性

```yaml
标题: 兼容性
创建时间: 2023年8月26日
```

### 各种文字的兼容性

各地文字之间存在兼容性，比如 DNA、NBA 和 FPS 这些英文缩写，以及 Apple、Google 和 Microsoft 这些知名公司，
都已经成为了事实上的中文 [外来语](https://zh.wikipedia.org/wiki/外来语)。属于直接使用的外来词，
就像是香港常用的张 Sir 来表示张先生一样，没有使用引号标示的必要。

但是如果是中文、俄文或者日文，出现在英文环境，就需要使用引号包围了。

### 兼容其他规范

简介里有提到因为《律法》是模块化的，所以可以选配各种不同的规范，所以现有的排版规范也可以使用《律法》来实现。

《[中文文案排版指北][]》是相当知名的中文文案、排版方案，可以通过启用部分《律法》模块来兼容《指北》，
具体是 GWLM 3-0, GWLM 3-1, GWLM 3-2-3, GWLM 3-3-3, GWLM 3-4-3, GWLM 3-6-1。

[中文文案排版指北]: https://github.com/sparanoid/chinese-copywriting-guidelines

## GWLM 5 表情

```yaml
标题: 表情
创建时间: 2023年8月27日
```

文字表情有多种形式，包括「假借文字表情」、颜文字和 Emoji 等等。

表情特殊的地方在于，可作为句号使用，例如：[^ccg_47]

[^ccg_47]: CatTail, 《[如何处理表情文本 · Issue #47 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/47)》, GitHub, 2016-10-01. (参照 2023-08-27).

> 今天出去 🛒，身上的 💰 竟然掉了，非常的 😫
>
> _(GWLM 3-4, GWLM 5)_

### 假借文字表情

在一些论坛，会在输入文字排版时，使用「233」或者「(bgm38)」这样的纯文本进行调用相应的表情图片，
比如「233」属于猫扑的 233 号表情，在输入时需要输入 233 这样的文字，久而久之 233 就获得了原本表情的含义。

「bgm38」也是相同的情况，这是 Bangumi 的第 38 号表情，可以在发布文字的框体中输入「(bgm38)」来调用相应的表情图片。

因为文字本身没有含义，主要是依靠这段文字能与表情产生关系，所以这里将「233」「bgm38」称作「假借文字表情」。

「假借文字表情」由常见的字符组成，所以受到 GWLM 3-4 控制，演示如下：

| 启用的模块       | 效果                |
| ---------------- | ------------------- |
| GWLM 3           | 这个视频真有趣233。 |
| GWLM 3, GWLM 5   | 这个视频真有趣233   |
| GWLM 3-4, GWLM 5 | 这个视频真有趣 233  |

### 颜文字

颜文字 (Kaomoji) 由许多半角或全角符号组成，所以应该将会分别检查首尾的全角／半角情况，
这受 GWLM 3-4 控制，演示如下：

| 启用的模块 | 效果                       |
| ---------- | -------------------------- |
| GWLM 3     | 颜文字♪（´▽｀）非常精妙。  |
| GWLM 3-4   | 颜文字 ♪（´▽｀）非常精妙。 |

### Emoji

Emoji 被视作半角字符，并且连续使用时，Emoji 之间也需要有空格：

> 🍣 🍤 🍙 🍘 这些料理真好吃！
>
> _(GWLM 3-4, GWLM 5)_

## GWLM 15834 简体中文标点符号用法模块化

```yaml
标题: 简体中文标点符号用法模块化
创建时间: 2023年8月28日
```

《GB/T 15834-2011 标点符号用法标准》这个标准存在一些模糊的情况，所以这里尝试使用更精确的模块替代部分标准。

主要目的是重写出一个符合 CC-BY 4.0 协议，并兼容《GB/T 15834-2011 标点符号用法标准》的模块。
这样在未来就不需要以不够开放的资料，作为 GWLM 的基础，但是任重道远，还有大量待重写的部分。

### GWLM 15834-1 范围

本模块规定了简体中文标点符号的用法，适用于简体中文书写系统。

### GWLM 15834-2 简体中文标点符号词汇表

#### GWLM 15834-2-1 标点符号 (punctuation)

标点符号是辅助断句、标示的符号，所以移除标点符号后，仍然可以获悉文字大意，
但增加了阅读的复杂度，还有歧义。

用来断句的符号是「点号」，标示的符号是「标号」。

#### GWLM 15834-2-2 句子

被句末点号包围的，表达相对完整意义的语言单位。

#### GWLM 15834-2-3 复句（复合句）

复句，又称「复合句」。由两个或以上意义上有密切关系含的分句组成的语言单位。

#### GWLM 15834-2-4 分句（单句）

分句，又称「单句」。被句内点号包围，含有相对完整意义的语言单位。

#### GWLM 15834-2-5 语段

对各种语言单位（词、句子、复句等）的统称。

#### GWLM 15834-2-6 点号

表示各种强度的停顿符号，分为「句末点号」和「句内点号」。

##### GWLM 15834-2-6-1 句末点号

表示一句话的结束。包括
[句号](#gwlm-15834-4-1-句号)、
[问号](#gwlm-15834-4-2-问号)、
[叹号](#gwlm-15834-4-3-叹号)。

##### GWLM 15834-2-6-2 句内点号

表示句内各种不同性质的停顿。包括
[逗号](#gwlm-15834-4-4-逗号)、
[顿号](#gwlm-15834-4-5-顿号)、
[分号](#gwlm-15834-4-6-分号)、
[冒号](#gwlm-15834-4-7-冒号)。

#### GWLM 15834-2-7 标号

起到标示作用的符号，使用标号（标识符号）能够快速识别某段文字的作用。

包括
引号、
括号、
破折号、
省略号、
着重号、
[连接号](#gwlm-15834-4-13-连接号)、
[间隔号](#gwlm-15834-4-14-间隔号)、
书名号、
专名号、
[分隔号](#gwlm-15834-4-17-分隔号)。

### GWLM 15834-3 未定义

《GB/T 15834-2011 标点符号用法标准》的 2 与 3 小节被合并到了 GWLM 15834-2，所以 GWLM 15834-3 暂时空缺。

### GWLM 15834-4 标点符号的定义、形式和基本用法

#### GWLM 15834-4-1 句号

GWLM 15834-4-1 是替代《GB/T 15834-2011 标点符号用法标准》4.1 小节的模块，
描述了句号的定义、形式和基本用法。

+   GWLM 15834-4-1-1 定义

    句末点号的一种，表示以陈述语气结束一句话的停顿与标示。

+   GWLM 15834-4-1-2 形式

    句号的形式是「。」。

    | 符号  | Unicode  | 名称                                                               |
    | :---: | :------: | ------------------------------------------------------------------ |
    |  。   | `U+3002` | [Ideographic Full Stop](https://www.compart.com/en/unicode/U+3002) |

+   GWLM 15834-4-1-3 基本用法

    +   GWLM 15834-4-1-3-1 用于句子末尾，表示陈述语气。

        > （海鸥甲：待会去码头整点薯条？）
        >
        > 海鸥乙：恩。
        >
        > 海鸥丙：我也要去，别忘记我。

    +   GWLM 15834-4-1-3-2 祈使和惊叹句的语气不强烈，也可以使用句号。

        > 少女祈祷中。

        > 更新后的版本实在是糟糕。

#### GWLM 15834-4-2 问号

GWLM 15834-4-2 是替代《GB/T 15834-2011 标点符号用法标准》4.2 小节的模块，
描述了问号的定义、形式和基本用法。

+   GWLM 15834-4-2-1 定义

    句末点号的一种，表示以疑问语气结束一句话的停顿与标示。

+   GWLM 15834-4-2-2 形式

    问号的形式是「？」。

    | 符号  | Unicode  | 名称                                                                 |
    | :---: | :------: | -------------------------------------------------------------------- |
    |  ？   | `U+FF1F` | [Fullwidth Question Mark](https://www.compart.com/en/unicode/U+FF1F) |

+   GWLM 15834-4-2-3 基本用法

    +   GWLM 15834-4-2-3-1 用于句子末尾，表示疑问语气（包括反问、设问等疑问类型）。

        > 为什么无法运行这个软件？

        > 啊？

    +   GWLM 15834-4-2-3-2 在选择问句的句中，可以使用问号替代逗号。

        > 什么键盘轴体更好：机械轴，光轴，还是电磁轴？

        > 什么键盘轴体更好：机械轴？光轴？还是电磁轴？

    +   GWLM 15834-4-2-3-3 异常强烈的疑问时，可以叠问号，通常是依次递增，最多使用三个问号。

        > 我儿子每一科的成绩都不过那个平均分呐，他现在初二，你叫我儿子怎么办啊？
        > 他现在还不到高中啊好不好？？
        > 你们这是什么群啊？？？

    +   GWLM 15834-4-2-3-4 问号也有标号的用法，即用于句内，表示存疑或不详。

        > 老子（前 571？―前 471？），可能名为李耳，世人尊称为「老子」。

        > 黄石公（？―？），秦朝末年人物，曾传授张良兵法。

        > 这把剑（刀？）不好用。

#### GWLM 15834-4-3 叹号

+   GWLM 15834-4-3-1 定义

    句末点号的一种，表示以感叹语气结束一句话的停顿与标示。

+   GWLM 15834-4-3-2 形式

    叹号的形式是「！」。

    | 符号  | Unicode  | 名称                                                                    |
    | :---: | :------: | ----------------------------------------------------------------------- |
    |  ！   | `U+FF01` | [Fullwidth Exclamation Mark](https://www.compart.com/en/unicode/U+FF01) |

+   GWLM 15834-4-3-3 基本用法

    +   GWLM 15834-4-3-3-1 用于句子末尾，表示感叹语气（包括祈使、反问等类型）。

        > 跳票这么久，终于发售了！

        > 电次！不要开门！

        > 哟！你们也来打雪仗了啊！

    +   GWLM 15834-4-3-3-2 用于拟声词后，表示声音短促或突然。

        > 咚！咚！咚！特勤干员 Fuze 正在释放集束炸弹。

        > 轰！人质被集束炸弹杀死，游戏结束。

    +   GWLM 15834-4-3-3-3 声音大或者加大，以及异常强烈的情感，可以叠用叹号，最多使用三个叹号。

        > 冻住！不许走！！

    +   GWLM 15834-4-3-3-4 用于同时包含疑问、感叹两种语气且都比较强烈时，同时使用问号以及感叹号。

        > 你敢直面恐惧吗？！

#### GWLM 15834-4-4 逗号

GWLM 15834-4-4 是替代《GB/T 15834-2011 标点符号用法标准》4.4 小节的模块，
描述了逗号的定义、形式和基本用法。

+   GWLM 15834-4-4-1 定义

    句内点号的一种，表示句子尚未结束的常规停顿与标示。

+   GWLM 15834-4-4-2 形式

    逗号的形式是「，」。

    | 符号  | Unicode  | 名称                                                         |
    | :---: | :------: | ------------------------------------------------------------ |
    |  ，   | `U+FF0C` | [Fullwidth Comma](https://www.compart.com/en/unicode/U+FF0C) |

+   GWLM 15834-4-4-3 基本用法

    +   GWLM 15834-4-4-3-1 为复句分隔，通常使用逗号，有时用分号（见 4.6.3.1）。

        > 能观测就能干涉，能干涉就能控制。

        > 我前脚刚走，后脚就跟上了。

    +   GWLM 15834-4-4-3-2 用于间隔各种语法位置：

        > 收集各种奖杯，也没什么用。

        > 准备好大容量硬盘，还有高速的网络，以及 ArchiveTeam Warrior 进行众包存档吧。

    +   GWLM 15834-4-4-3-3 用于口语化文字的停顿处：

        > 团长，车已经准备好了。

        > 第一，绝对不会意气用事；第二，绝对不漏判任何一件坏事；第三，绝对裁判的公正漂亮。

#### GWLM 15834-4-5 顿号

GWLM 15834-4-5 是替代《GB/T 15834-2011 标点符号用法标准》4.5 小节的模块，
描述了顿号的定义、形式和基本用法。

+   GWLM 15834-4-5-1 定义

    句内点号的一种，表示语段中并列词语之间或某些序次语之后的停顿与标示。

+   GWLM 15834-4-5-2 形式

    顿号的形式是「、」。

    | 符号  | Unicode  | 名称                                                           |
    | :---: | :------: | -------------------------------------------------------------- |
    |  、   | `U+3001` | [Ideographic Comma](https://www.compart.com/en/unicode/U+3001) |

+   GWLM 15834-4-5-3 基本用法

    +   GWLM 15834-4-5-3-1 作为弱于逗号的停顿，示例：

        > 我准备讲两个问题：一、CSGO 经济系统是什么？二、怎样学好 CSGO 经济系统？

        > 甲、意识；乙、枪法；丙、道具；丁、运气。

        > 寻血猎犬总是不断、不断地重伤倒地。

    +   GWLM 15834-4-5-3-2 作为「连词」的替代符号（「连词」即连接两个词语的词语，
        比如「和」「跟」「与」及「或者」）。

        > 《Apex 英雄》是一款专注于角色、小队制的大逃杀射击游戏。

        > GDP、人均 GDP 和常住人口这项指标，可以划分出一、二、三线城市。[^ltcic]

        [^ltcic]:  xunyun, [_Lower-tier_Cities_in_China/data/低线城市划分.md_](https://github.com/xunyun/Lower-tier_Cities_in_China/blob/master/data/低线城市划分.md), GitHub, 2018-11-20. (参照 2023-08-27).

        如果本来就没有必要使用「连词」，那么也无需使用顿号，比如：

        > 我喜欢《Apex 英雄》《机器人总动员》《我兔斯基你》「东方 Project」这些作品。

        书名号或者引号已将这些内容间隔开了，所以不再需要使用「连词」或者顿号，但是如果这些词语的首尾符号不同，
        那么就需要使用顿号间隔，比如：

        > 我喜欢《Apex 英雄》（游戏）、《机器人总动员》（电影）、《我兔斯基你》（绘本）、「东方 Project」
        （文化）这些作品。

        因为括号属于夹注，能够推理出括号内容是对前文的注释，但是混排在一起就会缺少间隔，
        增加了理解句子的难度，下面是反例：

        > 我喜欢《Apex 英雄》（游戏）《机器人总动员》（电影）《我兔斯基你》（绘本）「东方 Project」（文化）
        这些作品。

#### GWLM 15834-4-6 分号

GWLM 15834-4-6 是替代《GB/T 15834-2011 标点符号用法标准》4.6 小节的模块，
描述了分号的定义、形式和基本用法。

+   GWLM 15834-4-6-1 定义

    句内点号的一种，作为分割并列关系复句的停顿与标示，重复句式的间隔。

+   GWLM 15834-4-6-2 形式

    分号的形式是「；」。

    | 符号  | Unicode  | 名称                                                             |
    | :---: | :------: | ---------------------------------------------------------------- |
    |  ；   | `U+FF1B` | [Fullwidth Semicolon](https://www.compart.com/en/unicode/U+FF1B) |

+   GWLM 15834-4-6-3 基本用法

    +   GWLM 15834-4-6-3-1 作为分割并列关系复句的停顿，比起逗号的间隔感更强。

        > 正因为生命有限，所以才显得更重要；正因为生命有限，所以才更应该努力不懈。

        > 大道废，有仁义；智慧出，有大伪；六亲不和，有孝慈；国家昏乱，有忠臣。

    +   GWLM 15834-4-6-3-2 主要是选择、转折等关系之间的停顿。

        > 在人类生活的壮丽行列中，我觉得真正可贵的，不是政治上的国家，而是有创造性的、
        > 有感情的个人，是人格；只有个人才能创造出高尚的和卓越的东西，而群众本身在思想上总是迟钝的，
        > 在感觉上也是迟钝的。

    +   GWLM 15834-4-6-3-3 用于分项列举的各项之间。

        > 第一，绝对不会意气用事；第二，绝对不漏判任何一件坏事；第三，绝对裁判的公正漂亮。

#### GWLM 15834-4-7 冒号

GWLM 15834-4-6 是替代《GB/T 15834-2011 标点符号用法标准》4.7 小节的模块，
描述了冒号的定义、形式和基本用法。

+   GWLM 15834-4-7-1 定义

    句内点号的一种，提起下文或总结上文的停顿与标示。

+   GWLM 15834-4-7-2 形式

    冒号的形式是「：」。

    | 符号  | Unicode  | 名称                                                         |
    | :---: | :------: | ------------------------------------------------------------ |
    |  ：   | `U+FF1A` | [Fullwidth Colon](https://www.compart.com/en/unicode/U+FF1A) |

+   GWLM 15834-4-7-3 基本用法

    +   GWLM 15834-4-7-3-1 用于解释符号前的提示词，或者表示有人说话，用来提示下文。

        > 和平捍卫者的配件：霰弹枪栓、瞄具、枪托和干扰器。

        > 系色望：「我是视而不见的专家哦，我就是靠对所有事情视而不见活下来的！」

    +   GWLM 15834-4-7-3-2 用于总结上文。

        > 张华考上了北京大学；李萍进了中等技术学校；我在百货公司当售货员：我们都有光明的前途。

    +   GWLM 15834-4-7-3-3 用在需要说明的词语之后，表示注释和说明。

        > 机箱：黑暗骑士 Z1；硬盘：希捷 500 GB 黑盘；显示器：AOC C27G2ZE/11。

    +   GWLM 15834-4-7-3-4 用于信件（包括短信和电子邮件）、讲话稿中称谓语或称呼语之后。

        > 尊敬的客户：您缴费已成功……

    +   GWLM 15834-4-7-3-5 冒号不能在一段内重复使用，需要让文字分段。

        > 这赛季的枪械排名：
        >
        > T0：复仇女神、复仇男神。
        >
        > T1：和平捍卫者、R99。
        >
        > T2：三重狙击枪、R301。
        >
        > T3：莫桑比克、P2020。

#### GWLM 15834-4-13 连接号

GWLM 15834-4-13 是替代《GB/T 15834-2011 标点符号用法标准》4.13 小节的模块，
描述了连接号的定义、形式和基本用法。

+   GWLM 15834-4-13-1 定义

    标号的一种，标示某些相关联成分之间的连接。

+   GWLM 15834-4-13-2 形式

    连接号的形式有短横线「-」、一字线「―」和浪纹线「～」三种。

    | 符号  | Unicode  | 名称                                                         |
    | :---: | :------: | ------------------------------------------------------------ |
    |   -   | `U+002D` | [Hyphen-Minus](https://www.compart.com/en/unicode/U+002D)    |
    |   ―   | `U+2015` | [Horizontal Bar](https://www.compart.com/en/unicode/U+2015)  |
    |  ～   | `U+FF5E` | [Fullwidth Tilde](https://www.compart.com/en/unicode/U+FF5E) |

    其他相似符号：

    | 符号  | Unicode  | 名称                                                                |
    | :---: | :------: | ------------------------------------------------------------------- |
    |   ~   | `U+007E` | [Tilde](https://www.compart.com/en/unicode/U+007E)                  |
    |   ‐   | `U+2010` | [Hyphen](https://www.compart.com/en/unicode/U+2010)                 |
    |   ‑   | `U+2011` | [Non-Breaking Hyphen](https://www.compart.com/en/unicode/U+2011)    |
    |   −   | `U+2212` | [Minus Sign](https://www.compart.com/en/unicode/U+2212)             |
    |   –   | `U+2013` | [En Dash](https://www.compart.com/en/unicode/U+2013)                |
    |   —   | `U+2014` | [Em Dash](https://www.compart.com/en/unicode/U+2014)                |
    |  －   | `U+FF0D` | [Fullwidth Hyphen-Minus](https://www.compart.com/en/unicode/U+FF0D) |

+   GWLM 15834-4-13-3 基本用法

    +   GWLM 15834-4-13-3-1 存在连接关系，比如：

        +   复合名词：「印度-欧亚板块」「吐鲁番―哈密盆地」。

        +   双名人名：「让-吕克·皮卡德」(Jean-Luc Picard)。

        +   复姓人名：「康斯坦策·阿马莉·冯·布劳恩施班克―阿尔布雷希茨贝格」(Constanze Amalie von Braunschbank-Albrechtsberger)。

    +   GWLM 15834-4-13-3-2 存在序列关系，比如：

        +   元素、化合物：「碳-14」「碳-12」「3-戊酮」。

        +   对附件标识序号：「图-12」「表-2」。

        +   电话号码：「+1 (917) 285-7362」。[^bpn]

        +   时间：「2023-08-28」。

        [^bpn]: 此电话号码来自《疑犯追踪》([Person of Interest](https://personofinterest.fandom.com/wiki/(917)_285-7362))。

    +   GWLM 15834-4-13-3-3 标示起止或范围，比如：

        +   经济计划：「中国-中亚-西亚经济走廊」。

        +   铁路：「巴库―第比利斯―卡尔斯铁路」。

        +   时间：「2023 年 8 月 28 日―29 日」。

        +   重量：「40～60 千克」「四十～六十千克」。

#### GWLM 15834-4-14 间隔号

GWLM 15834-4-14 是替代《GB/T 15834-2011 标点符号用法标准》4.14 小节的模块，
描述了间隔号的定义、形式和基本用法。

+   GWLM 15834-4-14-1 定义

    标号的一种，标示某些相关联成分之间的分界。

+   GWLM 15834-4-14-2 形式

    间隔号的形式是「·」。

    | 符号  | Unicode  | 名称                                                    |
    | :---: | :------: | ------------------------------------------------------- |
    |   ·   | `U+00B7` | [Middle Dot](https://www.compart.com/en/unicode/U+00B7) |

    其他相似符号：

    | 符号  | Unicode  | 名称                                                             |
    | :---: | :------: | ---------------------------------------------------------------- |
    |   ‧   | `U+2027` | [Hyphenation Point](https://www.compart.com/en/unicode/U+2027)   |
    |  ・   | `U+30FB` | [Katakana Middle Dot](https://www.compart.com/en/unicode/U+30FB) |

+   GWLM 15834-4-14-3 基本用法

    +   GWLM 15834-4-14-3-1 标示被翻译为汉字的人名。

        > 阿姆罗·雷 (Amuro Ray)

    +   GWLM 15834-4-14-3-2 标示作品名与篇（章、卷）名之间的分界。

        > 《汉志·蜀王本记》

    +   GWLM 15834-4-14-3-3 标示词牌、曲牌、诗体名等和题名之间的分界。

        > 《天净沙·即事》

    +   GWLM 15834-4-14-3-4 用在构成标题或栏目名称的并列词语之间。

        > 《游戏·人》

    +   GWLM 15834-4-14-3-5 以月、日为标志的事件或节日，在数字间使用。如果是汉字数字，
        仅在一、十一和十二月后用间隔号（防止歧义）。

        > 五一二大地震

        > 十二·十世界人权日

        > 12·25 圣诞节

#### GWLM 15834-4-17 分隔号

GWLM 15834-4-17 是替代《GB/T 15834-2011 标点符号用法标准》4.17 小节的模块，
描述了分隔号的定义、形式和基本用法。

+   GWLM 15834-4-17-1 定义

    标号的一种，标示诗行、节拍及某些相关文字的分隔。

+   GWLM 15834-4-17-2 形式

    分隔号的形式是「/」「／」。

    | 符号  | Unicode  | 名称                                                 |
    | :---: | :------: | ---------------------------------------------------- |
    |   /   | `U+002F` | [Solidus](https://www.compart.com/en/unicode/U+002F) |

    +   其他相似符号：

    | 符号  | Unicode  | 名称                                                           |
    | :---: | :------: | -------------------------------------------------------------- |
    |  ／   | `U+FF0F` | [Fullwidth Solidus](https://www.compart.com/en/unicode/U+FF0F) |

    备注：GWLM 15834-4-17 本身并未指定半角或全角的分隔号（斜线、斜杠）

+   GWLM 15834-4-17-3 基本用法

    +   GWLM 15834-4-17-3-1 诗歌接排时分隔诗行。

        > 洛阳城东路/桃李生路旁/花花自相对/叶叶自相当。

    +   GWLM 15834-4-17-3-2 标示诗文中的音节节拍。

        > 床前/看月光，疑是/地上霜。

    +   GWLM 15834-4-17-3-3 分隔供选择或可转换的两项，标示「或」。

        > 这部手机需要指纹/密码来解锁。

    +   GWLM 15834-4-17-3-4 分隔组成一对的两项，标示「和」。

        > 这是 12/13 赛季最强的武器。

        > 乒乓球混合双打的组合有水谷隼/伊藤美誠、埃马纽埃尔·勒贝松/袁嘉楠。

    +   GWLM 15834-4-17-3-5 分隔层级或类别。

        > 行政区划分：省/县/乡/村。

        > 为 Android 手机开启 Android 调试（ADB 功能），需要进入设置/关于手机，
        > 连续点击版本号七次，回到设置首页后进入设置/系统/开发者选项/调试，就能找到 Android 调试。
