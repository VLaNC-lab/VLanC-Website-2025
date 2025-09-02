---
layout: default
title: schedule
permalink: /course/spring-2024/schedule/
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester.Schedule of Foundations of NLP, NLP - Spring 2024" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research", "Readings", "NLP - Spring 2024", "Office Hours","Class Schedule"]
---
<style>
:root {
  --text-color-light: #2c3e50;
  --text-color-dark: #ecf0f1;
  --bg-color-light: #ffffff;
  --bg-color-dark: #1e1e1e;
  --header-bg-light: #34495e;
  --header-bg-dark: #2c3e50;
  --hover-light: #f1f1f1;
  --hover-dark: #2a2a2a;
  --border-color: #ccc;
}
<style>
:root {
  --text-color-light: #2c3e50;
  --text-color-dark: #ecf0f1;
  --bg-color-light: #ffffff;
  --bg-color-dark: #1e1e1e;
  --header-bg-light: #34495e;
  --header-bg-dark: #2c3e50;
  --hover-light: #f1f1f1;
  --hover-dark: #2a2a2a;
  --border-color: #ccc;
}

@media (prefers-color-scheme: dark) {
  body {
    background-color: var(--bg-color-dark);
    color: var(--text-color-dark);
  }
  .projects-table {
    background-color: var(--bg-color-dark);
    color: var(--text-color-dark);
  }
  .projects-table thead {
    background-color: var(--header-bg-dark);
  }
  .projects-table tbody tr:hover {
    background-color: var(--hover-dark);
  }
  a.hover{
  color: white;       
  }
}

@media (prefers-color-scheme: light) {
  body {
    background-color: var(--bg-color-light);
    color: var(--text-color-light);
  }
  .projects-table {
    background-color: var(--bg-color-light);
    color: var(--text-color-light);
  }
  .projects-table thead {
    background-color: var(--header-bg-light);
    color: white;
  }
  
  .projects-table tbody tr:hover {
    background-color: var(--hover-light);
  }
   a.hover{
  color: white;       
  }
}

.page-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  box-sizing: border-box;
  text-align: center;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}

h2 {
  margin-bottom: 1rem;
  font-size: 2rem;
}

.projects-table {
  width: 100%;
  max-width: 1100px;
  border-collapse: collapse;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.projects-table th, .projects-table td {
  padding: 1rem;
  text-align: center;
  border: 1px solid var(--border-color);
}

.github-icon {
  width: 24px;
  height: 24px;
  vertical-align: middle;
  filter: invert(0);
}

@media (prefers-color-scheme: dark) {
  .github-icon {
    filter: invert(1);
  }
}

.projects-table a {
  display: inline-block;
  text-align: center;
}

.projects-table td {
  text-align: center; /* center content inside table cells */
}

@media (max-width: 768px) {
  .projects-table thead {
    display: none;
  }
  .projects-table, .projects-table tbody, .projects-table tr, .projects-table td {
    display: block;
    width: 100%;
  }
  .projects-table tr {
    margin-bottom: 1rem;
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 1rem;
    text-align: center;
  }
  .projects-table td {
    text-align: center;
    padding-left: 50%;
    position: relative;
  }
  .projects-table th {
    text-align: center;
  }
  .projects-table td::before {
    content: attr(data-label);
    position: absolute;
    left: 1rem;
    width: 45%;
    font-weight: bold;
    text-align: left;
  }
}

.pagination {
  margin-top: 10px;
  text-align: center;
}
.pagination button {
  padding: 0px 0px;
  margin: 0px;
}
.pagination span {
  font-weight: bold;
  margin: 0 8px;
}
</style>



<div class="page-container">

{% assign course = site.data.spring-2024 | where: "title", "CS3126" | first %}

{% if course %}
<h1>📘 Course Info: {{ course.title }}</h1>

<div class="course-info">
  {{ course.course_info }}
</div>
{% else %}
<p>⚠️ Course information not found for CS3126.</p>
{% endif %}


{% include section.html %}
  <details markdown="1">
<summary>Full Class Schedule</summary>
  

<div class="page-container">
  <h2>📘 NLP Course Weekly Schedule – Spring 2024</h2>
  <table class="projects-table" id="projectTable">
  <thead>
    <tr>
      <th>Week</th>
      <th>Topic</th>
      <th>Lecture Slides</th>
      <th>Assignments</th>
      <th>Readings</th>
    </tr>
  </thead>
  <tbody>
    {% for week in site.data.spring-project.spring_lecture_schedule %}
    <tr>
      <td data-label="Week">{{ week.week }}</td>
      <td data-label="Topic">{{ week.topic }}</td>

      <td data-label="Lecture Slides">
        {% if week.lecture_slides and week.lecture_slides.size > 0 %}
          <ul style="list-style-type: none; padding-left: 0; margin: 0;">
            {% for slide in week.lecture_slides %}
              <li><a href="{{ slide }}" target="_blank">Slides {{ forloop.index }}</a></li>
            {% endfor %}
          </ul>
        {% else %}
          <span style="opacity: 0.6;">N/A</span>
        {% endif %}
      </td>

      <td data-label="Assignments">
        {% if week.assignments and week.assignments.size > 0 %}
          <ul style="list-style-type: none; padding-left: 0; margin: 0;">
            {% for assign in week.assignments %}
              <li>{{ assign }}</li>
            {% endfor %}
          </ul>
        {% else %}
          <span style="opacity: 0.6;">N/A</span>
        {% endif %}
      </td>

      <td data-label="Readings">
        {% if week.readings and week.readings.size > 0 %}
          <ul style="list-style-type: none; padding-left: 0; margin: 0;">
            {% for read in week.readings %}
              <li><a href="{{ read.url }}" target="_blank">{{ read.title }}</a></li>
            {% endfor %}
          </ul>
        {% else %}
          <span style="opacity: 0.6;">N/A</span>
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
</div>
</details>
</div>
