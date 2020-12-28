---
title: Archive
layout: blog
---

# Archive

<ul id="listing-archive">
	{% for post in site.posts %}
		<li>
			<time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time> - 
			<a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endfor %}
</ul>
