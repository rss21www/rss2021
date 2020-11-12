---
layout: page
title: Workshops
description: Workshop times, venues, and details.
days: ['SUN', 'MON']
room_pictures: ['32-123', '32-124', '32-141', '32-144', '32-155', '36-112', '36-144', '36-153', '36-155', '36-156', '34-101', '34-301', '34-302']
invisible: False
---


Workshops will take place July 12 and 13, 2020. They are generally scheduled to take place between 7:00AM PST and 11:15PM PST (14:00-18:15 UCT), and are recommended to have coffee breaks from 9:15-9:30AM and 11:15-11:30AM PST. However, each workshop is organized as a semi-independent event, and has a unique schedule that may deviate from the recommended schedule. Please check the workshop websites for more details on their particular schedules.

{% comment %}
[Here]({{ site.baseurl }}/docs/campusmap.pdf) is a labeled map of the workshop buildings.
{% endcomment %}




{% for day in page.days %}
{% if day == 'SUN' %}
#### Sunday, July 12  {#sun}
{% elsif day == 'MON' %}
#### Monday, July 13    {#mon}
{% endif %}


<table class="table table-striped table-workshop">
  <thead>
    <tr>
      <th width="15%" align="center">WS</th>
      <th width="36%">Title</th>
      <th width="30%">Organizers</th>
      <th width="20%">Virtual Session Link</th>
    </tr>
  </thead>
  <tbody>
    {% for workshop in site.data.workshops %}
    {% if workshop.date contains day %}

	{% if workshop.external_id == 'WS1-1' or workshop.external_id == 'WS1-7' %}
       <tr>
      <td> <s> {{ workshop.external_id }} </s></td>
      <td> <s>
        <a href="{{ workshop.url }}">
          {{ workshop.title }}
        </a> </s>
      </td>
      <td>
	<s>
        {{ workshop.organizers | replace: ',', '<br/>' }}
 	</s>
      </td>
	<td>
        <s> N/A </s>
	</td>
     
          </tr>
    
    {% else %}
    <tr>
      <td>{{ workshop.external_id }}</td>
      <td>
        <a href="{{ workshop.url }}">
          {{ workshop.title }}
        </a>
      </td>
      <td>
        {{ workshop.organizers | replace: ',', '<br/>' }}
      </td>     

<td> <a href="{{ workshop.pheedloop }}">
          [Session]
        </a> </td>
    </tr>
	{% endif %}
    {% endif %}
    {% endfor %}
  </tbody>
</table>
{% endfor %}

