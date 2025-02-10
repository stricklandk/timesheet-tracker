---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Timesheet Tracker
---
<h1>Timesheet Tracker</h1>
<table>
  <tr>
    <th>Date</th>
    <th>Project</th>
    <th>Hours</th>
  </tr>
  {% for entry in site.data.timesheets.entries %}
  <tr>
    <td>{{ entry.date }}</td>
    <td>{{ entry.project }}</td>
    <td>{{ entry.hours }}</td>
  </tr>
  {% endfor %}
</table>