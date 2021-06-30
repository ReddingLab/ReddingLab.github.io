---
layout: page
title: Publications
permalink: /Publications/
---

<h2>Publications</h2>
<div class="container">

{% for publication in site.publications reversed %}
<hr>
<div class="row" style="padding-top: 60px; margin-top: -60px;" id="{{publication.pmid}}">
<div><h5>{{ publication.title | markdownify }}</h5>
{{ publication.authors | markdownify | remove: '<p>' | remove: '</p>' }}
{% if publication.journal %}
<i>{{ publication.journal }}.</i>
{{publication.pub_date}}.</div>
{% endif %}
</div>
<br>
<div class="row">
    <div class="col-md-6">
        {% if publication.pmid %}
		    <li>PMID: <a href="http://www.ncbi.nlm.nih.gov/pubmed/{{publication.pmid}}" alt = "pubmed link: {{publication.pmid}}"> {{publication.pmid}}</a></li>
	    {% endif %}
	    {% if publication.biorxiv %}
		    <li>Biorxiv Preprint: <a href="http://dx.doi.org/10.1101/{{publication.biorxiv}}" alt = "biorxiv preprint link: {{publication.biorxiv}}"> {{publication.biorxiv | split: "." | last }}</a></li>
		{% endif %}
		{% if publication.github %}
		<li>{% if publication.github.size > 1 %}Repositories:{%else%}Repository:{% endif %}
			{% for record in publication.github %}
				<a href="https://www.github.com/ReddingLab/{{record.url}}/">{{record.url}}</a>{% if record.description %} ({{record.description}}){% endif %}{% unless forloop.last %}, {% endunless %}
			{% endfor %}
		</li>
		{% endif %}
		{% if publication.links %}
			{% for link in publication.links %}
				<li><a href="{{link.url}}" alt="{{link.name}}">{{link.name}}</a></li>
			{% endfor %}
		{% endif %}	
    </div>
    <div class="col-md-6">
        <img class = "img-fluid" src = "{{publication.image}}" style="max-height: 300px;">
    </div>    
</div>
<br>

{% endfor %}

