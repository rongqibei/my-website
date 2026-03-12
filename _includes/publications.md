<h1 id="publications"></h1>

<h2 style="margin: 40px 0px -15px;">Selected Research in AI and Digital Health</h2>

<div class="publications" style="margin-top:2.2rem;">
<ol class="bibliography">

{% for pub in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ pub.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if pub.conference_short and pub.conference_short != "" %}
    <abbr class="badge">{{ pub.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
    <div class="title">
      {{ pub.title }}
      {% if pub.link %}
      <a href="{{ pub.link }}" target="_blank" rel="noopener noreferrer" class="pub-link-btn">Link</a>
      {% endif %}
    </div>
    <div class="author">{{ pub.authors }}</div>
    <div class="periodical"><em>{{ pub.conference }}</em></div>
    <div class="links">
      {% if pub.notes %}
      <strong><i style="color:#e74d3c; font-weight:600">{{ pub.notes }}</i></strong>
      {% endif %}
      {% if pub.tags %}
      <div class="pub-tags">
        {% for tag in pub.tags %}
        <span class="pub-tag">{{ tag }}</span>
        {% endfor %}
      </div>
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>

<div style="text-align:right; margin-top:-15px;">
  <a href="https://scholar.google.com/citations?user=qelg1bcAAAAJ" target="_blank" rel="noopener noreferrer" class="pub-link-btn">View all publications →</a>
</div>


