---
title: Projects
nav:
  order: 2
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects, Funding, Featured & Grant

At the **VLANC** Lab, our research is centered on integrating **vision**, **language**, and **knowledge** to build intelligent systems that can comprehend and reason over multimodal data. Our ongoing projects span a range of areas, including:

<details markdown="1">
<summary>Graph-based Models</summary>
Graph-based models for entity linking and structured knowledge representation</details>

<details markdown="2">
<summary>Knowledge Graph Construction</summary>
Knowledge graph construction from unstructured text
</details>

<details markdown="3">
<summary>Multimodal Reasoning</summary>
Multimodal reasoning across image-text pairs
</details>

<details markdown="4">
<summary>Deep Generative Models</summary>
Deep generative models for interpreting brain-computer interface (BCI) signals
</details>







We are also actively investigating low-resource learning and domain adaptation techniques to enhance the robustness and generalizability of our models across diverse real-world scenarios


{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filter="group == 'featured'" %}

{% include section.html %}

## Others

{% include list.html component="card" data="projects" filter="!group"  %}
