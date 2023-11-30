---
title: Christmas Poems! 🎄
date: 2023-11-30T01:31:32.452Z
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
<h1>Random Christmas Poem</h1>
  <button onclick="getRandomPoem()">Get Random Poem</button>
  <p id="poem"></p>

  <script>
    const poems = [
      "Twas the night before Christmas, when all through the house...",
      "In the bleak midwinter, frosty wind made moan...",
      // Add more poems here
    ];

    function getRandomPoem() {
      const poemElement = document.getElementById("poem");
      const randomIndex = Math.floor(Math.random() * poems.length);
      poemElement.textContent = poems[randomIndex];
    }
  </script>