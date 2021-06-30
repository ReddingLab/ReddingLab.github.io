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
  <b>The Redding Lab is looking to hire at the Research Specialist 
  and Technician levels. Contact the lab for more information</b>
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
        {% if people.website %}
            <a style="overflow-wrap: break-word;" href= "{{people.website}}">{{people.website}}</a> <br>
        {% endif %}
        {% if people.twitter %}
            <a href="http://twitter.com"><img class="inline-block mem-icon" src="/static/img/twitter2_logo.svg"></a>
            <a href= "http://twitter.com/{{member.twitter}}"> @{{people.twitter}} </a> <br>
        {% endif %}
        {% if people.github %}
            <a href="http://github.com"><img class="inline-bloc mem-icon" src="/static/img/github_logo.svg"></a>
            <a href= "http://github.com/{{member.github}}"> {{people.github}} </a> <br>
        {% endif %}
        </div>
    </div>
</div>

{% endfor %}
