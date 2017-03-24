#Table of Contents
  1. How to run
  2. Optimizations made
    2.1 index.html
    2.2 views/js/main.js

=========================

## How to run
  1. Navigate to download folder (typically downloads/frontend-nanodegree-mobile-portfolio)
  2. Open index.html

=========================

## Optimizations made

### index.html
1. Compressed images
2. Inlined css
3. Removed render-blocking css (google font)
4. Added the async attribute to the external JavaScript

### views/js/main.js
1. Moved switch from sizeSwitcher function into changePizzleSlices function.
2. Removed conversion of units. Only uses percent now.
3. removed unnecessary parts of for loop. newWidth is determined in switch. query selector set to a variable, it returns an array. for loop just itterates through array. queryselector only needs to run once.
4. removed the document.body.scrollTop /1250 from inside the for loop as it is a constant and only needs to run once. set it to a variable which i used inside the for loop.
