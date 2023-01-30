---
title: "作者博客"
permalink: "/about/"
layout: page
author: 熊的猫
---

>大家好，我是`熊の猫`。欢迎光临我的博客，它叫`爨博客`。
>`写志`：汉语词语，意思为抒发情志。这也刚好符合我个人博客的意义，这种存在犹如网络树洞般的奇妙。

不管您从何处来，我都高兴于您能在浩瀚如烟的互联网世界里发现这个博客，更感谢您能够饶有兴致地浏览这个页面。

自2016年第一篇博客起，这里已经悄悄地运行了 <span id="days"></span> 天，截至 {{ site.time | date: "%Y 年 %m 月 %d 日" }}，不知不觉已经写了 {{ site.posts.size }} 篇随笔杂记，累计起来已经有 {% assign count = 0 %}{% for post in site.posts %}{% assign single_count = post.content | strip_html | strip_newlines | remove: ' ' | size %}{% assign count = count | plus: single_count %}{% endfor %}{% if count > 10000 %}{{ count | divided_by: 10000 }} 万 {{ count | modulo: 10000 }}{% else %}{{ count }}{% endif %} 个字了。

![](https://files.oicp.io/files/new-about.jpg)

三分钟热情的我总是写写、停停、修修、改改，最后不了了之。这里很有可能也会如此。暂且不管能坚持多久，我都希望这个地方是一个自由表达自己的地方。我将在此分享我对相关主题的看法。呃...我甚至还可能分享图片、视频以及其他有趣东西的链接。有人来看，有人评论，简单而有乐趣。每个人都能静静地看文章，都不哗众取宠，不讨好别人。

好好生活，好好工作，好好记录。每天多一点思考，每天就会多一点成长。

如果您有兴趣的话，欢迎给我来信。以下是我的几种联系方式：

>✉：8200ⓐ88.com（注意：ⓐ=@）
>
>QQ：5592112，[点我](http://wpa.qq.com/msgrd?v=3&uin=5592112&site=qq&menu=yes){:target="_blank"}
>
>微信：[微信点这，扫码加好友](https://www.douban.com/photos/photo/2625796574/){:target="_blank"}
>
>Telgram：fm789，[点我](https://t.me/fm876){:target="_blank"}

本博客采用 **[知识产权署名-非商业性使用 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh){:target="_blank"}** 进行许可。

最后特别感谢[@Fooleap](https://blog.fooleap.org/){:target="_blank"} 、 [@钛客志](https://fffou.com/){:target="_blank"} 和  [@水八口](https://blog.shuiba.co/){:target="_blank"} 对本博客的帮助。

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
