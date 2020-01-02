---
layout: page
title: Program Committee
description: Reviewing team.
---

 <div id="area-chairs" class="row text-center">
    <b>Program Chair</b><br>
        <a href="http://ipvs.informatik.uni-stuttgart.de/mlr/marc/">Marc Toussaint</a><br>
		<i>University of Stuttgart</i><br>
            <br>

	<b>Area Chairs</b><br>
    {% for member in site.data.acs %}
    {% capture modulo %}{{ forloop.index0 | modulo:3 }}{% endcapture %}
    {% if modulo == '0' %}<div class="row text-center">{% endif %}
        <div class="col-sm-6">
            <a href="{{ member.Link }}">{{member.Name}}</a><br>
		<i>{{ member.Affiliation }}</i><br>
		<a href="{{ member.Scholar }}">Google Scholar</a><br>
            <br>
        </div>
    {% if modulo == '3' or forloop.last %}</div>{% endif %}
    {% endfor %}
 </div>



{% comment %}
<ul class="two-col text-left" style="list-style: none;">
{% for member in site.data.pc %}
<li>{{ member.FirstName }} {{ member.LastName }} (<i>{{ member.Organization }}</i>)</li>
{% endfor %}
</ul>
{% endcomment %}
