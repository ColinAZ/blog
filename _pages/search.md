---
title: "搜索 / Search / 検索けんさく / 검색"
permalink: "/search/"
layout: page
author: 刘看山
---

<!-- HTML elements for search -->
<input type="text" id="search-input" placeholder="搜索博客 - 输入标题/相关内容/日期.." style="text-align:center"/>
<ul id="results-container"></ul>

<!-- script pointing to jekyll-search.js -->
<script src="/js/simple-jekyll-search.min.js"></script>

<script>
SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '/search.json',
    searchResultTemplate: '<li><a href="{url}" title="{desc}">{title}</a></li>',
    noResultsText: '没有搜索到文章',
    limit: 20,
    fuzzy: false
  })
</script>