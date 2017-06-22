# Project Objectives
Optimize to meet specifications for:
- Critical Rendering Path: Achieved PSI 87/100 for mobile/desktop
- Frame rate: Achieved 60fps while scrolling
- Computation Efficiency: Achieved < 5ms to resize pizza

## Download
To download the app, click [here]( https://adabonyan.github.io/frontend-nanodegree-mobile-portfolio/ )


## Major changes
### html
- Removed the link to google fonts. This saves roundtrip time to get these fonts. On style.css, Serif and Sans-serif were added.
- Added css style for mobile devices to the head. This allows for faster page rendering on mobile devices.
- Moved javascript from head to the end of the body.
- Deleted the link to a separate perfmatters.js and copied entire script to the end of body.
- All analytical js are `async`.
- Deleted media print link. This is a small file. Content of file added to style.css

### view/main.js  (pizza.html specific)
- These functions determineDx, sizeSwitcher and changePizzaSizes have been deleted. A new function `changePizzaSizes` is called when the slider moves. Result is in % width of the image container.
- Declared variables which are used in more than one function as global.
- Variables (which are used in for loop) declared outside and before the loop.
- Replaced all querySelector with either getElementById or getElementsByClass
- Reduce the total number of pizza from 201 to 26. Note a small code is written just for the purpose of investigating the effect of pizza nu on performance
- Deleted eventListener attached to generating pizza images while loading the page

### style.css
- Deleted styles for html. The styles are now for the body.
- Defined body styles once.
- Created class for each element instead of hierarchical pointer (e.g. .headerP instead of header p)
- Used element Id instead of hierarchical pointer (footer span)

### Images
Great reduction in images sizes


## Minor changes
### style.css
- Applied `<b>` tag instead of creating new classes b, strong
- Deleted link-state styles for visited, focus and active; hover is just OK
- Deleted styles for `<pre>` and `<code>`; they are not used

### view/style.css  (specific for pizza.html)
- Commented out some classes because they do not appear in the html and js files. This reduces memory usage.




