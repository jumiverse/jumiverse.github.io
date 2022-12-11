---
layout: post
title:  blog
date:   2022-12-11 12:24:49 +0100
categories: blog
pagination: 
  enabled: true
---
--- 
 
 <h1 align="center">Welcome to the</h1>
 <p align="center">
  <br>
  <img src="../logo.png?sanitize=true" width="200px" height="200px">
</p>
 <h1 align="center">JuMiblog</h1>
 
## Categories 

<html>  
 <body>
<!-- Menu link fragment #id should match a div id. Example: <a href="#home"> links to <div id="home"></div>  -->
      <p align="center">
      <ul class="main-menu">
        <li><a href="#eat">🥘 eat</a></li>
        <li><a href="#move">🚶move</a></li>
        <li><a href="#learn">:book: learn</a></li>
      </ul>                 
      </p>
<!-- Posts -->
<ul id="posts">

	{% for post in paginator.posts %}

	  <li class="post">
	  	<h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
	  	<time datetime="{{ post.date | date_to_xmlschema }}" class="by-line">{{ post.date | date_to_string }}</time>
	  	<p>{{ post.content | strip_html | truncatewords:50 }}</p>
	  </li>

    {% endfor %}

</ul>
 </body>
</html>

<div id="container">
      <div class="inner">
        <div id="content"> 
          <div id="eat" class="content-region hide">
            <h2>eat</h2>
            <p>
              <br>
              <a href="https://mariaseltmann.github.io/blog/recipes.html"><strong>recipes »</strong></a>
            </p>
          </div>
	<div id="move" class="content-region hide">
            <h2>move</h2>
            <p>
              <br>
              <a href="https://mariaseltmann.github.io/blog/recipes.html"><strong>all about health »</strong></a>
            </p>
          </div>
	 <div id="learn" class="content-region hide">
            <h2>learn</h2>
            <p>
              <br>
              <a href="https://mariaseltmann.github.io/blog/recipes.html"><strong>articles, books, ted talks »</strong></a>
            </p>
          </div>
	</div>
    </div>
</div>
		
## Fun of the day
![](https://pranjaldhole.github.io/images/evolution.jpg)

## About us
<p>
              <br>
              <a href="https://mariaseltmann.github.io/blog/meet-jugan.html"><strong>Meet Jugan »</strong></a>
              <br>
              <a href="https://mariaseltmann.github.io/blog/meet-mia.html"><strong>Meet Mia »</strong></a>
              <br>
            </p>
