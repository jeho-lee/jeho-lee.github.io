<h2 id="publications" style="margin: 2px 0px -25px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

<p style="font-size: 0.95rem;"><strong>*</strong> Co-first author</p>

<h4 style="margin: -10px 0px 6px;">Conference and Journal</h4>

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <!-- <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div> -->
  <!-- <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;"> -->
  <div class="col-sm-9" style="position: relative;">
    <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
    <div class="author" style="font-size:0.95rem;">{{ link.authors }}</div>
    <div class="periodical" style="font-size:0.95rem;"><em>{{ link.conference }}</em></div>
    <div class="links">
      <!-- {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %} -->
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong style="color:#e74d3c">{{ link.notes }}</strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<!-- <br> -->

{% endfor %}



<h4 style="margin:2px 0px 6px;">Other Publications</h4>

{% for link in site.data.publications_others.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;">
    <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
    <div class="author" style="font-size:0.95rem;">{{ link.authors }}</div>
    <div class="periodical" style="font-size:0.95rem;"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>

