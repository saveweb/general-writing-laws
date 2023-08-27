# 通用写作律法

```yaml
标题: 通用写作律法
创建时间: 2023年8月26日
版本: 0.0.3-beta
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

其他语言的完整支持，以及律法翻译尚未完成。

Full support for other languages, and legal translations are not yet complete.

目前暂未完成各项模块的情况，可能会有编号变动的情况。

## 简介

《律法》是为了将各种书写规范模块化，而诞生的规则，借鉴了一些 [BEP 0000][]（BitTorrent 增强建议索引）的设计。

[BEP 0000]: https://www.bittorrent.org/beps/bep_0.html

并且《律法》兼容多种语言，不仅仅是中文主体，而是要打造一套各种语言都通用的写作规则，
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

| 序号 | 标题             |
| ---- | ---------------- |
| 0    | 通用写作律法模块 |
| 1    | 语言空间         |
| 2    | 语言规范         |
| 3    | 兼容性           |

### 草案的 GWLM

| 序号 | 标题   |
| ---- | ------ |
| x    | 占位符 |

### 延期的 GWLM

| 序号 | 标题   |
| ---- | ------ |
| x    | 占位符 |

### 拒绝的 GWLM

| 序号 | 标题   |
| ---- | ------ |
| x    | 占位符 |

## GWLM 1 语言空间

```yaml
标题: 语言空间
创建时间: 2023年8月26日
```

「语言空间」是为文字的不同语言部分「划分空间」，并为各种部分指定「语言属地规范」。

### 划分空间

1.  标记「书名」「数字」以及「计量单位符号」等特殊的情况。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    ```

    备注：GitHub 的代码块并没有严格调用浏览器默认的等款字体，结果会造成排版错位，
    需要回到 GitHub 顶部，然后点击右上角的 Raw 按钮查看原始的等宽内容。

2.  标记外语的「片段环境」：

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

    这些外语的语言环境被称为「片段环境」。

3.  定义「语言环境」：

    通过标题和表意文字都是中文，能够给文章整体设下「简体中文」的「语言环境／环境变量」。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    语言环境 |      ·          ·          ·zh-Hans       ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

### 语言属地规范

