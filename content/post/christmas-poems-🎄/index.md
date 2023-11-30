---
title: Christmas Poems! 🎄
date: 2023-11-30T01:31:32.452Z
summary: G﻿et into the Christmas spirit by reading some poems!
draft: false
featured: true
tags:
  - Entertainment
image:
  filename: christmas-animation.gif
  focal_point: Smart
  preview_only: false
---
  <style>
    /* CSS styles for the button */
    button {
      background-color: white;
      border: 2px solid black;
      border-radius: 5px;
      padding: 10px 40px;
      font-family: serif;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s, color 0.3s;
    }

    button:hover {
      background-color: #f0f0f0;
    }
  </style>

<h1>Get a Christmas Poem!</h1>
  <button onclick="getRandomPoem()">CLICK HERE</button>
 ﻿ <br>
 ﻿ <br>

  <p id="poem"></p>

  <script>
    const poems = [
      "Snowflakes dancing in the air,
Landing softly everywhere,
 
Blanketing the world in white,
A wondrous and magical sight.",
      "Christmas bells in the air,
Ringing out with love and care,
Joyful songs fill the night,
Bringing warmth and pure delight.",
 ﻿     "<insert-website>"
    ];

    function getRandomPoem() {
      const poemElement = document.getElementById("poem");
      const randomIndex = Math.floor(Math.random() * poems.length);
      poemElement.textContent = poems[randomIndex];
    }
  </script>

