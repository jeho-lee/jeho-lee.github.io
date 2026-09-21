{% if include.group == "selected" %}
<div class="publications" id="publications">
  <h2 id="selected-publications">Selected Publications</h2>
  <p class="publication-note"><strong>*</strong> Co-first author</p>
  <ol class="bibliography">
    {% for publication in site.data.publications.main %}
      {% if publication.selected %}
        {% include publication-item.html paper=publication %}
      {% endif %}
    {% endfor %}
  </ol>
</div>
{% else %}
<div class="publications">
  <h2 id="publication-list">Publications</h2>
  <h3>Conference and Journal</h3>
  <ol class="bibliography">
    {% for publication in site.data.publications.main %}
      {% unless publication.selected %}
        {% include publication-item.html paper=publication %}
      {% endunless %}
    {% endfor %}
  </ol>
  <h3>Short Papers, Posters, &amp; Highlights</h3>
  <ol class="bibliography">
    {% for publication in site.data.publications_others.main %}
      {% include publication-item.html paper=publication %}
    {% endfor %}
  </ol>
</div>
{% endif %}
