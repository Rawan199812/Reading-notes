## From the Duckett HTML book:

### The ways in which people access the web:
1. Web Browser – like Firefox, Internet Explorer, Safari, Chrome, and Opera.
2. Web Server-special computers which host the website.
3. Screen Readers-used by people with visual impairments.
4. Devices -including desktop computers, laptops, tablets, and mobile phones.

- The web server that hosts the website we are visiting can be anywhere in the world.

## Dictionary 

|   word        | meaning                                               |
|---------------|-------------------------------------------------------|
|    DNS        |stands for Domain Name System.servers tell the browser |
|               |how to find the website                                |
|---------------|-------------------------------------------------------|
|     ISP       |Internet Service Provider                              |
|---------------|-------------------------------------------------------|
|   IP address  |a number of up to 12 digits separated by periods       |
|---------------|-------------------------------------------------------|


- Every device connected to the web has a unique IP address.

## Chapter 1: Structure

- When we add structure to a Word document to make it easier to understand. We use structure in the same way when writing web pages.
- To describe the structure of a web page, we add code to the words we want to appear on the page. (Like in HTML we use < h1 >, < p >..tags.)

***How HTML Uses Elements to Describe the Structure of Pages?***

- < h1 > we use for Main Heading.
- < p > paragraph we use it like introduction to the rest of the page.
- < h2 > we use for Sub-Heading.
- < p > another paragraph we use to help follow the structure of what is being written. 

- Tags tell us something about the information that located between the opening and closing tags.Example: < html > tag tell us that anything between it and </ html > tag is HTML code. 

