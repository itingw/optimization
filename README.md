## Website Performance Optimization portfolio project

####Part 1: Optimize PageSpeed Insights score for index.html

1. Minimize render blocking
  - Media Queries
  - Inline CSS
2. Minimize parser blocking JS
  - Add async
3. Resize Images using Grunt
4. Convert Images to png format
5. Move scripts to end of the body

####Part 2: Optimize Frames per Second in pizza.html

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
