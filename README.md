## Website Performance Optimization portfolio project
This project is based on a Cameron Pittman's portfolio and pizzeria website.

### Optimizations
#### Optimizations for index.html
- Images optimized to reduce download time
- Pizza size image reduced to 100px to reduce download time
- Inlined styles.css to reduce load blocking CSS download
- Removed print.css from critical rendering path with media set to print.
- Asynchronously loading Google font
- Removed loading of unused 700 font weight
- Google Analytics JS tags loaded asynchronously

#### Optimizations for `index.html` and `views/js/main.js`
- Inlined styles.css  to reduce load blocking CSS download
- Reduced pizzeria.jpg image size and compressed
- Refactored “changePizzaSizes” function to remove forced synchronous layout, removing DOM queries out of the loop and setting size based on percent width.
- Refactors DOMContentLoaded function to only load pizzas based on window size (actual columns and rows. Previously set statically to 200.
- Replace querySelectorAll() that has too broad of a scope more efficient with getElementsByClassName

### Running the project
To run `index.html`, navigate your browser to [http://colinchong.github.io](http://colinchong.github.io).

From this page, use the last link for Cam's Pizzeria to view `pizza.html`.
