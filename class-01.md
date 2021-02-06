# From the Duckett HTML book:

### The ways in which people access the web:
1. Web Browser – like Firefox, Internet Explorer, Safari, Chrome, and Opera.
2. Web Server-special computers which host the website.
3. Screen Readers-used by people with visual impairments.
4. Devices -including desktop computers, laptops, tablets, and mobile phones.

- The web server that hosts the website we are visiting can be anywhere in the world.

## Dictionary 
|DNS       |stands for Domain Name System.servers tell the browser how to find the website |
| ISP      |Internet Service Provider                                                      |
|IP address|a number of up to 12 digits separated by periods / full stops.                 |

- Every device connected to the web has a unique IP address.
## Chapter 1: Structure
- When we add structure to a Word document to make it easier to understand. We use structure in the same way when writing web pages.
- To describe the structure of a web page, we add code to the words we want to appear on the page. (Like in HTML we use < h1 >, < p >..tags.)
***How HTML Uses Elements to Describe the Structure of Pages?***
< h1 > we use for Main Heading.
< p > paragraph we use it like introduction to the rest of the page.
< h2 > we use for Sub-Heading.
< p > another paragraph we use to help follow the structure of what is being written. 

- Tags tell us something about the information that located between the opening and closing tags.Example: < html > tag tell us that anything between it and </ html > tag is HTML code. 

![htmlimg](https://cdo-curriculum.s3.amazonaws.com/media/uploads/html_element.png)
As we see in the picture: p is stands for paragraph and the closing tag has a forward slash after the < symbol(less-than sign).

*Attributes* provide additional information about the contents of an element. it require a name and a value.

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








