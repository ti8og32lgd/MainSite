---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
date: 2022-10-20 15:04:05
permalink: /test/collection
---


<table>    <tr><th>collections</th> </tr>
{% for unit in site.my_collection %}
<tr>
<td><a href="{{unit.url}}">
            {{ unit.title }}
        </a></td>
</tr>
{% endfor %}
</table>
