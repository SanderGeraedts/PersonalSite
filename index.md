---
permalink: /
layout: default
slug: home
---
<div>{% include avatar.html %}</div>{: .f-center }
Hi, mijn naam is Sander Geraedts, leuk om je op deze site te zien! Ik ben {{site.job}} bij [{{site.company}}]({{site.company_url}}) en amateur atleet. Op deze site schrijf ik van alles wat er in me op komt.
{: .t-center }
{% for post in site.posts limit:1 %}
## [{{post.title}}]({{post.url}})
{% include date.html date=post.date %}{: .date }
{{post.content}}
{% endfor %}
