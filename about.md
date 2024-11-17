---
layout: page
title: Haoyi Zeng
permalink: /
pubs:
    - title:   "The Blurred Drinker Paradox and Blurred Choice Axioms for the Downward Löwenheim-Skolem Theorem"
      author:  "Dominik Kirst, Haoyi Zeng"
      conference: "Draft"

    - title:   "Post’s Problem in Constructive Mathematics"
      author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst"
      conference: "Draft"

    # - title:   "Destabilizing Iris"
    #   author:  "Simon Spies, Niklas Mück, Haoyi Zeng, Michael Sammler, Andrea Lattuada, Peter Müller, Derek Dreyer"
    #   conference: "Submitted to PLDI 2025"
    #   url:     "http://publish-more-stuff.org"

workshops:
    - title:   "Kawa: An Abstract Language for Scalable and Variable Detection of Spectre Vulnerabilities"
      author:  "Zheyuan Wu, Haoyi Zeng, Aaron Bies"
      conference: "SRC SPLASH 2024 (🥉 3rd place in the undergraduate category)"
      url:     "https://dl.acm.org/doi/10.1145/3689491.3689971"

    - title:   "Post’s Problem in Constructive Mathematics"
      author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst, Takako Nemoto"
      conference: "CCC 2024"
      url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/CCC2024_Post.pdf"

    - title:   "Constructive Reverse Mathematics of the Downward Löwenheim-Skolem Theorem"
      author:  "Dominik Kirst, Haoyi Zeng"
      conference: "Logic Colloquium 2024"
      url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/LC_2024_LS.pdf"

    - title:   "Post’s Problem and the Priority Method in CIC"
      author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst"
      conference: "TYPES 2024"
      url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/TYPES_2024_Post.pdf"

    - title:   "The Blurred Drinker Paradox and Blurred Choice Axioms for the Downward Löwenheim-Skolem Theorem"
      author:  "Dominik Kirst, Haoyi Zeng"
      conference: "TYPES 2024"
      url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/TYPES_2024_LS.pdf"

ongoing:
    - title: "Formalizing Hardware-Software Contracts in Lean"
      author: "Haoyi Zeng, Thomas Bourgeat"
---

{% include image.html url="images/Duessedorf.jpg" width="200px" align="right" %}

Hey, I'm a computer science bachelor student at [Saarland University]. 
I'm broadly interested in programming languages, verification, hardware design, and type theory.

<!-- **Email:** (λx. λy. x00001@stud.uni-y.de) (haze) (saarland) -->
📬 (λx. λy. x00001@stud.uni-y.de) (haze) (saarland)

<br>

---
### Ongoing Projects
{% for pub in page.ongoing %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {{ pub.author }}<br />
    <i>{{ pub.conference }}</i><br />
    {% if pub.note %} <i>({{ pub.note }})</i> {% endif %} <i>{{ pub.year }}</i>
    {% if pub.doi %} [[doi]({{ pub.doi }})] {% endif %}
    {% if pub.media %}
      <br />Talk: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank">{{ article.name }}</a>
        <!-- <a href="{{ article.url_c}}" target = "_black">{{ article.conference}} </a> -->
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}

---
<!-- ### Publications -->
### Research Papers
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
    <i>{{ pub.conference }}</i><br />
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

----
### Extended Workshop Abstracts
{% for pub in page.workshops %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {{ pub.author }}<br />
    <i>{{ pub.conference }}</i><br />
    {% if pub.note %} <i>({{ pub.note }})</i> {% endif %} <i>{{ pub.year }}</i>
    {% if pub.doi %} [[doi]({{ pub.doi }})] {% endif %}
    {% if pub.media %}
      <br />Talk: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank">{{ article.name }}</a>
        <!-- <a href="{{ article.url_c}}" target = "_black">{{ article.conference}} </a> -->
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}




---

### Achievements

- [Summer@EPFL](https://summer.epfl.ch/) Fellowship
- German National Scholarship (Deutschlandstipendium)
- Bachelor’s Honors Program 

---
### Teaching
I'm a TA for a number of courses at UdS.
- Saarland University: [**Introduction to Computational Logic**](https://cms.sic.saarland/icl_23/) (2023)
- Saarland University: [**Programming 2**](https://cms.sic.saarland/prog2_23/) (2023)
- Saarland University: [**Programming 2 Pre-Course**](https://cms.sic.saarland/p2vorkurs23/) (2023)

---

### Events
- SPLASH 2024
- TYPES 2024
- Iris Workshop 2023/2024
- Proof and Computation 2023

<br>
---
---
If you are tired, take a look at [Baloo].

[Saarland University]: https://saarland-informatics-campus.de/
[Baloo]: https://zheyuanwu.github.io/baloo.html