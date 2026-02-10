---
layout: page
title: Publications
permalink: /publications/
---

{% for pub in site.data.publications %}
### {{ pub.title }}

**{{ pub.authors }}**  
*{{ pub.journal }}*, {{ pub.year }}

{% if pub.links %}
[
{% if pub.links.pdf %}PDF{% endif %}
{% if pub.links.doi %} · DOI{% endif %}
{% if pub.links.code %} · Code{% endif %}
]
{% endif %}

{% endfor %}
