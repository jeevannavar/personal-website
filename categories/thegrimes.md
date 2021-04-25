---
layout: page
title: The Hindustan Grimes
permalink: /thegrimes/
---

<h3> {{ page.title }} </h3>

Here are articles I've written for <a href="https://thegrimes.substack.com" target="_blank">The Hindustan Grimes</a>. The newsletter goes out once a week, on the Friday, and has three articles each issue. <a href="https://saiguha.com" target="_blank">Momo</a> and I write articles for the newsletter. Here, I've listed articles that I've written.

<div style="padding: 20px; padding-left: 50px">
	{% for post in site.categories.thegrimes %}
	 <li>
		 <span style="display: inline-block; width:100px">
		 	{{ post.date | date_to_string }}
		 </span> 
		 &nbsp; 
		 <span>
			 <a href="{{ post.url }}">{{ post.title }}</a>
		 </span>
	 </li>
	{% endfor %}
</div> 
