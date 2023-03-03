---
layout: default
meta-description: "DeFOx: Decentralised Finance Research Group at Oxford"
---

# DeFOx
Technology is reshaping the future of the financial landscape and challenging traditional stakeholders. The aim of DeFOx is to discuss and promote academic and industrial work addressing the emerging challenges in finance. DeFOx focuses the attention on the recent and cutting-edge contributions to topics in decentralised finance and financial technology: economics, microstructure, models of liquidity taking and making, and new design paradigms that can help lay the foundations for the future financial landscape. 




{% for category in site.data.talks %}
# {{ category.type }}
<div class="talk-list">
  {% for talk in category.members %}
  <div class="talk list-group-item">
  <div class="talk-date">{{ talk.date }}</div>
  <div class="talk-presenter">{{ talk.speaker }}</div>
  {% if talk.title %}
  <div>
    {% if talk.recording %}
      <span><a class="talk-title-link" href="{{ talk.recording }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% elsif talk.livestream %}
      <span><a class="talk-title-link" href="{{ talk.livestream }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% else %}
      <span>{{ talk.title }}</span>
      {% if talk.link %}
      <summary><a href="{{ talk.link }}">Link to paper</a> </summary>
      {% endif %}
      {% if talk.link2 %}
      <summary><a href="{{ talk.link2 }}">Link to second paper</a> </summary>
      {% endif %}
      {% if talk.link3 %}
      <summary><a href="{{ talk.link3 }}">Link to third paper</a> </summary>
      {% endif %}
    {% endif %}
  </div>
  {% endif %}
  {% if talk.abstract %}
    <details>
    <summary>Abstract</summary>
    {{ talk.abstract }}
    
    

    {% if talk.bio %}
    <br><br>
    <strong>Bio: </strong> {{ talk.bio }}
    {% endif %}

    {% if talk.recording %}
      <br><br>
      <strong><a href="{{ talk.recording }}">Video Link</a></strong>
    {% elsif talk.livestream %}
      <br><br>
      <strong><a href="{{ talk.livestream }}">Livestream Link</a></strong>
    {% endif %}
    </details>
  {% endif %}
  </div>
  {% endfor %}
</div>
{% endfor %}

# About DeFOx

**Organisers:** <a href="https://sites.google.com/site/alvarocartea/home">Álvaro Cartea</a>, <a href="https://www.stats.ox.ac.uk/~cucuring/">Mihai Cucuringu</a>, <a href="https://www0.maths.ox.ac.uk/people/faycal.drissi">Fayçal Drissi</a>, <a href="https://www.maths.ox.ac.uk/people/deborah.miori">Deborah Miori</a>, <a href="https://www.maths.ox.ac.uk/people/marcello.monga">Marcello Monga</a>

**Join us**:
Participants can join to receive notifications about the seminar series, click <a href="mailto:mihai.cucuringu@stats.ox.ac.uk">here</a> to send a request.
