---
layout: page
title: Sci-on
permalink: /
---

<div class="poem-block" markdown="1">

  Let's try and think like Tinbergen:

***One**, "It's thus. What makes it so?"*  
***Two**, "Huh. But why should it be so?"*  
***Three**, "How has it come to be,*  
*What ingredients make the recipe?"*  
***Finally**, it must be solved*  
*How on earth has this evolved?*  

</div>

---

Welcome, welcome!

Tinbergen reckons that to understand behaviour, one must ask questions of four kinds - questions on "Causation", "Function", "Development" and "Evolution". And this shall serve as the foundation for the kinds of papers we’ll geek out on. So, we'll look at:

- **Causation** – What immediate processes cause the behaviour?  
- **Development** – How does the behaviour emerge?  
- **Function** – Why does it exist? What does it do for the animal?  
- **Evolution** – How did it arise over time?

We’ll interpret these terms freely (you’ll see!). Overall, though, these four lenses guide how I read papers and think about science.

Use the navigation bar above to explore.

---

# Featured

<div class="featured-grid">

  {% assign featured_posts = site.posts | sort: "date" | reverse %}

  {% for post in featured_posts limit:6 %}
    <a href="{{ post.url | relative_url }}" class="featured-card">
      <img src="{{ post.thumbnail | default: '/assets/img/sci-art/Sciontho.png' }}" alt="{{ post.title }}">
      <div class="featured-title">{{ post.title }}</div>
    </a>
  {% endfor %}

</div>
