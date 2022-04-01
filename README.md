# HTML-Semantics-Refactoring

>> Refactoring a HTML page for better accessibility

The following aspects have been considered and the relevant changes have been made as described below:


Logical division of the page:

Using semantic elements header and footer instead of div
    Note: kept the class so that the CSS still worked as it was, but that can be adjusted

Using semantic elements in the body:
Using nav tags inside the header to enclose the unordered list
    Note: adjusted the CSS descriptions accordingly

Using section tags instead of div tags for the content section

Using aside tags instead of div tags for the benefits section (side part)


Identification of the different elements:

Using figure tags around images to enclose the img tags and its caption (if relevant)
    Note: that helps when placed just before a paragraph (for example in benefits section), so the screen reader knows the difference between the picture's info and a separate paragraph

Adding alt attribute into the img attributes to give a description for each picture and icon
    Note: that helps the screen reader when reading the images on the page

Adding a longer description in the title space to have a more meaningful title

Adjusting the header in the footer to h4 so that it falls into a logical order with the others
    Note: adjusted in html line and CSS description


Bug fix:
Added an id to first nav bar item target to redirect to correct location on page

