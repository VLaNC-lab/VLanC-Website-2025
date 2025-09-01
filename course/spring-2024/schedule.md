---
layout: default
title: schedule
permalink: /course/spring-2024/schedule/
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester.Schedule of Foundations of NLP, NLP - Spring 2024" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research", "Readings", "NLP - Spring 2024", "Office Hours","Class Schedule"]
---
<style>
.page-container {
  display: flex;
  flex-direction: column;
  justify-content: center;  /* vertical center */
  align-items: center;      /* horizontal center */
  padding: 2rem;
  box-sizing: border-box;
  text-align: center;
}

/* Limit width and style course info box */
.course-info {
  max-width: 800px;
  background-color: #f9f9f9;
  border-left: 4px solid #007acc;
  padding: 1rem;
  border-radius: 6px;
  margin-bottom: 0.5rem;
  color: #222;
}

/* Dark mode support */
@media (prefers-color-scheme: dark) {
  .course-info {
    background-color: #1e1e1e;
    border-left-color: #66ccff;
    color: #f0f0f0;
  }
}

/* Reduce margin above and below headings */
h1, h2, h3, h4, h5, h6 {
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}

/* Center the faculty portraits container */
.portrait-list {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 800px;
  gap: 1rem; /* Adjust gap between portraits */
}


.projects-table {
    width: 100%;
    border-collapse: collapse;
    margin-bottom: 2rem;
    font-family: "Segoe UI", sans-serif;
    font-size: 15px;
  }

  .projects-table th,
  .projects-table td {
    border: 1px solid #ddd;
    padding: 12px;
    text-align: left;
    vertical-align: top;
  }

  .projects-table th {
    background-color: #f5f5f5;
    font-weight: bold;
    color: #333;
  }

  .projects-table td ul {
    margin: 0;
    padding-left: 1.2rem;
  }

  .projects-table td li {
    margin-bottom: 4px;
  }

  .projects-table a {
    color: #007acc;
    text-decoration: none;
  }

  .projects-table a:hover {
    text-decoration: underline;
  }

  .projects-table .na {
    color: #888;
    font-style: italic;
  }

  @media (max-width: 768px) {
    .projects-table thead {
      display: none;
    }

    .projects-table tr {
      display: block;
      margin-bottom: 15px;
      border-bottom: 2px solid #ccc;
    }

    .projects-table td {
      display: block;
      text-align: right;
      padding-left: 50%;
      position: relative;
    }

    .projects-table td::before {
      content: attr(data-label);
      position: absolute;
      left: 12px;
      top: 12px;
      font-weight: bold;
      color: #555;
      text-align: left;
    }
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
  <table class="projects-table">
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
          <ul>
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
          <ul>
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
          <ul>
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
