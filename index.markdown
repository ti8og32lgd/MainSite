---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


# All Blogs
<table>
    <tr><th>title</th> <th>link</th> <th>time</th> </tr>
    {% for post in site.posts %}
    <tr>
    <td>{{ post.title }}</td>
    <td>
        <a href="/{% if jekyll.environment=='production' %}{{site.github.repository_name}}{% endif %}{{ post.url }}">{{ post.url }}</a>
    </td>

      <td>{{ post.date| date: "%Y-%m-%d %H:%M" }}</td>

    </tr>
    {% endfor %}
  </table>
