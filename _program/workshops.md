---
layout: page
title: Workshops
description: Workshop times, venues, and details.
days: ['SUN', 'MON']
room_pictures: ['32-123', '32-124', '32-141', '32-144', '32-155', '36-112', '36-144', '36-153', '36-155', '36-156', '34-101', '34-301', '34-302']
invisible: True
---


Workshops will take place July 12 and 13, 2020.
They will commence at 9:30 AM and end at 5:30 PM.
The workshop coffee breaks will be from 10:30 to 11:00 AM and 3:00 to 3:30 PM, with lunch scheduled for 12:00 - 2:00 PM.

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
      <th width="20%">Full/Half Day</th>
    </tr>
  </thead>
  <tbody>
    {% for workshop in site.data.workshops %}
    {% if workshop.date contains day %}
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
      <td> {{ workshop.day }} </td>          
    </tr>
    {% endif %}
    {% endfor %}
  </tbody>
</table>
{% endfor %}
