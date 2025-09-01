---
layout: default
title: Readings
permalink: /course/fall-2024/readings/
description: "Visual LAnguage Neural Cognitive Computing (VLANC) Lab at Mahindra University integrates AI, Vision, Language, and Neural Computation for multimodal understanding, Knowledge Graphs, GNNs, and Brain-computer Interfaces. Several Courses are offered by Dr. Nidhi Goyal on Natural Language Processing (NLP), Foundation of Natural Language Processing (NLP) and Introduction to Computing (ITC) for Fall and Spring Semester.Recommended Readings in Foundations of NLP, NLP - Fall 2024" 
keywords: [ "VLANC", Visual Language Neural Cognitive Computing Lab,"Visual Language", "Neural Cognitive Computing", "VLANC Lab", "AI Research", "Knowledge Graph", "Graph Neural Networks", "Multimodal AI", "Brain-Computer Interfaces", "Deep Generative Models", "Natural Language Processing", "Vision-Language Integration","NLP", "AI", "AI and Neuroscience lab", "Mahindra University AI lab", "Nidhi Goyal", "Dr. Nidhi Goyal","Projects","Finding","Courses","Research", "Readings", "NLP - Fall 2024", "Recommended Readings","Books"]
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
  .github-icon {
    filter: invert(1);
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
  .github-icon {
    filter: invert(0);
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
}

.projects-table a {
  display: inline-block;
}

/* Responsive table for small screens */
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

/* Containers for lists */
.list-container {
  max-width: 700px;
  margin: 2rem auto 3rem auto;
  padding: 1rem 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.08);
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  text-align: left;
}

.journals {
  background-color: #f0f8ff;
  border: 1px solid #a9cce3;
  color: #154360;
}

.conferences {
  background-color: #e8f5e9;
  border: 1px solid #81c784;
  color: #2e7d32;
}

.list-container ul {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.list-container ul li {
  padding: 0.4rem 0;
  position: relative;
  font-size: 1.05rem;
}

/* Checkmark bullets for journals */
.journals ul li::before {
  content: "✓";
  color: #2e86c1;
  font-weight: bold;
  position: absolute;
  left: -1.5rem;
}

/* Arrow bullets for conferences */
.conferences ul li::before {
  content: "➤";
  color: #388e3c;
  font-weight: bold;
  position: absolute;
  left: -1.5rem;
}

/* Responsive tweaks */
@media (max-width: 768px) {
  .list-container {
    margin: 1rem 1rem 2rem 1rem;
    padding: 1rem;
  }
}

.list-row {
  display: flex;
  justify-content: center;
  gap: 3rem; /* space between the two boxes */
  flex-wrap: wrap; /* wrap on small screens */
  max-width: 1200px;
  margin: 2rem auto 3rem auto;
  padding: 0 1rem;
}

.list-container {
  flex: 1 1 400px; /* grow, shrink, basis width */
  padding: 1rem 1.5rem;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.08);
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  text-align: left;
}

.journals {
  background-color: #f0f8ff;
  border: 1px solid #a9cce3;
  color: #154360;
}

.conferences {
  background-color: #e8f5e9;
  border: 1px solid #81c784;
  color: #2e7d32;
}

.list-container ul {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.list-container ul li {
  padding: 0.4rem 0;
  position: relative;
  font-size: 1.05rem;
}

/* Checkmark bullets for journals */
.journals ul li::before {
  content: "✓";
  color: #2e86c1;
  font-weight: bold;
  position: absolute;
  left: -1.5rem;
}

/* Arrow bullets for conferences */
.conferences ul li::before {
  content: "➤";
  color: #388e3c;
  font-weight: bold;
  position: absolute;
  left: -1.5rem;
}

/* Responsive tweak: stack vertically on narrow screens */
@media (max-width: 768px) {
  .list-row {
    flex-direction: column;
    margin: 1rem;
    padding: 0;
  }
  .list-container {
    flex-basis: 100%;
    margin-bottom: 1.5rem;
  }
}


</style>

<div class="page-container">
  <h2>📚 Fall 2024 Readings – Natural Language Processing</h2>
  <p>The following texts are useful, but none are required. All of them can be read free online.</p>
  <table class="projects-table">
    <thead>
      <tr>
        <th>Title</th>
        <th>Authors</th>
        <th>Link</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Speech and Language Processing</td>
        <td>Dan Jurafsky and James H. Martin</td>
        <td><a href="https://web.stanford.edu/~jurafsky/slp3/" target="_blank">View</a></td>
      </tr>
      <tr>
        <td>Natural Language Processing</td>
        <td>Jacob Eisenstein</td>
        <td><a href="https://github.com/jacobeisenstein/nlp" target="_blank">View</a></td>
      </tr>
      <tr>
        <td>A Primer on Neural Network Models for Natural Language Processing</td>
        <td>Yoav Goldberg</td>
        <td><a href="https://u.cs.biu.ac.il/~yogo/NN4NLP/" target="_blank">View</a></td>
      </tr>
      <tr>
        <td>Natural Language Processing With PyTorch</td>
        <td>Delip Rao and Brian McMahan</td>
        <td><a href="https://www.oreilly.com/library/view/natural-language-processing/9781098103248/" target="_blank">View</a></td>
      </tr>
      <tr>
        <td>Natural Language Processing with Transformers</td>
        <td>Lewis Tunstall, Leandro von Werra, and Thomas Wolf</td>
        <td><a href="https://transformersbook.com/" target="_blank">View</a></td>
      </tr>
    </tbody>
  </table>



</div>
