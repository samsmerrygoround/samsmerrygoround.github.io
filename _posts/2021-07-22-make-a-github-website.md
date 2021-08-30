---
title: 编程小白制作个人网站（超简单！）
date: 2021-07-22T15:00:00-04:00
last_modified_at: 2021-07-22T15:00:00-04:00
tags:
  - 食盐两分
toc: true
toc_sticky: false
---

大家好！今天我想和大家分享一下我是怎么用 GitHub Pages 建立我的个人网站的。

<!--more-->

首先，直接上我的网站成品：[`https://samxshang.github.io/`](https://samxshang.github.io/)。

其次，我想做两个声明：

1.  我的网站主要用来展示我的学术生涯和学术成果。不求原创，不太追求美观，只求能用。所以不一定适合设计类的个人展示。
2.  我的网站知识极其有限，也基本上完全不懂 `html` 和 `css` 。我的分享是偏 practical 的，也就是我只能分享我做了什么，但是没有办法解释理论。如果我的分享中哪里有错误，非常欢迎专业人士进行补充和纠正哈。（我也希望通过这个声明给大家一点信心，就算我理论一窍不通我还是把网站做出来了，所以做网站真的没有那么难的！）

再次，作为一个前 Wordpress 使用者，我想谈一下我选择从 Wordpress（以下简称WP）转移到 GitHub Pages（以下简称GP）的两点原因：

1.  GP 本质上来说是把 Markdown 文件直接变成网页，且 GitHub 具有强大的 version control 功能。我直接可以在后台看到每一个 md 文件，非常便于备份和管理。可能也是我 WP 没太用明白，但我并没有在后台找到每个 WP page 或 post 的单独文件，这样如果我想转移或备份我的整个网站，相对来说就更困难一点。
2.  GP 开源免费，不需要花钱买空间和域名。WP 也有免费版本，但是感觉相对来说限制还是很多。

---

接下来进入正题：

# 背景知识

根据官网上的信息（[GitHub Pages](https://www.markdownguide.org/tools/github-pages/)，[Jekyll](https://jekyllrb.com/docs/ruby-101/)），GitHub 网站是由 `Jekyll` 来生成的，`Jekyll` 是用 `Ruby` 写的。使用 `Ruby` 可以写各种 `Gem`，比如 `Jekyll` 就是一个 `Gem`，`Jekyll` 的很多 `plugin` 也是 `Gem`。

如果你和我一样建站知识有限，你的反应可能和我一样：`Jekyll` 是个啥，`Ruby` 是个啥，`plugin` 是个啥，`Gem` 又是个啥。好消息：新手玩家建网站并不需要明白这些术语！因为有前人无私奉献做好的免费模板，我们只需要找到一个自己喜欢的模板，然后直接套用就可以。**不**需要在电脑上安装 `Jekyll`，也**不**需要在电脑上安装 `Ruby`！

# 轻松建站

以下是我使用 GitHub Pages 制作网站的步骤：

## 准备

1.  你需要有一个 [GitHub](https://github.com/) 账号。用户名会成为你网站域名的一部分（最后网站的域名是 `username.github.io`），所以需要谨慎选择用户名。
2.  下载安装 [Git](https://git-scm.com/downloads)，下载安装 [GitHub Desktop](https://desktop.github.com/)。
3.  找到一个你喜欢的免费 `Jekyll` 主题：[Jekyll Themes](https://jekyllthemes.io/)。我选中的是[”Minimal Mistakes“](https://jekyllthemes.io/theme/minimal-mistakes)。点进你选择的主题，点击Get it on GitHub，把跳转的网站放在那里备着。
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-minimal-mistake.jpeg" alt="minimal-mistake" width="400"/>
    
## 使用主题

有两个方法来使用现成的主题。

### 方法一

1.  在GitHub上建立一个新 Repository，Repository name 如下：`username.github.io`。  
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-git-repo.png" alt="git-repo" width="690"/>
<br>
（截图来自[官网](https://pages.github.com/)）
2.  在 GitHub Desktop 里选择 clone the repository：
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-git-desktop.png" alt="clone-repo" width="400"/>
<br>
3.  在你选中主题的 repository 网页上选择 Download ZIP：
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-zip.png" alt="git-repo" width="690"/>
<br>
4.  下载后在本地解压，然后把整个文件夹里的内容复制到你自己本地的 repository folder 里面。
5.  在 GitHub Desktop 里选中所有文件，先 Commit，然后 Push：  
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-commit.jpeg" alt="git-commit" width="690"/>
<br>
（截图来自[官网](https://pages.github.com/)）
6.  天哪！你的网站上线了！查看你的网址：**https:// _username_ .github.io**  
    （当然现在还是别人网站的状态，后面我会提到如何更改网站的设置，把网站变成自己的信息。）

### 方法二

1.  Fork 主题的 Repository：  
<br>
<img src="https://raw.githubusercontent.com/samsmerrygoround/samsmerrygoround.github.io/main/assets/images/web-fork.png" alt="fork-repo" width="690"/>
<br>
2.  点击 “Settings”，把 Repository name 改成：`username.github.io`
3.  天哪！你的网站上线了！查看你的网址：**https:// _username_ .github.io**
4.  当然现在还是别人网站的状态，为了更改网站的文件，你需要先把网站文件同步到本地。在 GitHub Desktop 里选择 clone the repository，然后 Fetch Origin。

## 更改网站文件

通常每一个主题都会自带一个 `README.md`，这个文件非常重要，建议一定要仔细读。虽然每个主题的具体文件不同，但通常最重要的（也就是你需要修改的）是以下三类文件：

1.  `_config.yml`：在 root 文件夹里，包括网站名，网站作者信息等等
2.  组成网站首页和结构的一系列网页（不知道怎么说，就是 Menu 下面的那些网页）：大部分现成主题选择用 markdown（`xxxx.md`）来写这些网页；也有一些主题是用 html （`xxxx.html`）来写。具体信息要参考主题自带的 `README.md`。
3.  posts：这些文件在 `_post` 文件夹里，通常都是用 markdown（`xxxx.md`）来写的。比如你想建一个blog，那么你的每一篇文章就由一个单独的 markdown 文件来写成。

改完网站的文件，在GitHub Desktop 里选中更改的文件，先 Commit，然后 Push。等一小会儿你的网站就会自动更新了。

## 进阶

如果你会写 `html`，`css`，甚至是 `Ruby`，那么你的网站会有更大的改造空间。如果想要进阶高级玩家，想在电脑上安装 `Jekyll` 和 `Ruby` 然后自己通过写码建站，可以参考这篇英文教程：[Jekyll教程：如何建立静态网站](https://www.taniarascia.com/make-a-static-website-with-jekyll/)。

---

以上就是全部分享了，是不是很简单呢？祝大家建站开心，欢迎讨论！

*注：本网站也是由相似的方法制作的。这次我用的模板是[TeXt-theme](https://github.com/kitian616/jekyll-TeXt-theme)。作者是中国人，网站也支持中文模板，非常方便美观。*

{% comment %}

Post: [编程小白制作个人网站（超简单！）](https://womenoverseas.com/t/topic/17528)

棍仔：Bootswatch [https://bootswatch.com](https://bootswatch.com/)  上面有非常多的template可以直接copy code对自己的网站进行装修。

八比的比：附上一个讲解git的教程：[目錄 | 猴子都能懂的GIT入门 | 贝格乐（Backlog）](https://backlog.com/git-tutorial/cn/contents/) 我在修改github page过程中发现用得上。

{% endcomment %}
