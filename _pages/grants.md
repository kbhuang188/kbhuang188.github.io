---
layout: single
title: "Grants"
permalink: /grants/
---

## National Science and Technology Council (國科會)

{% assign nstc = site.data.grants | where: "category", "National Science and Technology Council (國科會)" %}
{% for g in nstc %}
- **{{ g.title }}** ({{ g.period }}) — {{ g.role }}  
  Sponsor: {{ g.sponsor }}  
  Tags: {{ g.tags | join: ", " }}
  {% if g.link and g.link != "" %} — [Read more]({{ g.link }}){% endif %}
{% endfor %}

---

## Industry-Academia Cooperation (產學合作)

{% assign industry = site.data.grants | where: "category", "Industry-Academia Cooperation (產學合作)" %}
{% for g in industry %}
- **{{ g.title }}** ({{ g.period }}) — {{ g.role }}  
  Sponsor: {{ g.sponsor }}  
  Tags: {{ g.tags | join: ", " }}
  {% if g.link and g.link != "" %} — [Read more]({{ g.link }}){% endif %}
{% endfor %}
