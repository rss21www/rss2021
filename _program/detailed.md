---
layout: page
title: Detailed Program
description: Detailed schedule of the program.
priority: 9
invisible: false
---

* Our [**virtual conference site**](https://pheedloop.com/rss2020/virtual/)
hosts all live events, allows users to flexibly join workshops and
paper discussion sessions, interact with each other and sponsors, and
manages registration.
* All [**accepted papers with pre-recorded presentations**]({{ site.baseurl
}}/program/papers/) are now available.
* Our [**RSS youtube channel**](https://www.youtube.com/channel/UCeEbAUGjtBlzmqWO5u6VeGg) hosts all pre-recorded presentations, and will host recordings of the
live plenary sessions.
* Please find the [**workshop program**]({{ site.baseurl }}/program/workshops/) separately.

### Overview

<img src="{{ site.baseurl }}/images/schedule-crop.jpg"
       alt="Virtual Event Schedule" width = "700" /> 


<br/>

<center>
  <a class="btn btn-primary" href="#tue" role="button">Tuesday</a>
  <a class="btn btn-primary" href="#wed" role="button">Wednesday</a>
  <a class="btn btn-primary" href="#thu" role="button">Thursday</a>
</center>

<br/>

All times below are given in **Coordinated Universal Time (UTC)**.

<a name="tue">&nbsp;</a>

### Tuesday, July 14

<table class="table table-striped table-program">
  <tr>
    <td width="140px">14:15 - 15:00 UTC</td>
    <td>
      <b>Welcome & Opening</b>
      <br/>Marc Toussaint, Jens Kober, Antonio Bicchi, Hadas Kress-Gazit
    </td>
  </tr>
  <tr>
    <td width="140px">15:00 - 17:00 UTC</td>
    <td>
      <b>Live Paper Discussions #1-34</b>
	  <br/>
	  {% for paper in site.data.rss2020_papers %}
	  {% assign tmp = paper.PaperOrder | plus: 0 %}
      {% if tmp < 35 %}
	  #{{paper.PaperOrder }} <a href="{{ site.baseurl }}/program/papers/{{ paper.PaperOrder}}/">{{paper.PaperTitle}}</a>
	  <br/>
      {% endif %}
	  {% endfor %}
    </td>
  </tr>
  <tr>
    <td width="140px">17:00 - 17:45 UTC</td>
    <td>
      <b>Test of Time Award Talk + Q&A</b>
      <br/>Speakers: Frank Dellaert, Michael Kaess
      <br/>Moderator: Marc Toussaint
	  <br/>Title: <i>From Square Root SAM to GTSAM: Factor Graphs in Robotics</i>
    </td>
  </tr>
  <tr>
    <td width="140px">17:45 - 18:15 UTC</td>
    <td>
      <b>Test of Time Pabel Debate</b>
      <br/>Panelists: Frank Dellaert, Michael Kaess, Danica Kragic, Gaurav Sukhatme
	  <br/>Moderator: Marc Toussaint
    </td>
  </tr>
  <tr>
    <td width="140px">18:30 - 19:15 UTC</td>
    <td>
      <b>Early Career Award Keynote + Q&A</b>
      <br/>Speaker: Byron Boots
      <br/>Moderator: Marco Pavone
    </td>
  </tr>
</table>

<a name="wed">&nbsp;</a>

### Wednesday, July 15

<table class="table table-striped table-program">
  <tr>
    <td width="140px">14:00 - 15:00 UTC</td>
    <td>
      <b>Inclusion@RSS hosts: Future of Robotics Panel</b>
      <br/>Moderators: Torrie Edwards, Marwa ElDiwiny
    </td>
  </tr>
  <tr>
    <td width="140px">15:00 - 17:00 PT</td>
    <td>
      <b>Live Paper Discussions #35-69</b>
	  <br/>
	  {% for paper in site.data.rss2020_papers %}
	  {% assign tmp = paper.PaperOrder | plus: 0 %}
      {% if tmp >= 35 and tmp < 70 %}
	  #{{paper.PaperOrder }} <a href="{{ site.baseurl }}/program/papers/{{ paper.PaperOrder}}/">{{paper.PaperTitle}}</a>
	  <br/>
      {% endif %}
	  {% endfor %}
    </td>
  </tr>
  <tr>
    <td width="140px">17:00 - 18:00 UTC</td>
    <td>
      <b>Keynote + Q&A</b>
      <br/>Speaker: Josh Tenenbaum
      <br/>Moderator: Marc Toussaint
	  <br/>Title: <i>It's all in your head: Intuitive physics, planning, and problem-solving in brains, minds and machines</i>

    </td>
  </tr>
  <tr>
    <td width="140px">18:00 - 18:30 UTC</td>
    <td>
      <b>Virtual Meetups</b>
    </td>
  </tr>
  <tr>
    <td width="140px">18:30 - 19:15 UTC</td>
    <td>
      <b>Early Career Award Keynote + Q&A</b>
      <br/>Speaker: Luca Carlone
      <br/>Moderator: Angela Schoellig
  <br/>Title: <i>The Future of Robot Perception: Certifiable Algorithms and Real-time High-level Understanding</i>

    </td>
  </tr>
</table>

<a name="thu">&nbsp;</a>

### Thursday, July 16

<table class="table table-striped table-program">
  <tr>
    <td width="140px">14:15 - 15:00 UTC</td>
    <td>
      <b>Discussion & Town Hall Meeting</b>
      <br/>Hadas Kress-Gazit, Antonio Bicchi, Marc Toussaint
    </td>
  </tr>
  <tr>
    <td width="140px">15:00 - 17:00 PT</td>
    <td>
      <b>Live Paper Discussions #70-103</b>
	  <br/>
	  {% for paper in site.data.rss2020_papers %}
	  {% assign tmp = paper.PaperOrder | plus: 0 %}
      {% if tmp >= 70 %}
	  #{{paper.PaperOrder }} <a href="{{ site.baseurl }}/program/papers/{{ paper.PaperOrder}}/">{{paper.PaperTitle}}</a>
	  <br/>
      {% endif %}
	  {% endfor %}
    </td>
  </tr>
  <tr>
    <td width="140px">17:00 - 17:45 UTC</td>
    <td>
      <b>Early Career Award Keynote + Q&A</b>
      <br/>Speaker: Jeannette Bohg
      <br/>Moderator: Stefanie Tellex
    </td>
  </tr>
  <tr>
    <td width="140px">18:00 - 18:45 UTC</td>
    <td>
      <b>Paper Awards & Farewell</b>
      <br/>TBA
    </td>
  </tr>
</table>
