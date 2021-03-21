# 6 Reasons for Pair Programming

***Pair Programming increased code quality because it leads to clearer articulation of the complexities and hidden details in coding tasks, reducing the risk of error or going down blind alleys and it gives a better diffusion of knowledge among the team.***
- Pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together.

- Pair programming involves two roles : The Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. The Navigator uses their words to guide the driver but dose not provide ant direct input to the computer.

***What Is JQuery?***

**jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers. With a combination of versatility and extensibility, jQuery has changed the way that millions of people write JavaScript.**

**jQuery Features**

***Following are the important features of jQuery***

- HTML manipulation

- DOM manipulation

- DOM element selection

- CSS manipulation

- Effects and Animations

- Utilities

- AJAX

- HTML event methods

- JSON Parsing

- Extensibility through plug-ins.

1. Event Handling

***To handle DOM events using jQuery methods, first get the reference of DOM element(s) using jQuery selector and invoke appropriate jQuery event method.***

$('#saveBtn').click(function () { alert('Save button clicked'); });

<input type="button" value="Save" id="saveBtn" />

**Event Object**
- jQuery passes an event object to every event handler function. The event object includes important properties and methods for cross-browser consistency e.g. target, pageX, pageY, relatedTarget etc.

$('#saveBtn').click(function (eventObj) { alert('X =' + eventObj.pageX + ', Y =' + eventObj.pageY); });

<input type="button" value="Save" id="saveBtn" />

3. Hover Events jQuery provides various methods for mouse hover events e.g. mouseenter, mouseleave, mousemove, mouseover, mouseout and mouseup.

$('#myDiv').mouseenter(function (data) { $(this).css('background-color','green'); });

$('#myDiv').mouseleave(function (data) { $(this).css('background-color','red'); });

<div id="myDiv" style="width:100px;height:100px"> </div>

4. Event Bubbling.

$('div').click(function (event) { alert( event.target.tagName + ' clicked'); });

<div> <p> <span>This is span.</span> </p> </div>

- Get and Set Data Will only get first element in multi-select will set all the same also.

***How to include jquery from a CDN?***

- protocol relative URL
- 2 forward slashes
- starts with script
***Where to place them?***

**BEFORE CLOSING BODY TAG**