![htmlimg](https://cdo-curriculum.s3.amazonaws.com/media/uploads/html_element.png)
As we see in the picture: p is stands for paragraph and the closing tag has a forward slash after the < symbol(less-than sign).

***Attributes*** provide additional information about the contents of an element. it require a name and a value.

***Why it's very easy to use attributes?***
Because the attribute name indicates what kind of extra information we are supplying.lang attribute is used to indicate the language used in this element.

***How to write attributes?***
In the opening tag we write the name + equals sign and a value between quotations marks. 

![attribute](https://lh6.googleusercontent.com/proxy/DO0VkpXWZ5V8JEfMCcxVbFWyPYCM6c95Dk0JBUbFcthp8qg4t-dpXpeBo27vf74GASsX5vNQ_WCTshzGUH3ceZruJORPmJckiuDgoTTHgzAXuw=s0-d)

- We see < head > element first (contains information about the page).

- Then comes the < body > element (Everything inside this element is shown inside the main browser window.)

- Anything written between the < title > tags will appear in the title bar (at the top of the browser window)

***Looking at how other sites are built helps a lot:*** we can look for the View menu in the browser, and select the option that says Source or View source.

## Chapter 8: Extra Markup

- There are several different versions of HTML. We use now HTML5 and we write < !DOCTYPE html >in the top to indicate that and to help the browser to render a page correctly.

### Comments

***How to add comments in HTML?***
We add the comment between these characters: <! --  -->

***Why it is a good idea to add comments to your code?***
- Comments will make it much easier to remember why I write the code in this why (beacons after a while we might have a questions about the code) 
- If we were working in a time its good to pass on notes to help anyone who is looking at the code understand it.
- Sometimes we use comments to stop that code from being displayed in the browser. For example if I want to test the code without a specific line and I don’t want to delete it I make it a comment.

### ID Attribute and Class Attribute


|        ID Attribute              |                Class Attribute           |
|----------------------------------|------------------------------------------|
|Every HTML element can carry the  |Every HTML element can carry the class    |
|id attribute                      |  attribute                               |
|----------------------------------|------------------------------------------|
|Is used to uniquely identify that |Is used to identify several elements as   |
|element from other elements on the|being different from the other            |
|elements on the page.             |elements on the page.                     |
|----------------------------------|------------------------------------------|
|no two elements on the same page  |The class attribute on any element can    |
|have the same value for their id  |share the same value.                     |
|attributes                        |                                          |
|----------------------------------|------------------------------------------|



***Inline elements and Block elements:***

#### There are two type of element in format: Inline elements and block elements.

- The inline element means when we write them they will appear to continue on the 
same line as their neighbouring elements.

- Block elements will always appear to start on a new line in the browser window.

***Why we use < div  >element?***

- To grouping text and elements in one block

- it's useful when we add CSS style to the page.

- make it easier to follow your code if we use <div> elements to hold each section of the page.

***Why we use < span > element?***

- To grouping text and elements inline.
- To control the appearance of the content of these elements using CSS.

### iframe
***Why we use < iframe > element?***

- To embed a Google Map into a page.

***There are some attributes we use with iframe:***

#### Src:
(source) specifies the URL of the page to show in the frame.

#### Height: 
specifies the height of the iframe in pixels (px).

#### Width: 
specifies the width of the iframe in pixels (px).

#### Scrolling:
indicates whether the iframe should have scrollbars or not. (not supported in HTML5)

#### Frameborder: 
indicates whether the frame should have a border or not.(not supported in HTML5) 

#### Seamless: 
we applied to an iframe where scrollbars are not desired.

- The < meta > tag allows you to supply all kinds of information about your web page.
- There are some characters that are used in and reserved by HTML code such as: (& copy;)  for copyright ©

## Chapter17:HTML5 Layout

- There are elements that allow us to divide up the parts of a page and make the code easier to follow. The names of these elements indicate the kind of content in them.


|  ##Element           |                       ##Used for                       |
|----------------------|--------------------------------------------------------|
|                      |The main header or footer that appears at the top or    || < header > < footer >|bottom of every page on the site and for an individual  ||                      |or within the page.                                     |
|----------------------|--------------------------------------------------------|
|                      |To contain the major navigational blocks on the site and||  Navigation < nav >  |some programmers use it for the links that appear at the||                      |bottom of every page.                                   |
|----------------------|--------------------------------------------------------|
|                      |A container for any section of a page that could stand  ||      < article >     |alone and potentially be syndicated and can be nested   | |                      |inside each other.                                      |
|----------------------|--------------------------------------------------------|
|                      |If it is inside an < article > element, it contain      | |                      |information that is related to the article but not      ||        < aside >     | essential to its overall meaning.                      |
|                      | If it is outside of < article >element, it acts as a   ||                      |container for content that is related to the entire page|
|----------------------|--------------------------------------------------------|
|                      |Groups related items together. It may contain several   ||      < section >     |distinct elements that have a common theme or purpose.  |
|                      |And sometimes to split the article up into separate     |
|                      |sections.                                               |
|----------------------|--------------------------------------------------------|
|     < hgroup >       |To group together a set of < h1> through< h6> |elements | |                      |so that they are treated as one single heading.         |
|----------------------|--------------------------------------------------------|
|     < figure >       |To contain any content that is referenced from the main |
|                      |flow of an article(like Images , Videos , Graphs..)     |
|----------------------|--------------------------------------------------------|

 

- Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements
Chapter18:Process & Design

#### We should know who we expect to use my website ( my audience)

- The audience can influence design decisions from color palettes to level of detail in descriptions. And we need to consider why People Visit my Website.
I have to figure out what information my visitors need and provide it to them.

- There are some sites people will visit a lot like news so I have to think of how many times people will open my website .

*Site map*: create a diagram of the pages that will be used to structure the site.

*Wireframe*: it shows how the page should look after we finished.
- Visual hierarchy helps visitors understand what you are trying to tell them.

- Headings Giving a chunk of information a heading clearly tells the user whether or not the content of the grouping is relevant to them.

## From the Duckett JS book:

### Introduction and chapter 1 

- JavaScript make the page feel interactive by responding to what the user does.
***Script:*** series of instructions that a computer can follow step by step to achieve a goal.

- When we state our goal and then list the tasks that need to be completed and break it down into smaller tasks, and learn one of these at a time. This way it seems simpler.

- We ca represent tasks using a Flowchart.

- Every step for every task shown in a flowchart needs to be written in a language the computer can understand and follow.

*Debugging*: several ways to discover what might have gone wrong
The flowcharts show the paths between each step.


***Objects:*** physical thing

***Properties:*** describe characteristics of the current web page ( characteristics of an object). Each one has a name and a value will tell us something about each individual instance of the object.

***Event ***

Programs are designed to do different things when users interact with the computer in different ways.( such as a user clicking or tapping on an element.)

***Methods:*** questions and instructions that tell us something about that object and change the value of the object's properties.

- Events can trigger methods, and methods can retrieve or update an object's properties.

***How JavaScript will fit together with the HTML and CSS in web pages?***

### Each language forms a separate layer with a different purpose:

*HTML:* Content Layer for( . html files)

*CSS:* Presentation Layer for(. css files)

*JavaScript:* Behavior Layer for ( .js files)
![img](http://qnimate.com/wp-content/uploads/2014/05/script-tag.jpg)

***How to write a script?***

We writ < script > and closing </ script > tags before the closing </ body > tag

- It is best to keep JavaScript code in its own JavaScript file.

- And we notice that the HTML is still exactly the same.(because the source of the web page does not actually show the new element that has been added into the page. it just shows the link to the JavaScript file.)







