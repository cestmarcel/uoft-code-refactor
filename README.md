# uoft-code-refactor
## Homework assignment no. 1, May 12, 2020

Homework assignment for HTML/CSS as part of University of Toronto's Coding class. The task was to make a website's hmtl code more accessible by using semantic html. I replaced the div-tags in the document with more easily understandable tags to make the code more accessible. I also fixed a broken anchor link and made other slight adjustments.

In the following I will be explaining what I changed in the __index.html file and other changes__ that I made.

### HTML-adjustments
- Wrapped the "SEO" part of the wordmark in a mark-tag to make it more easily visible that this part of the wordmark is emphasized (this step required a slight CSS adjustment, see below)
- Wrapped header area in header-tags and the links in the header in nav-tags (this step required CSS adjustments, see below)
- Wrapped the hero image in a figure-tag so that it becomes more clear at first glance that this is about an image
- Wrapped the main three content boxes for the agency's services in a main-tag to make it more visible that this part is the main content of the page.
    - Gave each of the three service-boxes a section-tag to make the three sections semantically visible
- Wrapped the benefits-area in an aside-tag to make it visible that this is content that is aside of the main content
    - Gave each of the three benefit descriptions section-tags
- Wrapped the footer in a footer-tag

### CSS-adjustments
Two adjustments to the project's CSS were necessary in order to use semantic HTML while keeping the existing styling of these elements.
- defined correct background color for mark-tag, because after replacing the span-tag in the logo with mark it would be given a background-color of bright yellow by the browser
- replaced .header div with .header nav so that navigation links can be wrapped in a semantic nav-tag without losing their styling

### Other adjustments
- Fixed anchor link to Search Engine Optimization section
- Made img-tag for cost benefit consistent with other img-tags in document
- Gave the website a more expressive title under the title-tag in the head-section to boost searchability