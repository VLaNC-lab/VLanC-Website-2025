---
title: Course
layout: default
nav:
  order: 2
  tooltip: Courses Taught
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research" ]
---



<h1 style="text-align: center; font-weight: bold;">{% include icon.html icon="fa-solid fa-book" %} Courses Offered</h1>

The **VLANC** Lab is actively involved in teaching and mentoring students through a variety of cutting-edge courses offered at both undergraduate and graduate levels. So that the students are ready to work on cutting-edge technology for the betterment of mankind.




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
  {% include tags_button.html tags="Faculty, Schedule, Readings,Books,Projects, Conferences" link="course/fall-2025" %}
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
  {% include tags_button.html tags="Faculty,Schedule,Readings,Books,Projects,Conferences" link="course/fall-2024" %}
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
  {% include tags_button.html tags="Faculty, Schedule, Readings,Books,Projects, Conferences" link="course/spring-2024" %}
  {% endif %}
{% endfor %}















