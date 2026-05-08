---
theme: neversink
layout: cover
transition: slide-up
---

# Ten a-maze-ing<br>uses for<br>maze algorithms.

Martijn van Iersel

<svg style="display:inline; color: blue" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M5.202 2.857C7.954 4.922 10.913 9.11 12 11.358c1.087-2.247 4.046-6.436 6.798-8.501C20.783 1.366 24 .213 24 3.883c0 .732-.42 6.156-.667 7.037c-.856 3.061-3.978 3.842-6.755 3.37c4.854.826 6.089 3.562 3.422 6.299c-5.065 5.196-7.28-1.304-7.847-2.97c-.104-.305-.152-.448-.153-.327c0-.121-.05.022-.153.327c-.568 1.666-2.782 8.166-7.847 2.97c-2.667-2.737-1.432-5.473 3.422-6.3c-2.777.473-5.899-.308-6.755-3.369C.42 10.04 0 4.615 0 3.883c0-3.67 3.217-2.517 5.202-1.026"/></svg>&nbsp;@mpvaniersel

---
layout: image
image: ./images/zelda-bow-labyrinth.jpg
transition: slide-down
---

<!-- Lomei labyrint island -->

<!-- <img src="./images/zelda-bow-labyrinth.jpg"> -->

---
layout: image-left
image: ./images/zelda2-maze-island.png
backgroundSize: contain
transition: slide-right
---

The *original* maze island...

from

Zelda II: The Adventure of Link

---
layout: image-left
image: ./images/squares.excalidraw.svg
backgroundSize: contain
transition: fade
---

# How to make a maze.

* Start with a grid.

---
layout: image-left
image: ./images/square-grid.excalidraw.svg
backgroundSize: contain
transition: fade
---

# How to make a maze.

* Start with a grid.
* Turn the grid into a **graph**.

---
layout: image-left
image: ./images/square-grid-msp.excalidraw.svg
backgroundSize: contain
transition: fade-out
---

# How to make a maze.

* Start with a grid.
* Turn the grid into a **graph**.
* Pick as few edges as possible.
* Graph theory calls this a **minimum spanning tree**.

---
layout: iframe-left

# the web page source
# url: https://amarillion.github.io/helixgraph/examples/maze/?grid=square&algorithm=recursivebt&ui=hidden
url: http://localhost:8080/examples/maze/?grid=square&algorithm=recursivebt&ui=hidden&animation=false
transition: slide-right
---

# A perfect maze

* Always exactly one path between two points

---
layout: image-left
image: ./images/zelda2-maze-island-loop-marked.png
backgroundSize: contain
transition: slide-down
---

# Not perfect

* Loops
* No dead ends? Braid maze.

---
layout: image-left
image: ./images/mazes-for-programmers-book-cover.jpg
transition: fade-out
---

# It began with a book

---
layout: image
image: ./images/topdesk-maze.png
backgroundSize: contain
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #1" v-drag="[740,75,175,102,15]">
Junior Programmer Training assignment
</StickyNote>

---
transition: fade-out
---

# Object Oriented programming

<img src="./images/oop.excalidraw.svg" v-drag="[236,107,458,355]"/>

---
transition: fade-out
---

# Functional programming

<img src="./images/functional.excalidraw.svg" v-drag="[137,198,652,157]"/>

---
layout: image
image: ./images/topdesk-maze-linkedin-collapsed.png
backgroundSize: contain
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #2" v-drag="[740,75,175,102,15]">
Pandemic boredom buster
</StickyNote>


---
transition: fade
---

# Getting creative with grids

* **Any grid** can be turned into a graph

<img src="./images/square-and-triangular-grid.excalidraw.svg">

---
transition: slide-left
---

# Getting creative with grids

* Maze algorithms **just work**!

<img src="./images/square-and-triangular-grid-msp.excalidraw.svg">

---
transition: slide-down
---

# Robin Maze

<img src="./images/topdesk-logo.png" v-drag="[333,13,517,81]">

<SlidevVideo autoplay v-drag="[214,187,525,316]" autoreset="slide">
  <source src="./images/robin-2021-11-14.webm" type="video/webm"/>
</SlidevVideo>

---
layout: image
image: ./images/creative-coding-workshop.jpg
backgroundSize: contain
transition: slide-right
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #3" v-drag="[737,75,175,129,15]">
Bring programmers and non-programmers together with a creative coding workshop
</StickyNote>

---
transition: fade-out
---

# Genuary 2025: Grid in grid

<SlidevVideo autoplay v-drag="[255,108,513,395]"  autoreset="slide">
  <source src="./images/Screencast from 2026-02-01 16-35-01.mp4" type="video/mp4"/>
</SlidevVideo>

---
layout: center
transition: fade-out
---

# Maze Algorithms

* Recursive Backtracker
* Prim's
* Kruskal's

---
layout: iframe-left

# the web page source
# url: https://amarillion.github.io/helixgraph/examples/maze/?grid=square&algorithm=prim_random&ui=hidden&animation=true&color=dist
url: http://localhost:8080/examples/maze/?grid=square&algorithm=prim_last_node&ui=hidden&animation=true&color=degree
transition: fade-out
---

