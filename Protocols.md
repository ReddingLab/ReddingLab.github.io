---
layout: page
title: Protocols
permalink: /Protocols/
---

<h2>Redding Lab Protocols</h2>

<h4>Assays</h4>
{% for protocol in site.protocols %}
{% if protocol.catagory == "assay" %}
[{{protocol.title}}]({{protocol.url}})       
{% endif %}
{% endfor %}

<h4>Reagents</h4>
{% for protocol in site.protocols %}
{% if protocol.catagory == "reagent" %}
[{{protocol.title}}]({{protocol.url}})       
{% endif %}
{% endfor %}

<h4>DNA</h4>
{% for protocol in site.protocols %}
{% if protocol.catagory == "DNA" %}
[{{protocol.title}}]({{protocol.url}})       
{% endif %}
{% endfor %}

<h4>Proteins</h4>
{% for protocol in site.protocols %}
{% if protocol.catagory == "protein" %}
[{{protocol.title}}]({{protocol.url}})       
{% endif %}
{% endfor %}



