---
layout: project
title: Projects & Cases
permalink: /projects/
published: true
---

<div class="row">
    {% for item in site.cases %}
    <div class="col-md-6">
        <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
        <a href="{{ item.url }}">
            <img src="{{ item.thumbnail }}" />
        </a>
        <p>
        <small>
        {% for tag in item.tags %}
            {% capture tag_name %}{{ tag }}{% endcapture %}
                <a href="/tag/{{ tag_name }}" class="badge badge-light">
                {{ tag_name }}
                </a>
        {% endfor %}
        </small>
        </p>
        <p>
            <small>Date: {{ item.date }}</small>
            <br />
            <small>Tagged:
            {% for tag in item.tags %}
            <i>{{ tag }}</i>
            {% endfor %}
            </small>
        </p>
        <p><a href="{{ item.url }}">{{ item.description}}</a></p>
    </div>
    {% endfor %}
</div>
