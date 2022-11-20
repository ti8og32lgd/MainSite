---
layout: default
title: Variable test
---


<table>
  <tr>    <th>Variables</th>  </tr>
  <tr>
    <td>site.time </td> <td>{{site.time}} </td>
  </tr>

  <tr>
    <td>jekyll.environment</td>
    <td>{{jekyll.environment}}</td>
  </tr>
  <tr>
    <td>scope</td>
    <td>{{scope}}</td>
  </tr>

  <tr>
    <td>page.title</td>
    <td>{{page.title}}</td>
  </tr>
  <tr>
    <td>file.path</td>
    <td>{{file.path}}</td>
  </tr>
  <tr>
    <td>site.lang</td><td>{{site.lang}}</td>
  </tr>

</table>

# defined data
<ul>
{% for member in site.data.myConf %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>
