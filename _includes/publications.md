<h2 id="publications" style="margin: 2px 0px 4px;">Publications &amp; Preprints</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-content">
  <div class="title"><a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a></div>
  <div class="author">{{ link.authors }}</div>
  <div class="periodical"><em>{{ link.conference }}</em></div>
  <div class="links">
    {% if link.pdf %}
    <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">PDF</a>
    {% endif %}
    {% if link.code %}
    <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Code</a>
    {% endif %}
    {% if link.page %}
    <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Project Page</a>
    {% endif %}
    {% if link.bibtex %}
    <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">BibTeX</a>
    {% endif %}
    {% if link.notes %}
    <strong><i class="publication-note">{{ link.notes }}</i></strong>
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
