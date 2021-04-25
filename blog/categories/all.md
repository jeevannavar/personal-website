---
layout: page
title: Blog Categories
permalink: /blog/categories/
---


<h3>  {{ page.title }} </h3>
<br>

<div id="categories">
	{% for category in site.categories %}
	  <div class="category-box" >
	    {% capture category_name %}{{ category | first }}{% endcapture %}
	    <div id="#{{ category_name | slugize }}"></div>
	    <h4 class="category-head">
	    		<a href="{{ site.baseurl }}/blog/categories/{{ category_name }}">{{ category_name}}</a>
	    	</h4>
	    	<br>
	    <a name="{{ category_name | slugize }}"></a>
	    {% for post in site.categories[category_name] %}
	    <article class="center">
	      <h6 >
	      	<a href="{{ site.baseurl }}{{ post.url }}">&emsp;&emsp;{{post.title}}</a>
	      </h6>
	    </article>
	    {% endfor %}
	  </div>
	{% endfor %}
</div>


