---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


# All Blogs
<table>
    <tr><th>title</th> <th>time</th> </tr>
    {% for post in site.posts %}
    <tr>
    <td>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </td>

      <td>{{ post.date| date: "%Y-%m-%d %H:%M" }}</td>

    </tr>
    {% endfor %}
  </table>
