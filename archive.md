---
layout: page
title: Archive
---

<table class="table table-hover">
  <thead>
    <tr>
      <th>Title</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
	  {% for post in site.posts %}
	  <tr>
		<td> 
			<a href="{{ post.url }}">{{ post.title }}</a>
		</td>
		<td>
			{{ post.date | date: "%-d %B %Y" }}
		</td>
	  </tr>
	  {% endfor %}
  </tbody>
</table>