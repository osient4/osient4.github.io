---
title: "Handelsregisters"
keywords: sample homepage
tags: [getting_started]
sidebar: tools_sidebar
permalink: handelsregisters.html
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
{% for handelsregister in site.data.tools.handelsregisters %}
	<tr>
		<td>
			{{ handelsregister.type }}
		</td>
		<td>
			{{ handelsregister.region }}
		</td>
		<td>
			<a href="{{ handelsregister.url }}" target="{{ handelsregister.target }}">
				{{ handelsregister.title }}
			</a>
		</td>
		<td>
			{{ handelsregister.description }}
		</td>
	</tr>
{% endfor %}
</table>