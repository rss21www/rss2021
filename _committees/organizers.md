---
layout: page
title: Organizing Committee
description: Organizing team.
---
<div>
    <div class="row text-center">
            <b>Program Chair</b><br>
            <a href="http://ipvs.informatik.uni-stuttgart.de/mlr/marc/">Marc Toussaint</a><br>
            <i>University of Stuttgart</i><br>
            <br>
	    <b>General Chair</b><br>
            <a href="https://www.iit.it/people/antonio-bicchi">Antonio Bicchi</a><br>
            <i>University of Pisa</i><br>
            <br>
            <b>Local Arrangements Chairs</b><br>
            <a href="https://eecs.oregonstate.edu/people/adams-julie" >Julie A. Adams</a><br>
            <i>Oregon State University</i><br>
			<a href="https://mime.oregonstate.edu/people/smart" >Bill Smart</a><br>
            <i>Oregon State University</i><br>
            <br>
            <b>Publicity Chair</b><br>
            <a href="https://bicr.atr.jp/~xmorimo/">Jun Morimoto</a><br>
            <i>ATR Computational Neuroscience Laboratories</i><br>
            <br>
	    <b>Workshop Chairs</b><br>
            <a href="https://homes.cs.washington.edu/~mcakmak/" >Maya Cakmak</a><br>
            <i>University of Washingtion</i><br>
	    <a href="https://kkhauser.web.illinois.edu/" >Kris Hauser</a><br>
            <i>University of Illinois at Urbana-Champaign</i><br>
            <br>
	    <b>Presentation Chair</b><br>
            <a href="http://www.jenskober.de/">Jens Kober</a><br>
            <i>TU Delft</i><br>
            <br>
	    <b>Publication Chair</b><br>
            <a href="http://www.cs.utah.edu/~thermans/">Tucker Hermans</a><br>
            <i>University of Utah</i><br>
            <br>
	    <b>Inclusion Chair</b><br>
            <a href="TBD">TBD</a><br>
            <i>TBD</i><br>
            <br>
	    <b>RSS Pioneers Chair</b><br>
            <a href="https://patricialvesoliveira.com/">Patrícia Alves-Oliveira</a><br>
            <i>ISCTE-IU, INESC-ID, and Cornell University</i><br>
	    <a href="http://valentinp.com/">Valentin Peretroukhin</a><br>
            <i>University of Toronto</i><br>
            <a href="Thttps://patricialvesoliveira.com/">Patrícia Alves-Oliveira</a><br>
            <i>ISCTE-IU, INESC-ID, and Cornell University (</i><br>
            <br>
	    <b>Families@RSS Chair</b><br>
            <a href="TBD">TBD</a><br>
            <i>TBD</i><br>
            <br>
            <b>Web Chair</b><br>
            <a href="https://www.rit.edu/directory/jrheee-jamison-heard">Jamison Heard</a><br>
            <i>RIT</i><br>
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
