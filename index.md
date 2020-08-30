---
layout: splash
feature_row:
  - title: "Airmen Coders"
    excerpt: "Learn more about our projects."
    url: "/projects/"
    btn_label: "Go to Projects"
    btn_class: "btn--inverse"
  - title: "Space Coders"
    excerpt: "Learn more about coding, DevSecOps, and enjoy our list of free courses."
    url: "/learn/"
    btn_label: "Start Learning"
    btn_class: "btn--inverse"
  - title: "Marine Coders"
    excerpt: "Learn more about the Air Force's software goals and enabling platforms on the Chief Software Officer's website."
    url: "https://software.af.mil"
    btn_label: "CSO Website"
    btn_class: "btn--inverse"
---
  
<br /><br />
![Airmen Coders logo with #BuiltByAirmen](/assets/images/AirmenCodersFull500x276.png){: .align-center}  

<p align="center">We are a group of U.S. Air Force Airmen who use code to improve the lives of our fellow Airmen.</p>
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



