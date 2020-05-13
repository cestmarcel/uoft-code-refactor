# uoft-code-refactor
## Homework assignment no. 1 | May 12, 2020

Homework assignment for HTML/CSS as part of University of Toronto's Coding class. The task was to make a website's hmtl code more accessible by using semantic html. I replaced the div-tags in the document with more easily understandable tags to make the code more accessible. I also fixed a broken anchor link and made other adjustments, including cleaning up the CSS.

In the following I will be explaining what I changed in the __index.html file and other changes__ that I made.

### HTML-adjustments
- Wrapped emphasized part of wordmark in a mark-tag to make it more easily visible that this part of the wordmark is emphasized (this also involved a slight adjustment of the CSS, see below)
- Wrapped header area in header-tags
- Wrapped the links in the header in nav-tags (this step required CSS adjustments, see below) and all nav-tags in an additional div-tag so that the CSS still works (if the initial div is simply replaced with a nav-tag, the CSS does not work properly anymore).
- Wrapped the hero image in a figure-tag so that it becomes more clear at first glance that this is about an image
- Wrapped the main three content boxes for the agency's services in a main-tag to make it more visible that this part is the main content of the page.
    - Gave each of the three service-boxes a section-tag to make the three sections semantically visible
- Wrapped the benefits-area in an aside-tag to make it visible that this is content that is aside of the main content
    - Gave each of the three benefit descriptions section-tags
- Wrapped the footer in a footer-tag

### CSS-adjustments
- Defined correct background color for mark-tag, because after replacing the span-tag in the logo with mark it would be given a background-color of bright yellow by the browser (defined  background-color for .seo class in CSS)
- Replaced .header div with .header nav so that navigation links can be wrapped in a semantic nav-tag without losing their styling

### CSS cleanup
- Moved a and p styles to the top of the file
- Consolidated styles of the benefits-area by creating a new ".benefit-description" class to be able to eliminate duplicates
    - Moved font color into the .benefits class as it applies to all elements in that class
    - Also adjusted adjacent styles (e.g. headings)
- Consolidated .search-engine-optimization, .online-reputation-management, and .social-media-marketing in a new class to eliminate CSS duplicates
    - Adjusted adjacent styles (e.g. img-tags and headings)
- Defined most frequently used font family in body-style. Left Trebuchet font for header (wordmark) and footer styles as initially defined.
- Rearranged styles to follow the semantic structure of the html-elements.

### Other adjustments
- Gave all images alt-attributes
- Made footer headings an h4 so that it falls in a sequential order with the other headings
- Fixed anchor link to Search Engine Optimization section
- Made img-tag for cost benefit consistent with other img-tags in document
- Gave the website a more expressive title under the title-tag in the head-section to boost searchability