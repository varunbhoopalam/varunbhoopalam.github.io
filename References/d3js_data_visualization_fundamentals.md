Pluralsight course by Lars Verspohl

D3 is a low-level Javascript Library for manipulating the document object model(DOM) based on data. It's a collection of modules which revolve around the core abstraction of binding data to dom elements. It uses web technologies (HTML, SVG, CANVAS) to actually do the drawing in the DOM and helps manage configuration of these technologies. By binding data to dom elements, the dom elements can size, transform, shape, color themselves appropriately to the specification. A theme of the helper functions in some of it's modules is to scale data to the screen, for example turning dollars into pixel locations. Since D3 is a low-level library, it offers a lot of control of dom manipulation to the user.

Throughout the course, Lars touches on topics of making better choices through visual design. Often this is motivated by having the audience of the visualization to work less. Additionally he focuses on using SVG as the drawing tool. SVG defines a canvas of an absolute pixel length. This canvas accepts children elements like line, circle, and text. SVG offers the ability to group children together and apply transformations to the group.

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
6. Further refine data
