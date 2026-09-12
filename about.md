---
title: About Us
nav: about
permalink: /about/
---
<section class="post">
  <header class="major">
    <h1>About AfricaWired</h1>
    <p>A software engineering company based in {{ site.company.address_line }}, {{ site.company.country }} —<br>
    building the systems that run businesses across Africa.</p>
  </header>

  <p>AfricaWired designs, develops and operates software for engineering, construction and project-driven businesses, as well as custom applications for clients across other industries. We work across the full stack of a modern technology company: software engineering, systems architecture, cloud infrastructure, cybersecurity, UI/UX design, data &amp; AI, and the consulting and training that goes with it.</p>
  <p>Our approach is to own outcomes, not just deliverables — every system we ship is designed cloud-native, secured by default, and built to be maintained long after launch, not handed off and forgotten.</p>
</section>

<section class="post">
  <header class="major">
    <h2>Founding Team</h2>
  </header>
  <div class="row">
    {% for member in site.data.team %}
    <div class="col-6 col-12-small team-box">
      <span class="avatar-circle">{{ member.initials }}</span>
      <h3>{{ member.name }}</h3>
      <p>{{ member.role }}</p>
    </div>
    {% endfor %}
  </div>
</section>

<section class="post">
  <header class="major">
    <h2>Why This Blog Exists</h2>
    <p>This is where our engineering team shares what we're building, the technical decisions behind it, and lessons learned running production systems for our clients — grounded in real project work, not theory.</p>
  </header>
  <ul class="actions special">
    <li><a href="{{ '/blog/' | relative_url }}" class="button large primary">Read the Blog</a></li>
    <li><a href="{{ '/services/' | relative_url }}" class="button large">Explore Our Services</a></li>
  </ul>
</section>
