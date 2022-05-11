# 前言

## 逆向工程介绍

逆向工程(Reverse Engineering)是一门“溯本求源”的技术。由于此概念在软件工程领域中的概念模糊不清<sup>[1]</sup>，按笔者的理解，可**粗略**理解为对于一个成品程序，通过其运行逻辑(乃至根据其运行逻辑而推测出来的类源代码)，来分析其设计理念、程序行为等开发者层面的内容的技术。

受到这门技术本身的“名声限制”，在互联网上相关的资料并不是很多，甚至到了2022年，mcbbs论坛上依然没有一个较成体系的逆向工程教程。技术是一把双刃剑，技术本身并没有绝对的对错。人将技术用于何种目的，该技术才有和这种目的相匹配的立场，逆向工程也是如此。出于补上空缺的目的，笔者编写了本教程。

## 本教程自述
本教程是一份**入门级别(Beginner-level)** 的逆向教程，这意味着阅读本教程的门槛较低：只要你有想学习逆向工程的想法都可以参考本教程学习。但如果拥有更高的追求，你可能还需要寻找其他教程进行进一步学习。**延伸阅读**里面给出了一些有用的链接。

本教程是一份**防御导向(Defense-oriented)型**的逆向教程。这意味着本教程旨在为读者提供基础逆向能力，以此更好地保护自己的信息系统安全，防止潜在的损失。**而非**通过逆向技术来攻击、入侵他人的计算机系统。

本教程是一份**实践(Practical)化**的逆向教程。在部分教程页面下会留下一定量的习题，在大章节下会留下大工程(Project)以供作为实践使用，习题、PJ本身仅供参考。在没有特殊说明的前提下，习题提供的所有插件均为**Minecraft 1.16.5的Spigot插件**。

## 教程改进工作
由于笔者水平有限，在逻辑严密性、文字措辞、涉及的知识点上都可能会存在一定缺陷。如果你对本教程的改进有建议或者意见，可用以下方式进行：
* 在mcbbs的帖子下直接回复;
* 在本教程的Github仓库提出issues或者提交Pull Request;

如果你有任何帮助改善教程习题的想法，也欢迎用以上方法提出。

## 额外声明

本教程内除另有声明外，其余文本部分均采用[CC BY-NC-SA 3.0协议](https://creativecommons.org/licenses/by-nc-sa/3.0/)授权，代码部分均**主动或被动放弃权利**。

本教程的任何一篇若存在参考资料，都会**独立地**在每一篇下方标出。

最后，引用一句话结束本前言：
> 一切伟大的行动和思想,都有一个微不足道的开始。 ——阿尔贝·加缪

本篇参考资料和致谢
1. Rarity's Plugin Dev Tutorial https://plgdev.xuogroup.top 感谢此教程在站点构建思路、前言的法律信息部分、部分思想等给我的启发。

延伸阅读：
1. 逆向工程 Wikipedia: https://zh.wikipedia.org/wiki/%E9%80%86%E5%90%91%E5%B7%A5%E7%A8%8B
2. CTF Wiki: https://ctf-wiki.org/
3. OI Wiki: https://oi-wiki.org/