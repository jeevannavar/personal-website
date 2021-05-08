---
layout: page
title: The Hindustan Grimes
permalink: /thegrimes/
---

<h3> {{ page.title }} </h3>

Here are articles I've written for <a href="https://thegrimes.substack.com" target="_blank">The Hindustan Grimes</a>. The newsletter goes out once a week, on the Friday, and has three articles each issue. <a href="https://saiguha.com" target="_blank">Momo</a> and I write articles for the newsletter. Here, I've listed articles that I've written.  
<br>

<table style="width:100%; border-spacing: 15px;">
	{% for post in site.categories.thegrimes %}
	<tr>
		 <td id="grimes-date" width="25%" style="padding-right: 10px; padding-bottom: 10px;">
		 	{{ post.date | date_to_string }}
		 </td> 
		 <td style="padding-bottom: 10px">
			 <a href="{{ post.url }}">{{ post.title }}</a>
		 </td> 
	</tr>			 
	{% endfor %}
</table>
