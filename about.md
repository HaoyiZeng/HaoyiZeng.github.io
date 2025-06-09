---
layout: page
title: Haoyi Zeng
permalink: /
pubs:
    - title:   "Post’s Problem in Constructive Mathematics"
      author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst, Takako Nemoto"
      conference: "Draft"
      url: "https://inria.hal.science/hal-04923365v1/"

    - title:   "The Blurred Drinker Paradox: Constructive Reverse Mathematics of the Downward Löwenheim-Skolem Theorem"
      author:  "Dominik Kirst*, Haoyi Zeng*"
      conference: "LICS"
      year: "2025"
      url: "https://lics.siglog.org/lics25/accepted.php"
      award: "⭐ Distinguished Paper"

    - title:   "Destabilizing Iris"
      author:  "Simon Spies, Niklas Mück, Haoyi Zeng, Michael Sammler, Andrea Lattuada, Peter Müller, Derek Dreyer"
      conference: "PLDI"
      year: "2025"
      url: "https://plv.mpi-sws.org/iris-daenerys/"

workshops:
    - title:   "Kawa: An Abstract Language for Scalable and Variable Detection of Spectre Vulnerabilities"
      author:  "Zheyuan Wu, Haoyi Zeng, Aaron Bies"
      conference: "SRC SPLASH "
      year: "2024"
      award: "🥉 3rd place in the undergraduate category"
      url:     "https://dl.acm.org/doi/10.1145/3689491.3689971"

    # - title:   "Post’s Problem in Constructive Mathematics"
    #   author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst, Takako Nemoto"
    #   conference: "CCC"
    #   year: "2024"
    #   url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/CCC2024_Post.pdf"

    # - title:   "Constructive Reverse Mathematics of the Downward Löwenheim-Skolem Theorem"
    #   author:  "Dominik Kirst, Haoyi Zeng"
    #   conference: "LC"
    #   year: "2024"
    #   url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/LC_2024_LS.pdf"

    - title:   "Post’s Problem and the Priority Method in CIC"
      author:  "Haoyi Zeng, Yannick Forster, Dominik Kirst"
      conference: "TYPES"
      year: "2024"
      url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/TYPES_2024_Post.pdf"

    # - title:   "The Blurred Drinker Paradox and Blurred Choice Axioms for the Downward Löwenheim-Skolem Theorem"
    #   author:  "Dominik Kirst, Haoyi Zeng"
    #   conference: "TYPES"
    #   year: "2024"
    #   url:     "https://www.ps.uni-saarland.de/~zeng/bachelor/TYPES_2024_LS.pdf"

ongoing:
    - title: "Formalizing Hardware-Software Contracts in Lean"
      author: "Haoyi Zeng, Thomas Bourgeat"
      # url:    "slides/hwsw_green.pdf"
---

{% include image.html url="images/Duessedorf.jpg" width="200px" align="right" %}

Hey, I'm a computer science bachelor student at [Saarland University]. 
I'm broadly interested in programming languages, verification, hardware design, and type theory.

<!-- **Email:** (λx. λy. x00001@stud.uni-y.de) (haze) (saarland) -->
📬 (λx. λy. x00001@stud.uni-y.de) (haze) (saarland)

📝 [Curriculum Vitae](CV/haoyi_CV.pdf)

### Upcoming Events
- SuRI@EPFL 2025 🇨🇭
- PLDI 2025 in Seoul 🇰🇷
- LICS 2025 in Singapore 🇸🇬

<br>

<!-- ---
### Ongoing Projects -->
### <span class="title-style">Ongoing Projects</span>
<hr class="title-line">

