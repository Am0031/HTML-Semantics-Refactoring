# HTML-Semantics-Refactoring

**Refactoring a HTML page for better accessibility**

This webpage's code is already built but its **semantic elements** were reviewed in order to be made more accessible for screen readers.

Deployed URL:

Github URL:

## Introduction - What are HTML Semantic elements

A semantic element is a tag that clearly describes the role of a part of the code or portion of the browser. It helps describe its function within the structure of the page.
More explanations and a list of semantic elements can be found on [the W3 schools website](https://www.w3schools.com/html/html5_semantic_elements.asp)
More details on each semantic tag can be found on [the mdn website](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html) and this [youtube video](https://www.youtube.com/watch?v=g2tzEil5TL0) is a good starting point to understand why using semantic matters.

The aspects listed below are important when looking at accessibility and good use of semantic elements:

## Semantic elements - Best practices

To make sure the html code is optimised for accessibility, it is good to follow these [best practices](https://www.freecodecamp.org/news/html-best-practices/#:~:text=It%20is%20best%20practice%20to,and%20elements%20instead.)
For this code review, we will be reviewing the following principles:

- Logical division of the page
- Better identification of the different elements on the page
- Bug fix for full accessibility

And we will also do some CSS refactoring for cleaner code.

Following these principles, the details of the changes made are shown in the descriptions and screenshots below.

## Logical division of the page:

To make sure the division of the page followed a good logic:

- We amended the code for the use of semantic elements header and footer instead of div

  See before and after header tags:

  Before:

  ![Original header code](/assets/images/screenshot-header-original.png)

  After amendment:

  ![Amended header code](/assets/images/screenshot-header-tag.png)

  See before and after footer tags:

  Before:

  ![Original footer code](/assets/images/screenshot-footer-original.png)

  After amendment:

  ![Amended footer code](/assets/images/screenshot-footer-tag.png)

- We amended the code for the use of semantic elements in the body:

  - Using nav tags inside the header to enclose the unordered list (_Note: adjusted the CSS descriptions accordingly_)
  - Using main and section tags instead of some of the div tags for a better structured content section
  - Using aside tags instead of div tags for the benefits section (side part of the page)

  See screenshot of amended tags:

  Before:

  ![Original main section](/assets/images/screenshot-main-original.png)

  After amendment:

  ![Amended main section](/assets/images/screenshot-main-tag.png)

## Identification of the different elements on the page:

To make sure the elements were identified correctly:

- We added additional properties for the hero image to made it more accessible.

  Original line:

  ![Original code line for hero image](/assets/images/screenshot-hero-original.png)

  Amended line:

  ![New code line for hero image](/assets/images/screenshot-hero-aria.png)

- We added the figure tags around images to enclose the img tags and its caption (if relevant).
  _Note: that helps when placed just before a paragraph (for example in benefits section), so the screen reader knows the difference between the picture's info and a separate paragraph_

- We added alt attribute into the img attributes to give a description for each picture and icon.
  _Note: that helps the screen reader when reading the images on the page_

  For example:

  ![Example of figure tags and alt attribute](/assets/images/screenshot-fig-alt.png)

- We amended the title: we gave a longer description in the title space to have a more meaningful title

  Original code:

  `<title>website</title>`

  Improved code:

  `<title>Horiseon - Digital Marking and Online Management</title>`

- We adjusted the header tag in the footer to h4 so that it falls into a logical order with the other header tags.
  _Note: adjusted in html code and in CSS description_

## Bug fix:

To make the page fully accessible, the redirection link must work and direct you to the right part of the page. </br>
To that effect, we added an id to the first nav bar item target to redirect to the correct part of the main section.

## Improvement of the CSS:

As part of our accessibility exercise, we also looked to improve the CSS code and we made the following changes:

- Grouping the different classes of the benefits in the aside part into one class called benefit-subset as they all have the same attributes and values
- Grouping the different classes of the sections in the main part into one class called content-subset as they all have the same attributes and values

## Still To Do:

- Review semantic elements to improve them
- Continue the refactoring of CSS code
- Review/Add comments
- Add screenshots
- Add link to deployed github page
