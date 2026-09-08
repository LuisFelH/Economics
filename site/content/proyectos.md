<div class="section-heading">
  <div>
    <p class="eyebrow">Applied projetcs</p>
    <h2>Consolidate analysis</h2>
    <p>All projects follow the same structure: research question, data status, main results, methodology, interpretation, and limitations.</p>
  </div>
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
<div class="panel" style="text-align:center; padding:3rem 2rem; margin-top:3rem; margin-bottom:2rem;">
  <p class="eyebrow">In preparation</p>
  <h2>Projects coming soon</h2>
  <p>I am currently developing research projects in empirical macroeconomics and macroeconometrics. Detailed project pages, replication materials, code, data documentation, and research outputs will be added here as they become available.</p>
  <div class="actions" style="justify-content:center;"><a class="button button-primary" href="https://github.com/LuisFelH" target="_blank" rel="noopener">Visit my GitHub</a></div>
</div>



<div class="section" style="padding-bottom:0">
  <div class="two-col">
    <div class="panel">
      <p class="eyebrow">Editorial criteria</p>
      <h2>What does the publication of a project imply?</h2>
      <p>This page does not execute maodels in real life. It processed outputs and validated this avoid that a fail when download, a R dependence or a methodolical review can crash the website.
      La página pública no ejecuta modelos en tiempo real. Consume salidas procesadas y validadas por cada pipeline. Esto evita que una falla de descarga, una dependencia de R o una revisión metodológica rompa el sitio completo.</p>
      <p>Los resultados se muestran con fecha de corte, estado y advertencias específicas. Cuando un insumo no está disponible, la salida correspondiente no se publica como si existiera.</p>
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