+   「片段环境」没有占满一句话时，不应该使用「片段环境」的属地语法，比如英语的句首大写。
+   在并列外语词语时，使用「语言环境」的属地语法的顿号，比如：

    > 我们的客户有 Yahoo、Facebook, Inc.、Microsoft Corporation 和 Google。

    > Our clients include “百度”, “腾讯”, “金山” and “奇虎360”.

    备注：是否使用引号包围外语，请参考《GWLM 3 兼容性》的〈[各种语言的兼容性](#各种语言的兼容性)〉章节。

## GWLM 2 语言规范

```yaml
标题: 语言规范
创建时间: 2023年8月26日
```

语言规范由正字法、标点符号用法标准以及其他细节组成。

+   简体中文以《[GB/T 15834-2011 标点符号用法标准][]》作为标点符号用法标准。
+   繁体中文以《[重訂標點符號手冊][]》作为标点符号用法标准。

[GB/T 15834-2011 标点符号用法标准]: http://www.moe.gov.cn/ewebeditor/uploadfile/2015/01/13/20150113091548267.pdf
[重訂標點符號手冊]: https://language.moe.gov.tw/001/Upload/FILES/SITE_CONTENT/M1/HAU/haushou.htm

其他语言基本没有硬性规定的正字法、标点符号用法标准，所以暂不进行定义。

下面是可选的模块：

+   GWLM 2-0：尊重产品名词、专有名词的书写规范。
+   GWLM 2-1：各语言的写作方法在能在片段环境中完整生效，例外：
    +   GWLM 2-1-1：句首大写。
+   GWLM 2-2：片段环境会影响首尾有成对的符号，例外：
    +   GWLM 2-2-1：括号。
    +   GWLM 2-2-2：引号。
    +   GWLM 2-2-4：书名号（包括使用斜体表示书名）。
+   GWLM 2-3：单位符号与数字之间需要增加空格，例外：
    +   GWLM 2-3-1：度数，例如 ° ℃ °C。
    +   GWLM 2-3-2：百分号、千分号和万分号，例如 % ％ ‰ ‱。
+   GWLM 2-4：全角与半角语言文字之间需要增加空格，例外：
    +   GWLM 2-4-1：全角阿拉伯数字。
    +   GWLM 2-4-2：全角标点符号，例如 ， 。 ； 《 等。
    +   GWLM 2-4-4：全角特殊符号，例如 ％ ＊ ￥ ／ 等。
+   GWLM 2-5：CJK 标点符号替换的目录：

    +   GWLM 2-5-1：替换「简体中文的弯引号」为「全角直角引号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |   “   | U+201C  |   「   | U+300C  |
        |   ”   | U+201D  |   」   | U+300D  |
        |   ‘   | U+2018  |   『   | U+300E  |
        |   ’   | U+2019  |   』   | U+300F  |

    +   GWLM 2-5-2：替换「全角单层直角引号」为「半角单层直角引号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |  「   | U+300C  |   ｢    | U+FF62  |
        |  」   | U+300D  |   ｣    | U+FF63  |

    +   GWLM 2-5-4：替换「CJK 通用全角括号」为「英文半角括号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |  （   | U+FF08  |   (    | U+0028  |
        |  ）   | U+FF09  |   )    | U+0029  |

    +   GWLM 2-5-8：替换「中日通用全角逗号」为「英文的半角逗号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |  ，   | U+FF0C  |   ,    | U+002C  |

    +   GWLM 2-5-16：替换「CJK 通用全角句号」为「CJK 通用半角句号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |  。   | U+3002  |   ｡    | U+FF61  |

    +   GWLM 2-5-32：替换「CJK 通用全角句号」为「英文的半角句号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |  。   | U+3002  |   .    | U+002E  |

+   GWLM 2-6：英语标点符号替换的目录：

    +   GWLM 2-6-1：替换「英语的弯引号」为「全角直角引号」。

        | 原始  | Unicode | 修改后 | Unicode |
        | :---: | :-----: | :----: | :-----: |
        |   “   | U+201C  |   「   | U+300C  |
        |   ”   | U+201D  |   」   | U+300D  |
        |   ‘   | U+2018  |   『   | U+300E  |
        |   ’   | U+2019  |   』   | U+300F  |

备注：启用 GWLM 2-2-3 表示同时启用了 2, 2-2, 2-2-3；
启用 GWLM 2-4-7，就表示同时启用了 2, 2-4, 2-4-1, 2-4-2, 2-4-4，
原理是部分模块使用 1, 2, 4, 8…… 这样的序列递增，其实是二进制的位关系，所以可以相加。

GWLM 2-5-1 与 2-6-1 的结果看起来相同，当其作用的领域不同。2-5 作用于 CJK 的标点符号，
即中日韩统一表意文字的标点符号。而 2-6 作用于英语的标点符号。

### 示例

下面是启用一些模块后的效果：

| 启用的模块      | 效果                           |
| --------------- | ------------------------------ |
| 原始            | apple在传记steve jobs          |
| 无              | apple在传记《steve jobs》。    |
| 2-0             | apple在传记《Steve Jobs》。    |
| 2-1             | Apple在传记《steve jobs》。    |
| 2-2             | apple在传记_steve jobs_。      |
| 2-4             | apple 在传记《 steve jobs 》。 |
| 2-4-4           | apple 在传记《steve jobs》。   |
| 2-2, 2-4-4      | apple 在传记 _steve jobs_。    |
| 2-0, 2-2, 2-4-4 | apple 在传记 _Steve Jobs_。    |

---

如果更改模块的排序，也会导致优先级改变，比如：

| 启用的模块 | 效果               |
| ---------- | ------------------ |
| 原始       | 用户打开qq音乐     |
| 无         | 用户打开qq音乐。   |
| 2-0        | 用户打开QQ音乐。   |
| 2-4        | 用户打开 qq 音乐。 |
| 2-0, 2-4   | 用户打开 QQ音乐。  |
| 2-4, 2-0   | 用户打开 QQ 音乐。 |

---

启用 2-2 后，如果提到了不同语言的作品名，那么需要使用当地语言的书名表达方式：

> 我听说过« Beispiel in Frankreich » «Beispiel in der Schweiz» »Beispiel in Deutschland und Österreich«
> 《十万个为什么》『吾輩は猫である』_Steve Jobs_ 这些书名。

分别是法语、瑞士、德国／奥地利、中文、日语和英文的书名号表示方式。[^53627]

[^53627]: 德语世界, 《[【学生园地】德语的引号问题](https://www.sohu.com/a/www.sohu.com/a/289535110_653627)》, 搜狐新闻／搜狐号, 2019-01-16. (参照 2023-08-26).

## GWLM 3 兼容性

```yaml
标题: 兼容性
创建时间: 2023年8月26日
```

### 各种语言的兼容性

语言之间存在兼容性，比如 DNA、NBA 和 FPS 这些英文缩写，以及 Apple、Google 和 Microsoft 这些知名公司，
都已经成为了事实上的中文 [外来语][]，属于直接使用的外来词，就像是香港常用的张 Sir 来表示张先生一样，
没有必要使用引号标注。

[外来语]: https://zh.wikipedia.org/wiki/外来语

但是如果是中文、俄语或者日语，出现在英文环境，就需要使用引号包围了。

### 兼容其他规范

简介里有提到因为《律法》是模块化的，所以可以选配各种不同的规范，所以现有的排版规范也可以使用《律法》来实现。

《[中文文案排版指北][]》是相当知名的中文文案、排版方案，可以通过启用部分《律法》模块来兼容《指北》，
具体是 GWLM 2-0, 2-1, 2-2-3, 2-3-3, 2-4-3, 2-5-1。

[中文文案排版指北]: https://github.com/sparanoid/chinese-copywriting-guidelines
