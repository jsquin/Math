---
title: AP Precalculus
layout: default

---

# {{ page.title }}

<style>
details summary {
    cursor: pointer;
    list-style: none;
    position: relative;
    padding-left: 20px; /* Add space for the custom arrow */
}

details summary::before {
    content: "▶";  /* Closed state arrow */
    position: absolute;
    left: 0;
}

details[open] summary::before {
    content: "▼";  /* Open state arrow */
}
  
details > div {
    margin-left: 20px; /* Indent the contents of the dropdown */
}
</style>

<details>
  <summary>Unit 1: Polynomial and Rational Functions</summary>
  <div>
    <a href="/units1/unit1.md">1.1: Bingus</a><br>
    <a href="/units1/unit1.md">1.2: Bingus2</a><br>
  </div>
</details>

<details>
  <summary>Unit 2: Exponential and Logarithmic Functions</summary>
  <div>
    <a href="/units1/unit1.md">1.1: Bingus</a><br>
    <a href="/units1/unit1.md">1.2: Bingus2</a><br>
  </div>
</details>

<details>
  <summary>Unit 3: Polynomial and Rational Functions</summary>
  <div>
    <a href="/units1/unit1.md">1.1: Bingus</a><br>
    <a href="/units1/unit1.md">1.2: Bingus2</a><br>
  </div>
</details>

<details>
  <summary>Unit 4: Polynomial and Rational Functions</summary>
  <div>
    <a href="/units1/unit1.md">1.1: Bingus</a><br>
    <a href="/units1/unit1.md">1.2: Bingus2</a><br>
  </div>
</details>

<!-- Add the Collapse All text (initially hidden) -->
<p id="collapseText" style="display: none; cursor: pointer; color: cyan;" onclick="collapseAll()">Collapse All</p>

<!-- Add JavaScript for collapsing all dropdowns and showing/hiding the text -->
<script>
// Function to collapse all open <details> elements
function collapseAll() {
  const details = document.querySelectorAll("details");
  details.forEach((detail) => {
    detail.removeAttribute("open");
  });
  toggleCollapseText();  // Hide the Collapse All text once all are collapsed
}

// Function to show/hide the Collapse All text based on open details
function toggleCollapseText() {
  const details = document.querySelectorAll("details");
  const collapseText = document.getElementById("collapseText");
  
  // Check if any <details> are open
  const anyOpen = Array.from(details).some((detail) => detail.hasAttribute("open"));

  // Show the Collapse All text if any <details> are open, otherwise hide it
  if (anyOpen) {
    collapseText.style.display = "block";
  } else {
    collapseText.style.display = "none";
  }
}

// Add event listeners to each <details> to monitor for open/close changes
document.querySelectorAll("details").forEach((detail) => {
  detail.addEventListener("toggle", toggleCollapseText);
});
</script>

<!--
https://precalculus.flippedmath.com/ap-precalc.html
https://mathspace.co/textbooks/syllabuses/Syllabus-1171/topics/Topic-22118/
https://precalculus.flippedmath.com/unit-1a-review.html


-->












