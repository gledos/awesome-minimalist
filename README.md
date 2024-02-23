<h1 align="center">Awesome Minimalist</h1>

<div align="center" markdown="1">

**简体中文** / [English](README.en.md)

</div>

记录极简主义内容的博物馆，比如最小的网站，最小的图片等。

## 网站

+   制作不到 1 KB 的网站（[Making a Website Under 1kB](https://btxx.org/posts/1kb/)）

    Bradley Taunt 编写了非常小的个人简历，不到 1 KB。即使缺少了 html、head 和 body 元素，这也是合法的 HTML5 网站。

+   世界上最短的域名

    `http://ai/` 是世界上最短的域名，.ai 是英国海外属地安圭拉的域名，ICANN 的意见是不允许直接使用顶级域。
    不过安圭拉没有遵守这点。

    现在的 ai 域名不再被正常使用了，请前往 Internet Archive 查看之前的快照：
    <https://web.archive.org/web/20201111192639/http://www.ai/>

+   [htmz - a low power tool for html](https://leanrada.com/htmz/#examples)

    htmz 是一个极简 HTML 片段，没有任何外部依赖，就能实现点击链接，更新页面的部分内容为其他 URL。
    做到类似于 XHR、AJAX 的功能。

## 多媒体

+   世界上最小的 PNG 格式图片（[The world's smallest PNG](https://evanhahn.com/worlds-smallest-png/)）

    Evan Hahn 根据 PNG 格式规范，制作出了最小的 PNG 格式图片，仅有 67 bytes。

+   有史以来最小的 GIF（[The Tiniest GIF Ever](http://probablyprogramming.com/2009/03/15/the-tiniest-gif-ever)）

    Probably Programming 博客的作者发布了文章，介绍了自己探索最小的 GIF 格式图片的过程，
    并给出了数种最小的 GIF 格式图片。

    +   最小的透明 GIF 格式图片：37 bytes。
    +   最小的白色 GIF 格式图片：35 bytes。（[Chris Coyier][cc] 创建了黑色版本）
    +   最小的未定义颜色 GIF 格式图片：26 bytes。（不同的图像解码器会显示为不同的颜色）

    附言：Proger 的 [文章][pro] 里，提到了仅有 14 bytes 的 GIF 格式图片，不过只能被少数解码器解析。

    [cc]: https://css-tricks.com/snippets/html/base64-encode-of-1x1px-transparent-gif/

    [pro]: <https://web.archive.org/web/20231113134754/http://proger.i-forge.net/Компьютер/[20121112] The smallest transparent pixel.html>

+   最小的 JPEG 格式图片

    2008 年，Jesse_hz 在论坛发布帖子 [Worlds Smallest, Valid JPEG?][jpeg]（世界上最小的、有效的 JPEG？），
    给出了仅 134 bytes 的 JPEG 格式图片，但是没有探索过程。

    2010 年，matja 在 Stack overflow 的 [What is the smallest valid jpeg file size (in bytes)][jpeg2] 问题中，
    给出了仅 125 bytes 的最小 JPEG 格式图片，它符合 JPEG 标准，但不被多数解码器解码的（在当时）。
    并提到 Jesse_hz 的图片缺少 EOI，不符合 JPEG 标准。

    之所以最小的 JPEG 格式图片，比 PNG、GIF 格式图片大上不少，可能是因为前者是有损格式，后者是无损格式，设计上存在差异。

    [jpeg]: https://web.archive.org/web/20111224041840/http://www.techsupportteam.org/forum/digital-imaging-photography/1892-worlds-smallest-valid-jpeg.html

    [jpeg2]: https://stackoverflow.com/questions/2253404/what-is-the-smallest-valid-jpeg-file-size-in-bytes/2349470#2349470

+   用途

    这种 1 × 1 px 图片在曾被用来作为 [网络信标][wb]，一些网站、电子邮件中会含有透明的图片。
    用户阅读电子邮件时，活动时间、IP 地址等信息就会被记录。是一种险恶的滥用行为，
    现在常见邮箱基本都不会默认加载外部资源，所以基本不用担心了。

    更早之前，CSS 还没有垄断网页样式的时期，人们可能会使用各种 GIF 格式图片来设计网页样式。
    比如深色背景其实是 1 px 图片平铺出来的，或者使用不同大小的图片来排列组装网页（这被叫做 [垫片 GIF][sgif]）。

    现在即使没有什么其他的作用，还是有人，比如像 [Jon Sneyers][jos]，仍在继续探索各种图片格式的最小情况，
    因为这也是学习图像格式规范的好方法。

    [wb]: https://en.wikipedia.org/wiki/Web_beacon

    [sgif]: https://en.wikipedia.org/wiki/Spacer_GIF

    [jos]: https://cloudinary.com/blog/one_pixel_is_worth_three_thousand_words
