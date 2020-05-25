Pluralsight course by Lars Verspohl

Lars covers D3.js in depth at a conceptual level and shows examples to illustrate the concepts covered. To have an in-depth understanding of what D3.js offers, he has to introduce the audience to other concepts fundamental to creating data visualization.

D3 is a low-level Javascript Library for manipulating the document object model(DOM) with data. D3 is a collection of modules. The core abstraction it offers is binding data to dom elements. By binding data to dom elements, the dom elements can size, transform, shape, color themselves to the specification creating informative visualization. The data join produces data categorized into differnt data change states; enter, update and exit state. D3 uses web technologies (HTML, SVG, CANVAS) to actually do the drawing in the DOM. D3 offers many helper libraries on top of the core data join abstraction. This ranges from functions to help scale data to the screen/pixel locations to stratification of data for hierarchical structure to user interaction infrastructure to capture user and browser events.

D3 is a low-level library. It offers a lot of control of dom manipulation to the user. Because of this it can have a higher learning curve to use than other higher-level libraries that require the user to know less. The following concepts are all useful to know when working with D3.

- General Update Pattern: This pattern exists to take advantage of the D3 data join. As a consequence, code becomes structured to abstract dyanamic parts of the code from static.
  - Create or get an existing d3 dom element, join new data to this element to create the data state categories, then deal with each category of data states programatically

- Visual Design: This is a field of study to enhance usability/readability and reduce cognitive burden for understanding visuals. Understanding visual design concepts and patterns is key to making more effective visualization.
  - Transitions are used to reduce cognitive load by making it easier to follow data. They help maintain object constancy.
  - Interactions have many different consequences as there are many different types of interactions available with data visualization. For example, Highlighting can reduce distraction while tooltips can serve additional information about a data point.
  
- SVG: Lars focuses on using SVG as the drawing tool. SVG defines a canvas of an absolute pixel length. This canvas accepts children elements like line, circle, and text. SVG offers the ability to group children together and apply transformations to the group.

- Re-usable module pattern: The intent is to create modules to share configurable data visualizations created from D3. It suggests to have sensible defaults for configuration and use chainable function calls after object instantiation. One way this can be achieved is via closure.

- Data Structures: It is impossible to create certain visualization unless data is structured in a way that allows for it. D3 has some helper libraries to move and re-structure data. It is important to understand what kind of data, format of data, and structure of data to know what visualizations are then possible to create to answer questions about the data.

Lars also offers a couple systematic approaches to common problems. 

- For data visualization in general, he recognized this cycle. 
  1. Define the goal
  2. Source, shape and clean the data
  3. Draw the data
  4. Collect insight
  5. Refine goal
  6. Go back to step 1 if not satisfied

- For drawing data, Lars recognized this pattern.
  1. Sketch desired visualization
  2. Fetch and transform data
  3. Chart dimensions
  4. Calculate scales
  5. Join data and draw
  6. Add Axis 
  7. Refine drawing
