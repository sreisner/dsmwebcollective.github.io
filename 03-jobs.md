---
layout: list
title: Jobs in Des Moines
nav_title: Jobs
permalink: /jobs/
---

<div class="list list-animate jobs-list">
    {% if site.data.jobs %}
        {% for job in site.data.jobs %}
            <a href="{{ job.url }}" target="_blank">
                <div class="title">
                    {{ job.title }}
                </div>

                <div class="group">{{ job.company }}</div>
            </a>
        {% endfor %}

        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">Have a job posting to add?</a>
    {% else %}
        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">No job postings at this time. Have a job posting to add?</a>
    {% endif %}
</div>
