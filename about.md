---
layout: page
title: Haoyi Zeng
permalink: /
pubs:
    - title:   "Paper title in 3-7 words that sound like Clingon"
      author:  "M. McFly, D. Kirk, L. Skywalker, H.J. Potter, I. Jones, H. Houdini"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2016"
      url:     "http://publish-more-stuff.org"
      doi:     "http://dx.doi.org"
    #   image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"
workshops:
    - title:   "Paper title in 3-7 words that sound like Clingon"
      author:  "M. McFly, D. Kirk, L. Skywalker, H.J. Potter, I. Jones, H. Houdini"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2016"
      url:     "http://publish-more-stuff.org"
      doi:     "http://dx.doi.org"
    #   image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"
---


{% include image.html url="images/haoyi.jpg" width="200px" align="right" %}

Hey, I'm a computer science bachelor student at [Saarland University]. 
I'm broadly interested in these topics: programming languages, verification, and formal logic.

Email: (λx. λy. x00001@stud.uni-y.de) (haze) (saarland)

[Saarland University]: https://saarland-informatics-campus.de/
[Baloo]: https://zheyuanwu.github.io/baloo.html

---
### Pub
{% for pub in page.pubs %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {{ pub.author }}<br />
    <i>{{ pub.journal }}</i><br />
    {% if pub.note %} <i>({{ pub.note }})</i> {% endif %} <i>{{ pub.year }}</i>
    {% if pub.doi %} [[doi]({{ pub.doi }})] {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank">{{ article.name }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}



<!-- <button onclick="togglePubDetails()">Show Publications</button>

<div id="pub-details" style="display:none; margin-top: 10px;">
  {% for pub in page.pubs %}
  <div style="display: flex; align-items: center; margin-bottom: 20px;">
    {% if pub.image %}
      <div style="margin-right: 20px;">
        {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
      </div>
    {% endif %}
    <div>
      <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
      {{ pub.author }}<br />
      <i>{{ pub.journal }}</i><br />
      {% if pub.note %} <i>({{ pub.note }})</i> {% endif %} <i>{{ pub.year }}</i>
      {% if pub.doi %} [[doi]({{ pub.doi }})] {% endif %}
      {% if pub.media %}
        <br />Media: 
        {% for article in pub.media %}
          <a href="{{ article.url }}" target="_blank">{{ article.name }}</a>
        {% endfor %}
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>

<script>
  // Function to toggle the visibility of the publication details
  function togglePubDetails() {
    var pubDetails = document.getElementById('pub-details');
    if (pubDetails.style.display === "none") {
      pubDetails.style.display = "block";
    } else {
      pubDetails.style.display = "none";
    }
  }
</script> -->

---
### workshop
{% for pub in page.pubs %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {{ pub.author }}<br />
    <i>{{ pub.journal }}</i><br />
    {% if pub.note %} <i>({{ pub.note }})</i> {% endif %} <i>{{ pub.year }}</i>
    {% if pub.doi %} [[doi]({{ pub.doi }})] {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank">{{ article.name }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}




---
### Teaching
...

---
If you are tired, take a look at [Baloo].
