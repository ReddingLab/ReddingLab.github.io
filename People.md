---
layout: page
title: People
permalink: /People/
---

<style>
.alert {
  padding: 20px;
  background-color: #57c557;
  color: white;
}

.closebtn {
  margin-left: 15px;
  color: white;
  font-weight: bold;
  float: right;
  font-size: 22px;
  line-height: 20px;
  cursor: pointer;
  transition: 0.3s;
}

.closebtn:hover {
  color: black;
}
</style>

[//]: # <div class="alert">
[//]: #  <b>The Redding Lab is looking to hire at the postdoctoral level for a number projects investigating 
[//]: #  protein-chromatin interactions and genome organization. If interested send an inquiry and C.V. to 
[//]: #  sy dot redding at umassmed dot edu
[//]: #  </b>
[//]: # </div>"



<hr>
<div>
<img class="img-fluid" src="/static/img/people/group_2025.jpeg" alt="xx">
</div>

<h2>Current Redding Lab members</h2>

[comment]: <> (loop over postdocs)

{% for people in site.people %}
{% if people.status == "current" %}
{% if people.position_id == "postdoc" %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name }}</h5>
        <b>Position:</b> {{people.position}} <br>
        <b>Project:</b> {{people.project}} <br>
        <b>email:</b> <em>{{people.email}}</em> <br>
        </div>
    </div>
</div>
{% endif %}
{% endif %}
{% endfor %}

[comment]: <> (loop over grad students)

{% for people in site.people %}
{% if people.status == "current" %}
{% if people.position_id == "gradstudent" %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name }}</h5>
        <b>Position:</b> {{people.position}} <br>
        <b>Project:</b> {{people.project}} <br>
        <b>email:</b> <em>{{people.email}}</em> <br>
        </div>
    </div>
</div>
{% endif %}
{% endif %}
{% endfor %}

[comment]: <> (loop over associates)

{% for people in site.people %}
{% if people.status == "current" %}
{% if people.position_id == "associate" %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name }}</h5>
        <b>Position:</b> {{people.position}} <br>
        <b>Project:</b> {{people.project}} <br>
        <b>email:</b> <em>{{people.email}}</em> <br>
        </div>
    </div>
</div>
{% endif %}
{% endif %}
{% endfor %}

[comment]: <> (Sy)
{% for people in site.people %}
{% if people.position_id == "PI" %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name }}</h5>
        </div>
    </div>
</div>
{% endif %}
{% endfor %}

<h2>Former Redding Lab members</h2>

{% for people in site.people %}
{% if people.status == "former" %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name | markdownify }}</h5>
        <b>Redding Lab Position:</b> {{people.position}} <br>
        <b>Current Position:</b> <em>{{people.currentposition}}</em> <br>
        </div>
    </div>
</div>
{% endif %}
{% endfor %}
