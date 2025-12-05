---
layout: page
title: Sci-art
permalink: /sci-art/
---

A small gallery of science-inspired art.

---

<div class="view-toggle">
  <button class="toggle-btn active" onclick="showGridView()">Grid view</button>
  <button class="toggle-btn" onclick="showScrollView()">Scroll view</button>
</div>

<div id="grid-view" class="art-grid">

  <figure>
    <img src="/assets/img/sci-art/Sciontho.png" alt="Sciontho" />
    <figcaption>Unpack dense science with Sciontho! (2025)</figcaption>
  </figure>

  <figure>
    <img src="/assets/img/sci-art/MirrorMirror.png" alt="Mirror self-recognition test" />
    <figcaption>Mirror self-recognition test — a classic behavioural experiment used to study self-awareness in animals.</figcaption>
  </figure>

  <figure>
    <img src="/assets/img/sci-art/DBJC.png" alt="Development and Behaviour Journal Club" />
    <figcaption>The Development and Behaviour Journal Club at the BLiSc campus, Bangalore.</figcaption>
  </figure>

  <figure>
    <img src="/assets/img/sci-art/MyPhD.png" alt="My PhD" />
    <figcaption>My PhD — the long, winding path through research.</figcaption>
  </figure>

</div>

<div id="scroll-view" markdown="1" style="display:none;">

## Gallery (scroll view)

### Unpack dense science with Sciontho! (2025)

![Sciontho](/assets/img/sci-art/Sciontho.png){: .sciart }

---

### Mirror self-recognition test — a classic behavioural experiment used to study self-awareness in animals

![Mirror mirror](/assets/img/sci-art/MirrorMirror.png){: .sciart }

---

### The Development and Behaviour Journal Club at the BLiSc campus, Bangalore

![DBJC](/assets/img/sci-art/DBJC.png){: .sciart }

---

### My PhD — the long, winding path through research

![My PhD](/assets/img/sci-art/MyPhD.png){: .sciart }

</div>

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
