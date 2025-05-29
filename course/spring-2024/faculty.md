---
layout: default
title: Faculty
permalink: /course/spring-2024/faculty/
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



<h2>{% include icon.html icon="fa-person-chalkboard" %} Instructor</h2>

<div class="portrait-list">
  {% include list.html data="members" component="portrait" filter="role == 'Faculty'" %}
</div>

</div>
