---
layout: default
title: Books
permalink: /course/spring-2024/books/
---
<style>
.page-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  box-sizing: border-box;
  text-align: center;
  background-color: #f9f9f9;
}

/* Headings spacing */
h1, h2, h3, h4, h5, h6 {
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}

/* Book list as 2-column grid */
.book-list {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
  max-width: 900px;
  width: 100%;
  justify-items: center;
}

/* Book card styling */
.book-card {
  border: 1px solid #999; /* darker border */
  border-radius: 10px;
  padding: 1rem;
  width: 100%;
  max-width: 300px;
  text-align: center;
  background: #ffffff;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.book-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.12);
}

.book-card img {
  max-width: 100%;
  height: auto;
  border-radius: 6px;
  margin-bottom: 0.5rem;
}

.book-card h3 {
  font-size: 1.1rem;
  margin: 0.5rem 0 0.3rem;
}

.book-card p {
  margin: 0;
  font-size: 0.9rem;
  color: #333;
}

.book-card a {
  display: inline-block;
  margin-top: 0.5rem;
  text-decoration: none;
  color: #005ea2;
  font-weight: bold;
}

/* Divider line styling */
hr {
  border: none;
  border-top: 1px solid #bbb;
  width: 90%;
  margin: 1rem auto;
}

/* Responsive fallback for small screens */
@media screen and (max-width: 640px) {
  .book-list {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="page-container">

<h1>{% include icon.html icon="fa-person-chalkboard" %} Recommended Books for Foundations of NLP - Spring 2024, MU</h1>

<!-- Book Display Section -->
<div class="book-list">
  {% assign books = site.data.fNLP-fall-2024 | where: "category", "books" %}
  {% for book in books %}
  <div class="book-card">
    <img src="{{ book.book_image }}" alt="{{ book.title }}">
    <hr/>
    <h3>{{ book.title }}</h3>
    <p><strong>Author:</strong> {{ book.author }}</p>
    <a href="{{ book.link }}" target="_blank">📖 Read</a>
  </div>
  {% endfor %}
</div>

<hr style="margin: 2rem 0; width: 80%;"/>

</div>
