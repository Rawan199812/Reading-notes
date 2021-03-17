 # RESPONSIVE WEB DESIGN and FLOATS

***What is the responsive web design?***

build web pages that detect the visitor’s screen size and orientation and change the layout accordingly.

***What are the Responsive web design three main components?***

1. **Flexible Layouts:**

Flexible grid built using relative length units(percentages or em units).
**formula to help identify the proportions of a flexible layout using relative values:**

**target ÷ context = result**


2. **Media Queries:**
Feature of CSS that enable webpage content to adapt to different screen sizes and resolutions.

-  provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation.

- Media queries may be inserted within a webpage's HTML or included in a separate CSS file referenced by the webpage.

***There are three different logical operators available for use within media queries:***

- **And:** allows an extra condition to be added.
- **Not:** negates the query, specifying any query but the one identified.
- **Only:**new operator and is not recognized by user agents.

- The height and width features are based off the height and width of the viewport rendering area.

***The mobile first*** approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.


3. **Flexible Media:**for images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes(using the max-width property with a value of 100%).

- max-width property doesn’t work well around iframes and embedded media.


***What is “Float” and how we can use it?***
The float CSS property places an element on the left or right side of its container, allowing text and inline elements to wrap around it. The element is removed from the normal flow of the page, though still remaining a part of the flow.

***What are the four valid values for the float property?***

**Left** and **Right**(directions respectively) **None** (the default) **Inherit** (assume the float value from that elements parent element).

***We use floats for:***

1. Used to create entire web layouts.
2. for layout in smaller instances.

**Clear property**: we use it to not move up adjacent element to the float like the float desires, but will move itself down past the float.

***Clear values :***

- **Both**(clear floats from left and right)
- **Left**
- **Right** 
- **None** (default)


***Pushdown*** :is a symptom of an element inside a floated item being wider than the float itself .

