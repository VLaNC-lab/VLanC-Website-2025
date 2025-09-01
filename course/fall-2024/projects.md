---
layout: default
title: Projects
permalink: /course/fall-2024/projects/
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester.Students Project in Foundations of NLP, NLP - Fall 2024" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research", "Conferences", "NLP - Fall 2024", "Recommended Conference","Publishing","Students Projects","Students Works"]
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

/* Light/dark mode support */
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
  text-align: left;
  border: 1px solid var(--border-color);
}

.github-icon {
  width: 24px;
  height: 24px;
  vertical-align: middle;
  filter: invert(0); /* default for light mode */
}

@media (prefers-color-scheme: dark) {
  .github-icon {
    filter: invert(1); /* inverts color to white in dark mode */
  }
}

.projects-table a {
  display: inline-block;
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
  }
  .projects-table td {
    text-align: right;
    padding-left: 50%;
    position: relative;
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
</style>

<div class="page-container">
  <h2>🚀 Final Project Showcase – Spring 2024</h2>
  <table class="projects-table">
    <thead>
      <tr>
        <th>Team No.</th>
        <th>Title</th>
        <th>GitHub</th>
      </tr>
    </thead>
    <tbody>
      {% for project in site.data.fall-project.fall-2024 %}
      <tr>
        <td data-label="Team No.">{{ project.team_no }}</td>
        <td data-label="Title">{{ project.title }}</td>
        <td data-label="GitHub">
          {% if project.github and project.github != "" %}
            <a href="{{ project.github }}" target="_blank" title="View on GitHub">
              <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" class="github-icon" />
            </a>
          {% else %}
            <span style="opacity: 0.6;">N/A</span>
          {% endif %}
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>
