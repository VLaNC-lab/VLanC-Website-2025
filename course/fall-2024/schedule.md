---
layout: default
title: Schedule
permalink: /course/fall-2024/schedule/
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester.Schedule of Foundations of NLP, NLP - Fall 2024" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research", "Readings", "NLP - Fall 2024", "Office Hours","Class Schedule"]
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

/* Remove default list styles, center text */
.course-info ul {
  list-style: none;
  padding: 0;
  margin: 0 auto;
  text-align: center;
  max-width: 400px;
}

.course-info li {
  margin-bottom: 0.5rem;
  line-height: 1.6;
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
</style>

<div class="page-container">

{% assign course = site.data.fNLP-fall-2024 | where: "title", "CS3126" | first %}

{% if course %}
<h1>📘 Course Code: {{ course.title }}</h1>

<div class="course-info">
  {{ course.course_info }}
</div>
{% else %}
<p>⚠️ Course information not found for CS3126.</p>
{% endif %}

</div>



