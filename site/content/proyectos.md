<div class="section-heading">
  <div>
    <p class="eyebrow">Applied projetcs</p>
    <h2>Consolidate analysis</h2>
    <p>This section will collect my applied research projects in macroeconomics and econometrics. Each project will document its research question, data, methodology, results, interpretation, and limitations.</p>
  </div>
</div>




<div class="panel" style="text-align:center; padding:3rem 2rem; margin-top:3rem; margin-bottom:2rem;">
  <p class="eyebrow">In preparation</p>
  <h2>Projects coming soon</h2>
  <p>I am currently developing research projects in empirical macroeconomics and macroeconometrics. Detailed project pages, replication materials, code, data documentation, and research outputs will be added here as they become available.</p>
  <div class="actions" style="justify-content:center;"><a class="button button-primary" href="https://github.com/LuisFelH" target="_blank" rel="noopener">Visit my GitHub</a></div>
</div>



<div class="card-grid">
{% for p in projects %}
<article class="project-card">
  <a class="card-image" href="proyectos/{{ p.slug }}.html"><img src="{{ p.image }}" alt="Vista previa de {{ p.short_title }}" loading="lazy"></a>
  <div class="card-body">
    <div class="card-kicker">{{ p.category }}</div>
    <h3 class="card-title"><a href="proyectos/{{ p.slug }}.html">{{ p.title }}</a></h3>
    <p class="card-description">{{ p.description }}</p>
    <div class="tag-row">{% for tag in p.tags %}<span class="tag">{{ tag }}</span>{% endfor %}</div>
    <div class="card-footer"><a class="card-link" href="proyectos/{{ p.slug }}.html">Abrir proyecto →</a><span class="status {% if p.status_class == 'note' %}status-note{% endif %}">{{ p.status }}</span></div>
        <p class="card-description">{{ p.description }}</p>
    <div class="tag-row">{% for tag in p.tags %}<span class="tag">{{ tag }}</span>{% endfor %}</div>
    <div class="card-footer"><a class="card-link" href="proyectos/{{ p.slug }}.html">Abrir proyecto →</a><span class="status {% if p.status_class == 'note' %}status-note{% endif %}">{{ p.status }}</span></div>
  </div>
</article>
{% endfor %}

</div>
<div class="section" style="padding-bottom:0">

  <div class="two-col">
    <div class="panel">
      <p class="eyebrow">Editorial criteria</p>
      <h2>How projects will be presented</h2>
      <p>Each public project will provide a transparent account of its motivation, data sources, empirical strategy, main findings, and limitations. Where possible, I will include reproducible code, documentation, and links to research outputs.

Published pages will use validated, pre-processed outputs rather than run models in real time. This makes the portfolio more reliable and preserves a clear separation between research pipelines and public presentation.

Projects related to other research fields will be also published here. The research agenda reflects my main interests.</p>
    </div>
    <div class="panel">
      <p class="eyebrow">Research agenda</p>
      <ul class="clean-list">
        <li><strong>Política monetaria y fluctuaciones cambiarias</strong><br><span class="muted">Extensión de la tesis de Magíster a reglas de reacción, shocks externos y bienestar.</span></li>
        <li><strong>Transmisión heterogénea de tasas</strong><br><span class="muted">Diferencias por producto, fase del ciclo y condiciones financieras.</span></li>
        <li><strong>Infraestructura digital y comercio de servicios</strong><br><span class="muted">Latencia, conectividad internacional, regulación y exportaciones.</span></li>
      </ul>
    </div>
  </div>
</div>
