---
layout: page
title: Search
permalink: /search/
description: Search anything in the site from here.
published: false
---




<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="Search..." autofocus>
</div>
<div id="results-container"></div>

<!-- Script pointing to jekyll-search.js -->
<script src="{{site.baseurl}}/js/jekyll-search.min.js" type="text/javascript"></script>
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<a class="nostyle" href="{url}"><div class="blog cards"><div class="image" style="background-image: url({image});"></div><div class="content"><h3 class="title">{title}</h3><p class="description">{description}</p></div></div></a>',
  noResultsText: 'No results found',
  json: '{{site.baseurl}}/search.json'
})
</script>

<!-- <a class="nostyle" href="{url}"><div class="blog cards rev"><div class="image" style="background-image: url({image});"></div><div class="content"><h3 class="title">{title}</h3><p class="description">{description}</p></div></div></a> -->