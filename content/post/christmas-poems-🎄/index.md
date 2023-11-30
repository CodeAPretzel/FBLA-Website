---
title: Christmas Poems! 🎄
date: 2023-11-30T01:31:32.452Z
summary: G﻿et into the Christmas spirit by reading some poems!
draft: false
featured: true
tags:
  - Entertainment
image:
  filename: website-images-christmas-poems.jpg
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
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s, color 0.3s;
    }

    button:hover {
      background-color: #e8dcdc;
    }
  </style>

<h1>Get a Christmas Poem!</h1>
 ﻿ <br>
  <button onclick="getRandomPoem()">CLICK HERE</button>
 ﻿ <br>
 ﻿ <br>

  <p id="poem"></p>

  <script>
    const poems = [
      `Setting up the nativity is a holiday tradition,
And each and every figure has its own special position.
The angel sits up on the roof, and the wise men go beneath.
Joseph and Mary go in the middle, surrounded by cows and sheep.
Baby Jesus in his manger always sits right in the center,
So everyone can admire him in all his glory and splendor.`,
      `Each year when Christmas rolls around
I get my nutcracker out.
And each time that he cracks a nut,
it makes me want to shout,
"Oh thank you Mr. Nutcracker for
Shelling my nuts for me.
Now all I need is a glass of eggnog,
and I'll eat them by my Christmas tree!"`,
 ﻿     `Copy this in your search bar:

https://docs.google.com/forms/d/e/1FAIpQLSewOaDbpc01h--dFwFSdwMb1gPG5iUtw-gWZZw0YitDXjCD-A/viewform?usp=sf_link`
    ];

    function getRandomPoem() {
      const poemElement = document.getElementById("poem");
      const randomIndex = Math.floor(Math.random() * poems.length);
      poemElement.textContent = poems[randomIndex];
    }
  </script>

