---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
---
##Career & IT Blog

{% for post in site.categories.career limit:1 %}
  {% include archive-single.html %}
{% endfor %}

[Career & IT](/blog/career/){: .btn .btn--primary .btn--large}

##Other Interests

{% for post in site.categories.personal limit:1 %}
  {% include archive-single.html %}
{% endfor %}

[Other Interests](/blog/other-interests/){: .btn .btn--info .btn--large}
