---
layout: splash
feature_row:
  - title: "Airmen Coders"
    url: "https://airmencoders.us"
    btn_label: "Visit"
    btn_class: "btn--inverse"
  - title: "Space Coders"
    url: "https://spacecoders.us"
    btn_label: "Visit"
    btn_class: "btn--inverse"
  - title: "Marine Coders"
    url: "https://marinecoders.us"
    btn_label: "Visit"
    btn_class: "btn--inverse"
---
  
<br /><br />

<p align="center">Visit our Service Coding Organizations</p>
<br /><br />
{% include feature_row %}
  
<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}

{% include paginator.html %}



