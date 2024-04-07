---
layout: default
title: Nick Cunningham - Archive
subtitle: Archive
description:
---

<div class="container">
  <div class="page-head">
    <h1 class="page-title">{% if page.subtitle %}{{ page.subtitle }}{% else %}{{ site.data.settings.projects__settings.projects__title }}{% endif %}</h1>
    {% if page.description %}
      <p class="page-description">{{ page.description }}</p>
    {% else site.data.settings.projects__settings.projects__description %}
      <p class="page-description">{{ site.data.settings.projects__settings.projects__description }}</p>
    {% endif %}
  </div>
</div>

<!-- <div style="text-align:center; font-family: $heading-font-family;
  font-size: 40px;">
    This page is currently under construction.
</div> -->

<div class="container animate">
  <article class="page">
    <div class="page__content">
      I have worked on a lot of stuff over the years. Unfortunately, not all of it makes the cut for my main portfolio. Here you can find my “other work.” This is where my former portfolio pieces, unrefined prototypes, game jams, older work and miscellaneous projects live.
    </div>
  </article>
</div>

<div class="projects-page container animate">
  <div class="row">
    {% for project in site.archive %}
      <article class="project col col-4 col-d-6 col-t-12">
        <div class="project__content">
          <a href="{{ project.url | prepend:site.baseurl }}" class="project__image">
            <img class="lazy" data-src="{{ project.image | prepend:site.baseurl }}" alt="{{ project.title }}">
          </a>
          <div class="project__info">
            <h3 class="project__title"><a href="{{ project.url | prepend:site.baseurl }}">{{ project.title }}</a></h3>
            {% if project.subtitle %}
            <div class="project__subtitle">{{ project.subtitle }}</div>
            {% endif %}
          </div>
        </div>
      </article>
    {% endfor %}
  </div>
</div>