---
title: Pre-PHD BINGO - Day 3-5 文献阅读，文献管理，本地文档与云端的自动同步和备份
date: 2021-06-11T12:00:02-04:00
last_modified_at: 2021-06-11T12:00:02-04:00
tags:
  - 读博预备役
toc: true
toc_sticky: false
---

文献阅读、文献管理和云端备份对我来说是相互联系的，所以放在一起来总结一下。

<!--more-->

# 我使用的各种工具/软件以及工具点评

-   文献阅读：**Remarkable 2**
    -   我选择用Remarkable 2读文献的原因主要有两点：1）把所有论文都打印出来难以管理、不方便随身携带；2）在纸上阅读文献的过程中在文献上圈圈点点的笔记没有办法直接存到云上，想保留笔记的话只能进行二次整理，有点麻烦。
    -   Remarkable 2的使用体验：E-ink 平板，不伤眼；写字基本可以达到和纸质一样的效果，无延迟，没有玻璃感；最近软件更新以后Remarkable也可以用双指放大局部字体了，读文献方便了很多。虽然Remarkable本身价格比较高，但是长久来看我觉得是值得的。
-   文献笔记：**Obsidian**
    -   支持markdown syntax，每个笔记卡片会在本地存为一个markdown文件。
    -   软件理念基于Zettelkasten卡片盒笔记系统；非常适合笔记间互链，文献间建立联系。
    -   界面优美，写作不容易分心。
    -   Obsidian是一个免费软件。
-   文献管理：**Paperpile**
    -   我使用Zotero已经快三年了，最近才在朋友的推荐下发现了Paperpile，简直惊为天人。Paperpile最大的优势是1）电脑网页端、ios和安卓端之间可以同步；2）文献自动储存在Google drive，因此在手机端或平板上也可以直接通过Paperpile打开文献pdf阅读；3）可以在软件后台直接设置所在学校的proxy connections，所以不需要每次存文献pdf的时候都通过学校图书馆或认证身份。
    -   Paperpile是有订阅费的，但是可以先免费试用。试用结束后也才2.99刀一个月，again，我觉得这个钱对我来说花得值得。
-   文献储存：**Google drive**

# 关联以上工具/软件

以下是我的工具使用场景：

-   第一步，我在网页上一键把文献信息和pdf储存到文献管理软件Paperpile上。Paperpile会自动帮我把文献改名为`Author_(Year)_Title`的形式，然后把pdf存到我的Google Drive上。
-   第二步，由于我设置了Google Drive和电脑本地同步，我会在电脑的对应文件夹里看到这篇文献的pdf。
-   第三步，我打开Remarkable的电脑桌面端，把文献从本地发送到我的Remarkable上。
-   第四步，我在Remarkable上读文献，圈圈点点，写一些short comment和阅读中产生的问题和灵感。
-   第五步，我把阅读完的文献在Remarkable的桌面端以相同的文件名保存至我的本地文献文件夹。于是Google Drive和Paperpile也会自动更新文献的pdf。这样下次我再打开这个文献pdf时，上面就会保留我上次阅读时做的笔记。
-   第六步，我打开Obsidian，建立一个新的笔记卡片，标题为Author, Year（in-text citation的格式）。在这个笔记卡片上，我会总结这篇文献的内容和我的想法。我还会在这个笔记卡片上用”#"记录本篇文献的关键词。
-   第七步（bonus），虽然Obsidian本身还没有ios和安卓端，但是由于Obsidian生成的文件是markdown文件，相对来说多平台同步还是比较方便的。（再次）由于我设置了Google Drive和电脑本地同步，我在Obsidian上做的笔记首先会自动同步到我的Google Drive上。我自己会有在平板上查看笔记和写作的需求，所以最近我花30大洋买了**iA Writer app**，可以读入并同步存储在Google Drive的markdown file；价格稍贵但是可以满足我的一切需要，所以还是值得的。如果只需要在平板上查看笔记而不需要修改，也可以考虑把markdown files同步到免费的GitHub上。

# 如何使用Obsidian关联文献笔记

-   第一步，像我上面提到的，每篇文献我会建立一个单独的笔记卡片，标题为Author, Year（in-text citation的格式）。在这个笔记卡片上，我会总结这篇文献的内容和我的想法。我还会在这个笔记卡片上用”#"记录本篇文献的关键词。
<br> 
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/obsidian-1.png" alt="obsidian-1" width="690"/>
<br> 
-   第二步，比如我现在要进行文献综述。我会为这篇文献综述建立一个新的笔记卡片。在这篇文献综述里，我会用双方括号来引用某一篇具体的文献。这样我Ctrl+单击双括号以内的文献标题，就可以看到我在引用哪一篇文献、关于那篇文献我都记了哪些笔记。
<br> 
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/obsidian-2.png" alt="obsidian-2" width="690"/>
<br> 
-   第三步，当然是Obsidian最强大的graph view了。在这个界面就可以看到哪些文献彼此之间有关联，这些文献和哪些关键词有关联。
<br> 
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/obsidian-3.jpeg" alt="obsidian-3" width="690"/>
<br> 

# 其他本地与云端同步

上面提到的主要是我的文献和文献笔记的同步。其他非常需要同步备份的文件应该就是在写的paper和统计的code。Version control最强大的肯定是GitHub啦，所以paper和code我都会在GitHub上备份；其他相关的文件（比如data files和实验材料），per IRB regulation，不能随意上传公开平台的，我会在Google Drive上进行备份。

---
以上就是我的文献系统啦。希望对大家也有一点启发。欢迎大家分享自己的文献系统，相互学习~

{% comment %}


{% endcomment %}