---
title: Services
nav: services
permalink: /services/
---
<section class="post">
  <header class="major">
    <h1>What We Do</h1>
    <p>AfricaWired designs, builds and runs software for businesses across Africa —<br>
    from a single product idea through to production infrastructure and ongoing support.</p>
  </header>

  <div class="row">
    {% for service in site.data.services %}
    <div class="col-4 col-6-medium col-12-small service-box">
      <span class="icon-circle"><i class="fas {{ service.icon }}"></i></span>
      <h3>{{ service.title }}</h3>
      <p>{{ service.description }}</p>
    </div>
    {% endfor %}
  </div>
</section>

<section class="post">
  <header class="major">
    <h2>Have a project in mind?</h2>
    <p>Tell us what you're building — we'll help you scope it out.</p>
  </header>
  <ul class="actions special">
    <li><a href="mailto:{{ site.company.email }}" class="button large primary">Email {{ site.company.email }}</a></li>
    <li><a href="{{ site.company.website }}" target="_blank" rel="noopener" class="button large">Visit {{ site.company.website | remove: "https://" }}</a></li>
  </ul>
</section>
