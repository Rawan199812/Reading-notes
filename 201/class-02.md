### From the Duckett HTML book:

## Chapter 2: Text
- Structural markup: the elements we use to describe headings and paragraphs

- Semantic markup: elements that are not intended to affect the structure of our web pages, but they add extra information.

+ Examples: <em> we use to indicate where emphasis should be placed on selected words and the <blockquote>element which indicates that a block of text is a quotation.

### There are six levels of headings HTML .the largest one and have more important in <h1>and <h2> is less and so on.

- < p > we use to create a paragraph

- < b >make characters appear bold.

- < i > make characters appear italic.

- < sup > characters that should be superscript.

- < sub > contain characters that should be subscript.


***White space collapsing:*** adding  extra spaces or start some elements on new lines to make code easier to read.

- < br /> to line break we use it inside the middle of a paragraph.

- < hr /> To create a break between themes.

***Empty elements:*** elements do not have any words between an opening and closing tag.

### There are two views of the page we are creating: 

- visual editor (resemble word processors)

- code view(show you the code created by the visual edito)



- < strong> indicates that its content has strong importance.
- < em> indicates emphasis that subtly changes the meaning of a sentence.

### There are 2 elements used for marking up quotations:

1. < blockquote > used for longer quotes.
2. < q > used for shorter quotes (Internet Explorer does not therefore many people avoid using the element.)
- < abbr > Abbreviations.

- < cite > indicate where the citation is from.

- < dfn > used to indicate the defining instance of a new term.

- < address > to contain contact details for the author of the page.

- < ins > to show content that has been inserted into a document.

- < del > to show text that has been deleted from it.
 
-  < s > element indicates something that is no longer accurate or relevant.

## Chapter 10:Introducing CSS

- CSS allows us to create rules that control the way that each individual box is presented.

### CSS rule contains two parts:  

1. Selectors: indicate which element the rule applies to.

2. Declarations: indicate how the elements referred to in the selector should be styled.

![imgcss](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics/css-declaration-small.png)

*Properties:* indicate the aspects of the element we want to change.

*Values:* specify the settings we want to use for the chosen properties.

### There are many ways to use CSS :

#### External

( we write inside the head in the html file the link of the CSS file and we write all the css in this file. )

***We use to do that:***

- *< link >* element 

- *href* to show the path

- *type* attribute specifies the type of document being linked to.

- *rel* specifies the relationship between the HTML page and the file it is linked to.

#### Internal

(We write within an HTML page by placing them inside a < style >inside the < head > of the page.)

- CSS selector allow us to target rules to specific elements in an HTML document

***If there are two rules that apply to the same element, which will take precedence?***

- *** The second selector ***(If the two selectors are identical, the latter of the two will take precedence)

- ***The more specific rule*** (If one selector is more specific than the others).

- ***The more important rule**

*Inheritance:*  save us from having to apply properties to as many elements

***Why it's better (good practice) to use External Style Sheets?***

- All of web pages can share the same style sheet.

- Once the user has downloaded the CSS stylesheet, the rest of the site will load faster.

- If we want to make a change we only need to edit the CSS file and all pages will be updated.

- The HTML code will be easier to read and edit because it does not have lots of CSS rules in the same document.


### From the Duckett JS book:

## Chapter 2: Basic JavaScript Instructions

*Statement:* instruction that a computer can follow and each one starts in a new line

- Statements can be organized into Code block (Each code block could contain many more statements)


***Why we write comments?***

- To explain what the code does.

- To help make code easier to read and understand.

- To help me and others who read your code.


### There are two types of JS comments:

- Multi-line comment (/**/)we use to write a comment that stretches over more than one line.

- single-line comment(//)anything that follows the two forward slash on that line will consider as comment

- We stored the data in a variable.it can change each time a script runs.


![imgJS](https://www.tektutorialshub.com/wp-content/uploads/2019/08/Declaring-the-Variable-in-Typescript.png)

### DATA TYPES:

- Strings (letters and other characters.)

- Numbers

- Boolean (two values: true or false.)

- We can change what is stored in the variable later in the same script.

***Array:*** a special type of variable stores a list of values.

- There are three methods to create an array. The difference is that we use square brackets [ ] for arrays instead of curly braces { }.

![new](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2019/08/how-to-create-JavaScript-array.jpg)

- we can change the value of an item an array by selecting it and assigning it a new using the equals sign and the new value for that item.

*expression* evaluates into a single value.


### There are two types of expressions:

1. Expressions that just assign a value To a Variable.

2. Expressions that use two or more value to return a signal value.



- Expressions rely on operators to calculate a value.

***Operators:*** allow programmers to create a single value from one or more values.

- ***Arithmetic operators*** (mathematical operators we use with numbers.)

- ***String operator:*** (+ symbol)

- ***Concatenation:*** joining together two or more strings to create one new string.


## Chapter 4: Decisions and Loops

- The code can take more than one path, which means the browser runs different code in different situations.


![home](https://www.sitesbay.com/javascript/images/if-statement.png)


- When we compare two values using string the result will be in True or False (Boolean).

- == Compare the value only (is equal to)

- === Compare the value and the datatype 

- !=  compare two values to see if there not the same (is not equal to) 

- !== compare two values to check if datatype and the value are not the same (strict not equal to)

* Evaluating the condition: testing or checking of a condition

*	Every value can be treated as true or false even if it is not a Boolean

*	In short circle evaluation a condition might not need to run.

*	The enclosing brackets are important when the expression is used as a condition in comparison operators.



#### To compare the results of more than one comparison operator

- Sometimes we don’t need to evaluate the hole condition.

Ex: False && (true /False) always will be false. 



#### If ... e1se statement allows you to provide two sets of code: 

1. One set if the condition evaluates to true 
2. Another set if the condition is false



