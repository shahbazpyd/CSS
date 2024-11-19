# Flexbox Layout Experiment

This project was created as a learning exercise to understand and practice using CSS Flexbox for layout.  I wanted to build a common web page structure with a header, navigation, main content area (split into two columns), and a footer.  This document outlines my learning process and experiences.

## Key Learnings

* **`display: flex`**: This is the fundamental property that enables flexbox layout on an element. I applied it to the main container (`.container`) to control the overall page layout, as well as the `.container2` element to arrange the article and div side-by-side.  I also used it on `.container3` within the article to control the vertical positioning of elements within the article.

* **`flex-direction`**: This property controls the direction in which flex items are laid out.  I used `flex-direction: column` on the main container to create a vertical flow (header, nav, content, footer).  I then used `flex-direction: row` on `.container2` to place the article and div next to each other horizontally.

* **`width` and `height`**:  I learned how to use viewport units (`vw` and `vh`) to make elements scale relative to the browser window size.  This is useful for creating responsive layouts.

* **`justify-content`**: I experimented with `justify-content: flex-end` within `.container3` to align the article footer to the bottom of the article section. This showed me how flexbox can be used for aligning items within a container.

* **Nesting Flex Containers**:  I learned how to nest flex containers within each other.  For instance, `.container2` (with `flex-direction: row`) is nested inside `.container` (with `flex-direction: column`). This allows for complex layouts by combining different flex directions.

* **Margin and Border**: I included margins and borders primarily for visualizing the different sections and understanding how they affect the layout. This helped in debugging and fine-tuning the spacing.


## Experiences and Challenges

* **Box Sizing**: Early on, I encountered issues with element sizing due to default padding and border being added to the element's width.  Adding `box-sizing: border-box;` universally solved this, making the sizing more predictable.

* **Aligning the Article Footer**:  Getting the article footer to stick to the bottom of the article section required some experimentation. Using a nested flex container (`.container3`) with `justify-content: flex-end` proved to be the solution.  Initially, I tried using `margin-top` on the footer, which pushed the content down but didn't truly align it to the bottom in a flexible way.

* **Understanding Viewport Units**:  Getting used to `vw` and `vh` units took a bit of practice.  It's important to remember that they are relative to the viewport size, so the actual pixel dimensions will change as the browser window is resized.

## Next Steps

* Explore other flexbox properties like `align-items`, `flex-wrap`, and `flex-grow`.
* Experiment with different combinations of flexbox properties to create more complex layouts.
* Learn about responsive design principles and how to use flexbox to create layouts that adapt to different screen sizes.
* Practice building more real-world examples.


This experiment provided a good foundation for understanding the basics of flexbox layout. I'm looking forward to exploring its more advanced features and using it in future projects.
