---
layout: default
title: Readings
permalink: /course/spring-2024/conferences/
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
  .list-container {
    background-color: var(--bg-color-dark);
    color: var(--text-color-dark);
    border-color: #444;
  }
}

@media (prefers-color-scheme: light) {
  body {
    background-color: var(--bg-color-light);
    color: var(--text-color-light);
  }
  .list-container {
    background-color: var(--bg-color-light);
    color: var(--text-color-light);
    border-color: var(--border-color);
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

.list-row {
  display: flex;
  justify-content: center;
  gap: 3rem;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 2rem auto 3rem auto;
  padding: 0 1rem;
}

.list-container {
  flex: 1 1 400px;
  padding: 1.5rem 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.08);
  border: 1px solid var(--border-color);
  text-align: left;
  transition: background-color 0.3s ease;
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

h3 {
  font-size: 1.4rem;
  margin-bottom: 1rem;
}

.badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;
  margin-top: 1rem;
}

.badge {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 0.4rem 0.8rem;
  border-radius: 1rem;
  border: 1px solid #ccc;
  font-size: 0.95rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.05);
  transition: transform 0.2s ease, background-color 0.2s ease;
}

.journals .badge {
  background-color: #eaf4fc;
  border-color: #aed6f1;
  color: #154360;
}

.conferences .badge {
  background-color: #e8f5e9;
  border-color: #81c784;
  color: #2e7d32;
}

.badge:hover {
  transform: scale(1.05);
  background-color: #f4f4f4;
  cursor: default;
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
  <h2>📚 Spring 2024 Conferences – Natural Language Processing</h2>

  <div class="list-row">
    <div class="list-container journals">
      <h3>📖 Journals</h3>
      <div class="badges">
        <span class="badge">Journal of Computational Linguistics</span>
        <span class="badge">Transactions of the ACL</span>
        <span class="badge">Journal of Information Retrieval</span>
        <span class="badge">Journal of Machine Learning</span>
      </div>
    </div>

    <div class="list-container conferences">
      <h3>📅 Conferences</h3>
      <div class="badges">
        <span class="badge">ACL</span>
        <span class="badge">EACL</span>
        <span class="badge">EMNLP</span>
        <span class="badge">NAACL</span>
        <span class="badge">COLING</span>
        <span class="badge">IJCNLP</span>
        <span class="badge">SIGIR</span>
        <span class="badge">WWW</span>
        <span class="badge">ICON</span>
      </div>
    </div>
  </div>
</div>
