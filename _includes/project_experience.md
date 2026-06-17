<h2 id="publications" style="margin: 2px 0px -15px;">Project Experience</h2>

<div class="publications">
<ol class="bibliography">


{% for link in site.data.project_experience.main %}
<h4 style="margin: 0px 10px 0px;">{{ link.time }}</h4>
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
    <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
        <div class="title">
          <span class = "project_name">
              {{ link.project_name }}
          </span>
        </div>
        <div >
          <ul style="list-style-type: disc; text-align: justify;">
            {% for key in link.key_points %}
                <li>{{ key }}</li>
            {% endfor %}
          </ul>
        </div>
      <!-- <div class="links">
        {% if link.pdf %} 
        <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        {% endif %}
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
        <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %} 
        {{ link.others }}
        {% endif %}
      </div> -->
    </div>
  </div>
</li>
<!-- <br> -->

{% endfor %}


</ol>
</div>
