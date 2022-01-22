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

<div class="alert">
  <b>The Redding Lab is looking to hire at the postdoctoral level for a number projects investigating 
  protein-chromatin interactions and genome organization. If interested send an inquiry and C.V. to 
  sy dot redding at umassmed dot edu
  </b>
</div>

<h2>Redding Lab members</h2>

{% for people in site.people %}
<hr>
<div class="row">
    <div class="col-md-4">
        <img class = "img-fluid" src = "{{people.image}}" alt = "Key Figure" style="max-height: 200px;">
    </div>
    <div class="col-md-8">
        <div><h5>{{ people.name | markdownify }}</h5>
        {{people.position}} <br>
        <em>{{people.email}}</em> <br>
        </div>
    </div>
</div>
{% endfor %}
