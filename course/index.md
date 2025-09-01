---
title: Course
layout: default
nav:
  order: 2
  tooltip: Courses Taught
---

# {% include icon.html icon="fa-solid fa-book" %} Courses

The **VLANC** Lab is actively involved in teaching and mentoring students through a variety of cutting-edge courses offered at both undergraduate and graduate levels. So that the students are ready to work on cutting-edge technology for the betterment of mankind.



{% include search-box.html %}
{% include search-info.html %}
{% include section.html %}

{% for course in site.data.fall-2025.fall-2025 %}

{% if course.category == "course" %}

  {% assign flip_value = forloop.index0 | modulo: 2 %}
  {% if flip_value == 1 %}
    {% assign flip_flag = true %}
  {% else %}
    {% assign flip_flag = false %}
  {% endif %}
  {% include feature.html
    image=course.image_course
    link=course.link
    title=course.title
    text=course.text
    tags=course.tags
    flip=flip_flag
  %}
  {% include tags.html tags="Faculty, Schedule, Readings,Books,Projects, Conferences" link="course/fall-2025" %}
  {% endif %}
{% endfor %}


{% for course in site.data.ITC-Spring-2025.Spring-2025 %}

{% if course.category == "course" %}

  {% assign flip_value = forloop.index0 | modulo: 2 %}
  {% if flip_value == 0 %}
    {% assign flip_flag = true %}
  {% else %}
    {% assign flip_flag = false %}
  {% endif %}
  {% include feature.html
    image=course.image_course
    link=course.link
    title=course.title
    text=course.text
    tags=course.tags
    flip=flip_flag
  %}
  {% endif %}
{% endfor %}


{% for course in site.data.ITC-Fall-2024.Fall-2024 %}
{% if course.category == "course" %}

  {% assign flip_value = forloop.index0 | modulo: 2 %}
  {% if flip_value == 1 %}
    {% assign flip_flag = true %}
  {% else %}
    {% assign flip_flag = false %}
  {% endif %}
  {% include feature.html
    image=course.image_course
    link=course.link
    title=course.title
    text=course.text
    tags=course.tags
    flip=flip_flag
  %}
  {% endif %}
{% endfor %}




{% for course in site.data.fall-2024.fNLP-fall-2024 %}

{% if course.category == "course" %}

  {% assign flip_value = forloop.index0 | modulo: 2 %}
  {% if flip_value == 0 %}
    {% assign flip_flag = true %}
  {% else %}
    {% assign flip_flag = false %}
  {% endif %}
  {% include feature.html
    image=course.image_course
    link=course.link
    title=course.title
    text=course.text
    tags=course.tags
    flip=flip_flag
  %}
  {% include tags.html tags="Faculty,Schedule,Readings,Books,Projects,Conferences" link="course/fall-2024" %}
  {% endif %}
{% endfor %}



{% for course in site.data.spring-2024 %}
{% if course.category == "course" %}

  {% assign flip_value = forloop.index0 | modulo: 2 %}
  {% if flip_value == 1 %}
    {% assign flip_flag = true %}
  {% else %}
    {% assign flip_flag = false %}
  {% endif %}
  {% include feature.html
    image=course.image_course
    link=course.link
    title=course.title
    text=course.text
    tags=course.tags
    flip=flip_flag
  %}
  {% include tags.html tags="Faculty, Schedule, Readings,Books,Projects, Conferences" link="course/spring-2024" %}
  {% endif %}
{% endfor %}















