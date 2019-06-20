---
layout: page
title: Organizing Committee
description: Organizing team.
---
<div>
    <div class="row text-center">
            <b>Program Chair</b><br>
            <a href="http://www.centropiaggio.unipi.it/~bicchi">Antonio Bicchi</a><br>
            <i>University of Pisa</i><br>
            <br>
            <b>General Chair</b><br>
            <a href="http://ipvs.informatik.uni-stuttgart.de/mlr/marc/index.html">Marc Toussaint</a><br>
            <i>University of Stuttgart</i><br>
            <br>
            <b>Local Arrangements Chair</b><br>
            <a href="https://eecs.oregonstate.edu/people/adams-julie" >Julie A. Adams</a><br>
            <i>Oregon State University</i><br>
			<a href="https://mime.oregonstate.edu/people/smart" >Bill Smart</a><br>
            <i>Oregon State University</i><br>
            <br>
            
            <br>
            <b>Web Chairs</b><br>
            <a href="https://scholar.google.com/citations?user=PIn36_wAAAAJ&hl=en">Jamison Heard</a><br>
            <i>Vanderbilt University</i><br>
            <br>
    </div>

{% comment %}
    <div id="area-chairs" class="row text-center">
        <b>Area Chairs</b><br>

    {% for member in site.data.areachairs %}
    {% capture modulo %}{{ forloop.index0 | modulo:3 }}{% endcapture %}

    {% if modulo == '0' %}<div class="row text-center">{% endif %}
        <div class="col-sm-4">
            <a href="{{ member.url }}">{{ member.name }}</a><br>
            <i>{{ member.affiliation }}</i><br>
            <br>
        </div>
    {% if modulo == '2' or forloop.last %}</div>{% endif %}

    {% endfor %}

    </div>
{% endcomment %}
</div>
