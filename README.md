## Website Performance Optimization portfolio project
This purpose of this project is to optimize the given portfolio page for speed.

#### Access the Project
Access the page here: https://itingw.github.io/optimization/

-OR-

1. Download the repository
2. Unzip the repository
3. Open "index.html" in any browser

#### Part 1: Optimize PageSpeed Insights score for index.html

1. Minimize render blocking
  - Media Queries
  - Inline CSS
2. Minimize parser blocking JS
  - Add async
3. Resize Images using Grunt
4. Convert Images to png format
5. Move print CSS and scripts to end of the body


#### Part 2: Optimize Frames per Second in pizza.html

1. Optimize updatePositions()
  - Move variable out of loop to avoid accessing document
  - Calculate items.length out of loop
2. Optimize document.addEventListener('DOMContentLoaded', function()
  - Optimize number of pizzas in loop by calculating the number of pizzas according to window height
  - Move variable out of loop to avoid accessing document
3. Optimize functions to resize Pizzas
  - Replace querySelector by getElementById to increase speed
  - Replace querySelectorAll by getElementsByClassName to increase speed
  - Calculate document.querySelectorAll(".randomPizzaContainer").length out of loop
4. Optimize window.performance.mark
  - Move pizzasDiv outside of loop
5. Enable hardware acceleration in CSS
  - Add transform and backface-visibility
