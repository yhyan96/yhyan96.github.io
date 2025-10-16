<h2 id="publications" style="margin: 2px 0px -15px;">Publications <span style="font-size: 0.6em; color: #666;">(<u>Co-author</u>, *Corresponding Author)</span></h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;margin-bottom: 8px;">
      <div class="title" style="color: #086bcfff,font-weight: bold;">{{ link.title }}</div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
  </div>
</div>

{% endfor %}

</ol>
</div>
