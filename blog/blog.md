 <h1 align="center">Welcome to the</h1>
 <p align="center">
  <br>
  <img src="../logo.png?sanitize=true" width="200px" height="200px">
</p>
 <h1 align="center">JuMiblog</h1>
 
## Features : 

<html>  
 <body>
<!-- Menu link fragment #id should match a div id. Example: <a href="#home"> links to <div id="home"></div>  -->
      <p align="center">
      <ul class="main-menu">
        <li><a href="#eat">🥘 eat</a></li>
        <li><a href="#move">🚶move</a></li>
        <li><a href="#sleep">😴 sleep</a></li>
      </ul>                 
      </p>
 </body>
</html>
     

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
	</div>
    </div>
</div>
		
### Fun of the day
![](https://pranjaldhole.github.io/images/evolution.jpg)

## About us
<p>
              Our Universe for writing posts.
              <br>
              <a href="https://mariaseltmann.github.io/blog/meet-jugan.html"><strong>Meet Jugan »</strong></a>
              <br>
              <a href="https://mariaseltmann.github.io/blog/meet-mia.html"><strong>Meet Mia »</strong></a>
              <br>
            </p>
