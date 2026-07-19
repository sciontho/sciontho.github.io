---
layout: page
title: in-verse
permalink: /in-verse/
---

Some poems I've scribbled down.

This is where I keep little poems that grow out of papers, ideas, talks, and lab life —
sometimes serious, mostly silly, often somewhere in between.

---

<div class="view-toggle">
  <button class="toggle-btn active" onclick="showGridView()">Gallery</button>
  <button class="toggle-btn" onclick="showScrollView()">Reading mode</button>
</div>

<div id="grid-view" class="poem-grid">

  <!-- Poem 1 -->
  <figure class="poem-card">
    <img src="/assets/img/in-verse/AnouksFantasy.png" alt="Anouk's Fantasy – a science poem">
    <figcaption>
      <strong>Why are some of us more drawn to the fantastic than others?</strong><br>
      A poem about <a href="https://sciwri.club/archives/13631" target="_blank" rel="noopener noreferrer">this wonderful article</a> by Apeksha Srivastava. Illustration by Andreia Rocha.
    </figcaption>
  </figure>

  <!-- Poem 2 -->
  <figure class="poem-card">
    <img src="/assets/img/in-verse/DiscoveringExoplanets.png" alt="The Discovery of Exoplanets">
    <figcaption>
      <strong>Are there other Suns with Earths going around them?</strong><br>
      The answer is yes—there are other stars with planets in orbit. But how did we discover these distant worlds?
      A poem inspired by <a href="https://sciwri.club/archives/13671" target="_blank" rel="noopener noreferrer">this article</a> by Moupiya Maji.
    </figcaption>
  </figure>

</div>

<div id="scroll-view" markdown="1" style="display:none;">

## Why are some of us more drawn to the fantastic than others?

![Anouk's Fantasy](/assets/img/in-verse/AnouksFantasy.png){: .poem-full }

A poem about <a href="https://sciwri.club/archives/13631" target="_blank" rel="noopener noreferrer">this wonderful article</a> by Apeksha Srivastava. Illustration by Andreia Rocha.

---

## Are there other Suns with Earths going around them?

![Discovering Exoplanets](/assets/img/in-verse/DiscoveringExoplanets.png){: .poem-full }

The answer is yes—there are other stars with planets in orbit. But how did we discover these distant worlds?

Inspired by <a href="https://sciwri.club/archives/13671" target="_blank" rel="noopener noreferrer">this article</a> by Moupiya Maji.

</div>

---

If you'd like to use any of these poems for teaching, outreach, or a journal club,
feel free to get in touch—I'm always happy to share or adapt them.

{% raw %}
<script>
  function showGridView() {
    document.getElementById("grid-view").style.display = "grid";
    document.getElementById("scroll-view").style.display = "none";
    setActiveButton("grid");
  }

  function showScrollView() {
    document.getElementById("grid-view").style.display = "none";
    document.getElementById("scroll-view").style.display = "block";
    setActiveButton("scroll");
  }

  function setActiveButton(view) {
    const buttons = document.querySelectorAll(".toggle-btn");
    buttons.forEach(btn => btn.classList.remove("active"));
    if (view === "grid") {
      buttons[0].classList.add("active");
    } else {
      buttons[1].classList.add("active");
    }
  }
</script>
{% endraw %}
