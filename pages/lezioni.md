---
layout: page
format: blog-index
# Don't index these pages dear Google.
noindex: true
title: "Lezioni svolte"
#subheadline: "Informazioni"
teaser: ""
permalink: /lezioni/
header: no
---
<posts>
        <table>
            {% for post in site.categories.lezioni reversed %}
            <tr>
                <td width="25%" class='date'>{{post.data}}</td>  
                <td>{{ post.args }}</td>
            </tr>
            <tr>
                <td colspan='2'>
                {{ post.excerpt }}
                </td>
            </tr>
    	{% endfor %}
        </table>
</posts>



