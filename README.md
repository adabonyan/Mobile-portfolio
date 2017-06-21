# Project Objectives
Optimize to meet specifications for:
- Critical Rendering Path
- Frame Rate of 60fps
- Computation Efficiency

## Download
To download the app, click [here]( https://adabonyan.github.io/frontend-nanodegree-mobile-portfolio/)

## Major changes
### index.html
- Removed the link to google fonts (to save roundtrip time to get this font). On style.css, Serif, Sans-serif are added. This covers all browsers
- Added style for mobile devices to the head. This allows for faster page rendering on mobile devices
- Moved javascript from head to the bottom of the body
- Deleted the link to a separate perfmatters.js and copied file contect to the bottom of the body
- All js analytical scripts are `async`
- Deleted media print link. This is a small file. Content of file added to style.css


### style.css
- Deleted html style. Focus strictly on rendering the page(s).
- Defined body styles once.
- Created class for each element instead of hierarchical pointer (e.g. .headerP instead of header p)
- Used element Id instead of hierarchical pointer (footer span)


### images
Great reduction in images sizes

## Minor changes
### style.css
- Applied <b> tag instead of creating new classes b, strong
- Deleted link states styles for visited, focus and active; hover is just OK
- Deleted styles for <pre> and <code>; they are not used in the html



