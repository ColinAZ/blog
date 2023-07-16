---
title: "我🈴博客"
permalink: "/about/"
layout: page
author: 熊的猫
---

>大家好，我是`熊の猫`。欢迎光临我的博客，它的名字叫`放牧`，网址也挺好记的——`fang.mu`。《东观汉记·光武纪》：商贾重宝，单车露宿，牛马放牧，道无拾遗。随着钢筋水泥的丛林越来越拥挤，年至中场的我突然发现自己越来越向往遥不可及的远方。远方有多远，远方有什么，我都不得而知，但它就像一个乌托邦，时时刻刻如北极星一般指引我往前走。本来博客还有其他一些更具市井气息的表达，但是偶然间翻书的时候看到了一个熟悉的词汇——`放牧`，慕然感到顺势而为才是自己的追求，遂注册了的`fang.mu`这个域名，并启用。

不管您从何处来，我都高兴于您能在浩瀚如烟的互联网世界里发现这个博客，更感谢您能够饶有兴致地浏览这个页面。

自2016年第一篇博客起，这里已经悄悄地运行了 <span id="days"></span> 天，截至 {{ site.time | date: "%Y 年 %m 月 %d 日" }}，不知不觉已经写了 {{ site.posts.size }} 篇随笔杂记，累计起来已经有 {% assign count = 0 %}{% for post in site.posts %}{% assign single_count = post.content | strip_html | strip_newlines | remove: ' ' | size %}{% assign count = count | plus: single_count %}{% endfor %}{% if count > 10000 %}{{ count | divided_by: 10000 }} 万 {{ count | modulo: 10000 }}{% else %}{{ count }}{% endif %} 个字了。

![](https://public.jstatic.net/files/new-about.jpg)

三分钟热情的我总是写写、停停、修修、改改，最后不了了之。这里很有可能也会如此。暂且不管能坚持多久，我都希望这个地方是一个自由表达自己的地方。我将在此分享我对相关主题的看法。呃...我甚至还可能分享图片、视频以及其他有趣东西的链接。有人来看，有人评论，简单而有乐趣。每个人都能静静地看文章，都不哗众取宠，不讨好别人。

<iframe src="https://www.google.com/maps/d/embed?mid=1vzlspT4Bn9J1Mw2sFvntv-T9WZLGMA3v&ehbc=2E312F" width="100%" height="400"></iframe>

好好生活，好好工作，好好记录。每天多一点思考，每天就会多一点成长。

如果您有兴趣的话，欢迎给我来信。以下是我的几种联系方式：

><i class="fa-solid fa-envelope"></i>：blogmailⓐfoxmail.com
>
><i class="fa-brands fa-qq"></i>：5592112，[点我](http://wpa.qq.com/msgrd?v=3&uin=5592112&site=qq&menu=yes){:target="_blank"}
>
><i class="fa-brands fa-weixin"></i>：[微信点这，扫码加好友](https://www.douban.com/photos/photo/2625796574/){:target="_blank"}
>
><i class="fa-brands fa-telegram"></i>：fm789，[点我](https://t.me/fm876){:target="_blank"}

本博客采用 **[ <i class="fa-brands fa-creative-commons"></i> <i class="fa-brands fa-creative-commons-by"></i> <i class="fa-brands fa-creative-commons-nc"></i> <i class="fa-brands fa-creative-commons-sa"></i>](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh){:target="_blank"}** `（知识产权署名-非商业性使用 4.0 国际许可协议）`进行许可。

<script>
var days = 0, daysMax = Math.floor((Date.now() / 1000 - {{ "2016-05-05" | date: "%s" }}) / (60 * 60 * 24));
(function daysCount(){
    if(days > daysMax){
        document.getElementById('days').innerHTML = daysMax;
        return;
    } else {
        document.getElementById('days').innerHTML = days;
        days += 10;
        setTimeout(daysCount, 1); 
    }
})();
</script>
