---
layout: default
permalink: /search.html
title: Jason Zerbe's draftbook | Search
---

<div data-role="page">
    <div data-role="header" data-tap-toggle="false">
        <a rel="external" href="/index.html" data-icon="user">about</a>
        <h1>{{ page.title }}</h1>
        <a rel="external" href="/search.html" data-icon="search">search</a>
    </div>

    <div data-role="content">
        <div id="cse" style="width: 100%;">Loading</div>
        <script src="http://www.google.com/jsapi" type="text/javascript"></script>
        <script type="text/javascript">
            google.load('search', '1', {language : 'en', style : google.loader.themes.MINIMALIST});
            google.setOnLoadCallback(function() {
                var customSearchOptions = {};
                var customSearchControl = new google.search.CustomSearchControl('014722425947596152422:uikm2inm8ae', customSearchOptions);
                customSearchControl.setResultSetSize(google.search.Search.FILTERED_CSE_RESULTSET);
                customSearchControl.draw('cse');
                customSearchControl.setLinkTarget(google.search.Search.LINK_TARGET_SELF);
            }, true);
        </script>
    </div>

    <div data-role="footer" data-tap-toggle="false">
        <div data-role="navbar" data-iconpos="left">
            <ul>
                <li><a rel="external" href="/tech.html" data-icon="gear">tech</a></li>
                <li><a rel="external" href="/trails.html" data-icon="location">trails</a></li>
                <li><a rel="external" href="/eats.html" data-icon="heart">eats</a></li>
            </ul>
        </div>
    </div>
</div>
