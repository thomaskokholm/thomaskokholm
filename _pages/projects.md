---
layout: projects
title: Projects & Cases
permalink: /projects/
published: true
---


<div class="row">
    {% for project in site.data.projects %}
    <div class="col-md-6">
        <h2>{{ project.title }}</h2>
        <img src="{{ project.thumbnail }}" />
        <p>
            <small>Date: {{ project.date }}</small>
            <br />
            <small>Tagged:
            {% for tag in project.tags %}
            <i>{{ tag }}</i>
            {% endfor %}
            </small>
        </p>
        <p>{{ project.short_info}}</p>
    </div>
    {% endfor %}
</div>
