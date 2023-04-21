---
title: "Afbeeldingen - Reverse"
keywords: afbeeldingen reverse
tags: [afbeeldingen]
sidebar: tools_sidebar
permalink: afbeeldingen-reverse.html
datatable: true
---

<table class="display">
	<thead>
		<tr class="header">
			<th>Type</th>
			<th>Regio</th>
			<th>Link</th>
			<th>Beschrijving</th>
		</tr>
	</thead>
{% for item in site.data.tools.afbeeldingen_reverse %}
	<tr>
		<td>
			{{ item.type }}
		</td>
		<td>
			{{ item.region }}
		</td>
		<td>
			<a href="{{ item.url }}" target="{{ item.target }}">
				{{ item.title }}
			</a>
		</td>
		<td>
			{{ item.description }}
		</td>
	</tr>
{% endfor %}
</table>