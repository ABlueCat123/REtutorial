## Project 2: 插件内核汉化

!> **注意** 本教程的**大工程**(Project, PJ)是教程的重要实践部分。原则上需要读者完成一定量的PJ内容才能视为“学有所得”。因此如果有机会还请实践完成。

### 背景

——“来帮忙搬运汉化个插件，有偿。”

——“好嘞，我翻译一下语言文件。”

——“诶，这里为什么没汉化呢？”

——“啊？语言文件里没有这句话啊。”

——“你工资没了！”

——“……我燃烧你的梦。”

（以上纯属瞎扯）

### PJ描述

众所周知，插件/mod的国际化(internationalization, i18n)是其能获得世界范围内源源不断的生命力的重要原因之一。在现代社会，“酒香也怕巷子深”。如果这条“巷子”还有语言的隔阂那就更糟糕了。

因此，在社区涌现出了一大批志愿者(俗称“搬运工”)，他们把这些插件/mod汉化，传播到中文社区内，极大地改善了玩家的游戏体验。

也正因为插件国际化的需求，有些作者会提供语言文件，有些甚至给出了语言选项，这样对搬运工来说就相对来说很容易。然而，并不是所有的过程都如此皆大欢喜 —— 有些作者会把自己的一部分文本直接写在代码里面，而非提供一个语言文件，然后插件引用语言文件的内容(俗称“写死”在代码里)。这样，一般的汉化过程就不奏效了。

在学习过字节码的操作方法后，我们可以很容易地做到这点 —— 用逆向工程的方法汉化插件！

### 注意事项
如果你是汉化插件的新手，笔者有必要说明一下搬运插件的基本流程：

首先，寻求**授权**。一般来说，搬运行为对于部分作者来说不可容忍，因此，在搬运之前请与作者联系，只有获得了搬运许可后才可继续接下来的事情。

接下来汉化工作的话，最好的莫过于你开一个本地服务器运行一下插件，看看在游戏过程中出现了什么文本，并汉化它。

如果你不想这样干，那么可以按照以下原则进行：
* 任何情况下都应该以**保守**的态度对待汉化。
* 配置文件(config.yml)内的注释文本**需要**汉化，插件属性文件(plugin.yml)**不应该**汉化
* sendMessage语句内的文本**原则上应当**汉化。
* 帮助类(如果有)里面的文本**原则上应当**汉化。
* 日志类语句的文本原则上**可以**汉化。
* 其他字符串**不应该**汉化。

**编码问题**，在插件内核汉化时，由于可能出现各种各样神奇的编码问题，如果确实遇到了，这里有一个通解：使用**Unicode**编码。

最后，应该把汉化后的插件再运行一次，确保它没有错误了之后进行发布。

### 实例
如果你确实没有找到合适的插件进行汉化，笔者找到了一些插件，你可以尝试汉化一下！最重要的是，这些插件在本文章撰写时**还没有**在mcbbs上出现过/发布帖早已过时！~~你甚至可以进行一个勋章的拿。~~

!> **注意** 以下插件仅供参考！笔者仅为教学目的找到以下插件，对其内容和功能不负责任。
* ChatItem https://www.spigotmc.org/resources/chatitem-display-items-in-chat.19064/
* THE MULTIWORLD MONEY  https://www.spigotmc.org/resources/the-multiworld-money.56671/
* Executable Items https://www.spigotmc.org/resources/custom-items-free-executable-items.77578/