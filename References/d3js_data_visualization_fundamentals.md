Pluralsight course by Lars Verspohl

Lars covers D3.js in depth at a conceptual level and shows examples to illustrate the concepts covered. To have an in-depth understanding of what D3.js offers, he has to introduce the audience to other concepts fundamental to creating data visualization.

D3 is a low-level Javascript Library for manipulating the document object model(DOM) with data. D3 is a collection of modules. The core abstraction it offers is binding data to dom elements. By binding data to dom elements, the dom elements can size, transform, shape, color themselves to the specification creating informative visualization. The data join produces data categorized into differnt data change states; enter, update and exit state. D3 uses web technologies (HTML, SVG, CANVAS) to actually do the drawing in the DOM. D3 offers many helper libraries on top of the core data join abstraction. This ranges from functions to help scale data to the screen/pixel locations to stratification of data for hierarchical structure to user interaction infrastructure to capture user and browser events.

D3 is a low-level library. It offers a lot of control of dom manipulation to the user. Because of this it can have a higher learning curve to use than other higher-level libraries that require the user to know less. The following concepts are all useful to know when working with D3.

- General Update Pattern: This pattern exists to take advantage of the D3 data join. As a consequence, code becomes structured to abstract dyanamic parts of the code from static.
  - Create or get an existing d3 dom element, join new data to this element to create the data state categories, then deal with each category of data states programatically

Throughout the course, Lars touches on topics of making better choices through visual design. Often this is motivated by having the audience of the visualization to work less. 

Transitions are used to reduce cognitive load by making it easier to follow data. They help maintain object constancy.

There are many interaction tools available for data visualization that have a variety of consequences. Highlighting can reduce distraction while tooltips can serve additional information about a data point.

Lars focuses on using SVG as the drawing tool. SVG defines a canvas of an absolute pixel length. This canvas accepts children elements like line, circle, and text. SVG offers the ability to group children together and apply transformations to the group.

The re-usable module pattern intent is to create modules to share configurable data visualizations created from D3. It suggests to have sensible defaults for configuration and use chainable function calls after object instantiation. One way this can be achieved is via closure.

Lars also offers a couple systematic approaches to common problems. 

For data visualization in general, he recognized this cycle. 
1. Define the goal
2. Source, shape and clean the data
3. Draw the data
4. Collect insight
5. Refine goal
Repeate the process until satisfaction

For drawing data, Lars recognized this pattern.
0. Sketch desired visualization
1. Fetch and transform data
2. Chart dimensions
3. Calculate scales
4. Join data and draw
5. Add Axis 
6. Refine drawing
