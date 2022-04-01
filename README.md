# HTML-Semantics-Refactoring

> > Refactoring a HTML page for better accessibility

This webpage's code is to be reviewed in order to be made more accessible for screen readers.
The aspects listed below have been reviewed and the relevant changes have been made. The details are shown in the descriptions and screenshots below.

- Logical division of the page
- Better identification of the different elements on the page
- Bug fix for full accessibility
- CSS refactoring for cleaner code

## Logical division of the page:

> Using semantic elements header and footer instead of div

    Note: kept the class so that the CSS still worked as it was, but that can be adjusted

> Using semantic elements in the body:

    Using nav tags inside the header to enclose the unordered list
    Note: adjusted the CSS descriptions accordingly

    Using main and section tags instead of div tags for the content section

    Using aside tags instead of div tags for the benefits section (side part)

## Identification of the different elements on the page:

Using figure tags around images to enclose the img tags and its caption (if relevant)
Note: that helps when placed just before a paragraph (for example in benefits section), so the screen reader knows the difference between the picture's info and a separate paragraph

Adding alt attribute into the img attributes to give a description for each picture and icon
Note: that helps the screen reader when reading the images on the page

Adding a longer description in the title space to have a more meaningful title

Adjusting the header in the footer to h4 so that it falls into a logical order with the others
Note: adjusted in html line and CSS description

## Bug fix:

Added an id to first nav bar item target to redirect to correct location on page

## Improvement of the CSS:

Grouping the different classes of the benefits in the aside part into one class called benefit-subset as they all have the same attributes and values
Grouping the different classes of the sections in the main part into one class called content-subset as they all have the same attributes and values

## Still To Do:

- Review semantic elements to improve them
- Continue the refactoring of CSS code
- Review/Add comments
- Add screenshots
- Add link to deployed github page
