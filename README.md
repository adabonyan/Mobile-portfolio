# Project Objectives
Optimize to meet specifications for:
- Critical Rendering Path
- Frame Rate of 60fps
- Computation Efficiency

## Download
To download the app, click [here]( https://adabonyan.github.io/frontend-nanodegree-mobile-portfolio/)


## Major changes
### html files
- Removed the link to google fonts (to save roundtrip time to get this font). On style.css, Serif, Sans-serif are added. This covers all browsers
- Added style for mobile devices to the head. This allows for faster page rendering on mobile devices
- Moved javascript from head to the bottom of the body
- Deleted the link to a separate perfmatters.js and copied file contect to the bottom of the body
- All analytical js are `async`
- Deleted media print link. This is a small file. Content of file added to style.css

### view/main.js  (pizza.html specific)
- Functions determineDx, sizeSwitcher and changePizzaSizes are deleted. A new function `changePizzaSizes` is called when the slider moves. Result is in % width of the image container.
- Declared variables which are used in more than one function as global.
- Declared variables (which are used inside a loop) outside and before the loop.
- In declaring variables, applied DOM getElementById, getElementsByClass instead of querySelector
- Reduce the total number of pizza to 26 (from 201). Note a small code is written just for the purpose of investigating the effect of pizza nu on performance
- Deleted eventListener attached to generating pizza images while loading the page

### style.css
- Deleted html style. Focus strictly on rendering the page (body).
- Defined body styles once.
- Created class for each element instead of hierarchical pointer (e.g. .headerP instead of header p)
- Used element Id instead of hierarchical pointer (footer span)

### images
Great reduction in images sizes


## Minor changes
### style.css
- Applied <b> tag instead of creating new classes b, strong
- Deleted link-state styles for visited, focus and active; hover is just OK
- Deleted styles for <pre> and <code>; they are not used

### view/style.css  (specific for pizza.html)
- Commented out some classes because they do not appear in the html and js files. This reduces memory usage.




