 <h1 align="center">Welcome to the</h1>
 <p align="center">
  <br>
  <img src="../logo.png?sanitize=true" width="200px" height="200px">
</p>
 <h1 align="center">JuMiblog</h1>
 
## Features : 
<!-- Menu link fragment #id should match a div id. Example: <a href="#home"> links to <div id="home"></div>  -->
      <p align="center">
      <ul class="main-menu">
        <li><a href="#eat">eat</a></li>
        <li><a href="#move">move</a></li>
        <li><a href="#sleep">sleep</a></li>
      </ul>                 
      </p>
      
- 🥘 eat
- 🚶 move
- 😴 sleep
- ❤️ repeat

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

### Fun of the day
![](https://pranjaldhole.github.io/images/evolution.jpg)

## About us
[Meet Mia](meet-mia.html)
<br>
[Meet Jugan](meet-jugan.html)

## Formatting

{% highlight markdown %}
 # This is a <h1> tag.
 ## This is a <h2> tag.
 <h3>, <h4>, <h5> and <h6> have the same style.
{% endhighlight %}

## Type-setting
Insert your text between two double asterisks to make it **bold**.

Insert your text between underscores to make it _italic_.

> This is a blockquote

### Unordered list
- list 1
- list 2
- list 3
- list 4

### Ordered list
1. one
2. two
3. three
4. four