# Prim's algorithm

* Very flexible
* This variant looks like the **recursive backtracker**
* Long branches

---
layout: iframe-left

# the web page source
# url: https://amarillion.github.io/helixgraph/examples/maze/?grid=square&algorithm=prim_random&ui=hidden&animation=true&color=dist
url: http://localhost:8080/examples/maze/?grid=square&algorithm=prim_random&ui=hidden&animation=true&color=degree
transition: fade-out
---

# Prim's algorithm 

* Very flexible
* This one is more random
* Shorter branches, more dead ends

---
layout: image
image: ./images/xmas-card-2022.png
transition: slide-right
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #4" v-drag="[740,75,175,102,15]">
Make something pretty
</StickyNote>

<!--
Using weights
Snowflake maze
Xmas cards
-->

---
layout: iframe
url: https://amarillion.github.io/snowflake-maze/
transition: slide-up
---

---
layout: iframe-left

# the web page source
# url: https://amarillion.github.io/helixgraph/examples/maze/?grid=square&algorithm=prim_random&ui=hidden&animation=true&color=dist
url: http://localhost:8080/examples/maze/?grid=square&algorithm=kruskal&ui=hidden&animation=true&color=none
transition: fade-out
---

# Kruskal's algorithm

* Especially useful when mixing pre-existing structures

---
layout: image
image: ./images/reddit-post.png
backgroundSize: contain
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #5" v-drag="[740,75,175,102,15]">
Reddit karma
</StickyNote>

---
transition: fade-out
---

<SlidevVideo autoplay v-drag="[153,29,659,508]" autoreset="slide">
  <source src="./images/capylandia.webm" type="video/webm"/>
</SlidevVideo>

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #6" v-drag="[740,75,175,102,15]">
Procedural level generation 
</StickyNote>

---
layout: image
image: ./images/tins_2026_poster-10-basic_banner.png
transition: slide-right
backgroundSize: contain
---

---
transition: fade-out
---

Food chain farm ecosystem game

---
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #7" v-drag="[740,75,175,102,15]">
Testing a graph based engine
</StickyNote>

---
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #8" v-drag="[740,75,175,102,15]">
Generate a treasure map
</StickyNote>

Problem: puzzle pieces need to have at least one connection to the rest
Solution: this is actually a minimum spanning tree problem

---
layout: image
image: ./images/i18n-puzzles-banner.png
transition: fade-out
---

---
layout: image
image: ./images/maze-generation-in-minecraft.png
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #9" v-drag="[740,75,175,102,15]">
Build something really complicated in Minecraft
</StickyNote>

<StickyNote color="blue-light" textAlign="left" width="180px" title="YouTube credit" v-drag="[39,19,185,81]">
CaptainLuma<br>
youtu.be/zbXKcDVV4G0
</StickyNote>

---
transition: fade-out
---

<StickyNote color="pink-light" textAlign="left" width="180px" title="Use #10" v-drag="[740,75,175,102,15]">
Talk about it at meetups and conferences.
</StickyNote>

QR Code
<QRCode value="https://amarillion.github.io/helixgraph/examples/maze/" :size="200" render-as="svg" />

Martijn van Iersel

<svg style="display:inline; color: blue" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path fill="currentColor" d="M5.202 2.857C7.954 4.922 10.913 9.11 12 11.358c1.087-2.247 4.046-6.436 6.798-8.501C20.783 1.366 24 .213 24 3.883c0 .732-.42 6.156-.667 7.037c-.856 3.061-3.978 3.842-6.755 3.37c4.854.826 6.089 3.562 3.422 6.299c-5.065 5.196-7.28-1.304-7.847-2.97c-.104-.305-.152-.448-.153-.327c0-.121-.05.022-.153.327c-.568 1.666-2.782 8.166-7.847 2.97c-2.667-2.737-1.432-5.473 3.422-6.3c-2.777.473-5.899-.308-6.755-3.369C.42 10.04 0 4.615 0 3.883c0-3.67 3.217-2.517 5.202-1.026"/></svg>&nbsp;@mpvaniersel

<PoweredBySlidev mt-10 />


---
transition: slide-up
layout: two-cols-header
---

# Links

<style>
a { 
  color: teal; 
}
</style>
::left::

* These slides... ##TODO##
* Mazes for programmers<br>http://www.mazesforprogrammers.com/
* HelixGraph Github repo<br>https://github.com/amarillion/helixgraph/
* HelixGraph npm library<br>https://www.npmjs.com/package/@amarillion/helixgraph
* HelixGraph Github Pages<br>https://amarillion.github.io/helixgraph/
* Algorithm toy<br>https://amarillion.github.io/helixgraph/examples/maze/

::right::

* Snowflake maze<br>https://amarillion.github.io/snowflake-maze/
* Food Chain Farm (ecosystem game)<br>https://helixsoft.itch.io/food-chain-farm
* Fole & Raul (generated dungeon game)<br>https://tins.amarillion.org/entry/283
* TINS Game Jam<br>https://tins.amarillion.org
* Internationalization puzzles (for programmers)<br>https://i18n-puzzles.com/
* @mpvaniersel on bluesky<br>
