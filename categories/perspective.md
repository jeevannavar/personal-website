---
layout: page
title: "Perspective: My Approach"
permalink: /perspective/
---

<h3> {{ page.title }} </h3>

This list contains articles I wrote when I was still a teenager. A few of them are decent. A few of them might make you, and likely me too, cringe. I keep it here to remind myself that future me will look at present me with the same pity that I currently view teenage me with. I do hope that that happens. Have to keep improving.  
<br>

<table style="width:100%">
	{% for post in site.categories.perspective %}
	<tr>
		 <td>{{ post.date | date_to_string }}</td> 
		 <td>
			 <a href="{{ post.url }}">{{ post.title }}</a>
		 </td> 
	</tr>			 
	{% endfor %}
</table>

