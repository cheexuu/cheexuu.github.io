<h2 id="publications" style="margin: 2px 0px -15px;">Qualifications</h2>

<div class="publications">
<ol class="bibliography">


{% for link in site.data.qualifications.main %}
<li>
  <div class="pub-row">
    {% if link.image %} 
    <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
      {% if link.image %} 
      <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
        {% if link.conference_short %} 
        <abbr class="badge">{{ link.conference_short }}</abbr>
        {% endif %}
      {% endif %}
    </div>
    {% endif %}
      <div >
        <ul style="list-style-type: disc; text-align: justify;">
            <li>{{ link.title }}</li>
        </ul>
      </div>
  </div>
</li>

{% endfor %}


</ol>
</div>