{% for pub in page.ongoing %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    {% if pub.url %}
      <strong style="font-size: 0.9em;"><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {% else %}
      <strong style="font-size: 0.9em;">{{ pub.title }}</strong><br />
    {% endif %}
    <span style="font-size: 0.9em;">{{ pub.author | replace: "Haoyi Zeng", "<span style='font-weight: 500; color: #999; '>Haoyi Zeng</span>" }}</span><br />
    <span style="font-family: Georgia, serif; font-variant: small-caps; font-size: 0.85em;">
  {{ pub.conference | downcase }} {{ pub.year }}</span>
    {% if pub.note %} <i style="font-size: 0.9em;">({{ pub.note }})</i> {% endif %} 
    <i style="font-size: 0.9em;">{{ pub.year }}</i>
    {% if pub.doi %} 
      <span style="font-size: 0.9em;">[[doi]({{ pub.doi }})]</span> 
    {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank" style="font-size: 0.9em;">{{ article.name }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}

<!-- ### Publications -->
<!-- ### Research Papers
{% for pub in page.pubs %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    {% if pub.url %}
      <strong><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {% else %}
      <strong>{{ pub.title }}</strong><br />
    {% endif %}
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
{% endfor %} -->

<!-- ---
### Research Papers -->
<!-- ### <span class="title-style">Research Papers </span> -->
### <span class="title-style">Research Papers</span> <span style="font-size: 0.6em;color: #999; margin-left: 10px;"><i>(* equal contribution)</i></span>

<hr class="title-line">

<!-- ### <span style="color: silver;">Research Papers</span> -->

{% for pub in page.pubs %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    {% if pub.url %}
      <strong style="font-size: 0.9em;"><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {% else %}
      <strong style="font-size: 0.9em;">{{ pub.title }}</strong><br />
    {% endif %}
    <span style="font-size: 0.9em;">{{ pub.author | replace: "Haoyi Zeng", "<span style='font-weight: 500; color: #999; '>Haoyi Zeng</span>" }}</span><br />
    <span style="font-family: Georgia, serif; font-variant: small-caps; font-size: 1.2em;">
      {{ pub.conference | downcase }}
      <span style="font-size: 0.75em;"> {{ pub.year }}</span>
      {% if pub.award %}
      <span style="font-size: 0.75em; color: #0a5c0a"> {{ pub.award | downcase}}</span>
      {% endif %}
    </span>
    {% if pub.note %} <i style="font-size: 0.9em;">({{ pub.note }})</i> {% endif %} 
    {% if pub.doi %} 
      <span style="font-size: 0.9em;">[[doi]({{ pub.doi }})]</span> 
    {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank" style="font-size: 0.9em;">{{ article.name }}</a>
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

<!-- ----
### Extended Workshop Abstracts -->

### <span class="title-style">Extended Workshop Abstracts<span style="font-size: 0.6em;color: #999; margin-left: 10px;"><i>(selected)</i></span>
<hr class="title-line">

{% for pub in page.workshops %}
<div style="display: flex; align-items: center; margin-bottom: 20px;">
  {% if pub.image %}
    <div style="margin-right: 20px;">
      {% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
    </div>
  {% endif %}
  <div>
    {% if pub.url %}
      <strong style="font-size: 0.9em;"><a href="{% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %}">{{ pub.title }}</a></strong><br />
    {% else %}
      <strong style="font-size: 0.9em;">{{ pub.title }}</strong><br />
    {% endif %}
    <span style="font-size: 0.9em;">{{ pub.author | replace: "Haoyi Zeng", "<span style='font-weight: 500; color: #999; '>Haoyi Zeng</span>" }}</span><br />
    <span style="font-family: Georgia, serif; font-variant: small-caps; font-size: 1.2em;">
      {{ pub.conference | downcase }}
      <span style="font-size: 0.75em;"> {{ pub.year }}</span>
      {% if pub.award %}
      <span style="font-size: 0.75em; color: #0a5c0a"> {{ pub.award | downcase}}</span>
      {% endif %}
    </span>
    {% if pub.doi %} 
      <span style="font-size: 0.9em;">[[doi]({{ pub.doi }})]</span> 
    {% endif %}
    {% if pub.media %}
      <br />Media: 
      {% for article in pub.media %}
        <a href="{{ article.url }}" target="_blank" style="font-size: 0.9em;">{{ article.name }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}



<!-- ---
### Achievements -->

### <span class="title-style">Achievements</span>
<hr class="title-line">

- [Summer@EPFL](https://summer.epfl.ch/) Fellowship
- German National Scholarship (Deutschlandstipendium)
- Bachelor’s Honors Program 

<!-- ---
### Thesis -->
### <span class="title-style">Thesis</span>
<hr class="title-line">
- Bachelor's thesis:
  [Post’s Problem and the Priority Method in Synthetic Computability](https://www.ps.uni-saarland.de/~zeng/bachelor/Zeng_thesis.pdf)

<!-- ---
### Teaching -->

### <span class="title-style">Teaching</span>
<hr class="title-line">
I'm a TA for a number of courses at UdS.
- Saarland University: [**Introduction to Computational Logic**](https://cms.sic.saarland/icl_25/) (2025)
- Saarland University: [**Introduction to Computational Logic**](https://cms.sic.saarland/icl_23/) (2023)
- Saarland University: [**Programming 2**](https://cms.sic.saarland/prog2_23/) (2023)
- Saarland University: [**Programming 2 Pre-Course**](https://cms.sic.saarland/p2vorkurs23/) (2023)

<!-- ---
### Events -->

### <span class="title-style">Events</span>
<hr class="title-line">
- **PLISS** 2025
- **SPLASH** 2024 
- **TYPES** 2024
- **Iris Workshop** 2023/2024/2025
- **Proof and Computation** 2023

<br>
---
---
If you are tired, take a look at [Baloo].

[Saarland University]: https://saarland-informatics-campus.de/
[Baloo]: https://zheyuanwu.github.io/baloo.html
