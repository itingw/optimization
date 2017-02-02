## Website Performance Optimization portfolio project

####Part 1: Optimize PageSpeed Insights score for index.html

1. Minimize render blocking
  - Media Queries
  - Inline CSS
2. Minimize parser blocking JS
  - Add async
3. Resize Images using Grunt

####Part 2: Optimize Frames per Second in pizza.html

1. Lower number of sliding pizzas in sliding pizzas loop
2. Optimize updatePositions()
  -Remove document access from the loop
  -calculate items.length out of loop
