## Mustache.js with Node and Express

**Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.**

- It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.

Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn

**In the above, we see two braces around {{ name }}. This is Mustache syntax to show that it is a placeholder. When Mustache compiles this, it will look for the ‘name’ property in the object we pass in, and replace {{ name }} with the actual value, e,g, “Sherlynn”.**

## Flexbox

***Before the Flexbox Layout module, there were four layout modes:***

**Block, for sections in a webpage Inline, for text Table, for two-dimensional table data Positioned, for explicit position of an element The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.**

- The align-content property is used to align the flex lines. 
- The direct child elements of a flex container automatically becomes flexible (flex) items. 
- The align-self property specifies the alignment for the selected item inside the flexible container. 
- The align-self property overrides the default alignment set by the container’s align-items property.

**Display:**

***This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.***

**flex-direction**
- row (default): left to right in ltr; right to left in rtl
- row-reverse: right to left in ltr; left to right in rtl 
- column: same as row but top to bottom 
- column-reverse: same as row-reverse but bottom to top

**flex-wrap**

By default, flex items will all try to fit onto one line. To change that: 
- nowrap (default): all flex items will be on one line 
- wrap: flex items will wrap onto multiple lines, from top to bottom. 
- wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

***flex-flow a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.***

**justify-content:**

(flex start,flex-end,center,space-between,space-around and space-evenly)
and many others.


