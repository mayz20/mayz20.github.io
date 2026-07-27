<h2 id="publications">Publications &amp; Preprints</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li class="publication-item">
<div class="pub-content">
  <div class="pub-heading">
    {% if link.conference_short %}
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a></div>
  </div>
  <div class="author">{{ link.authors }}</div>
  <div class="publication-meta">
    <span class="periodical">{{ link.conference }}</span>
    <span class="links">
    {% if link.pdf %}
    <a href="{{ link.pdf }}" target="_blank" rel="noopener">PDF</a>
    {% endif %}
    {% if link.code %}
    <a href="{{ link.code }}" target="_blank" rel="noopener">Code</a>
    {% endif %}
    {% if link.page %}
    <a href="{{ link.page }}" target="_blank" rel="noopener">Project Page</a>
    {% endif %}
    {% if link.bibtex %}
    <a href="{{ link.bibtex }}" target="_blank" rel="noopener">BibTeX</a>
    {% endif %}
    </span>
    {% if link.notes %}
    <strong class="publication-note">{{ link.notes }}</strong>
    {% endif %}
    {% if link.others %}
    {{ link.others }}
    {% endif %}
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>
<p class="publication-legend">* Equal contribution. # Corresponding author.</p>
