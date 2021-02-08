#### From the Duckett JS book:


***Array:*** a special type of variable stores a list of values.

- There are three methods to create an array. The difference is that we use square brackets [ ] for arrays instead of curly braces { }.

- we can change the value of an item an array by selecting it and assigning it a new using the equals sign and the new value for that item.

*expression* evaluates into a single value.

### The Switch Statement

- we use the switch statement to select one of many code blocks to be executed.

- switch statements allow you to compare a value against possible outcomes. 


***How switch statement works?***

- The switch expression is evaluated once.

- The value of the expression is compared with the values of each case.

- If there is a match, the associated block of code is executed.

- If there is no match, the default code block is executed.



*** default** specifies the code to run if there is no case match (like else in if statment)

### Type coercion :
convert data types behind the scenes to complete an operation.

- *Falsy* values are treated as if they are false and *Truthy* values are treated as if they are true. 

***Why logical operators will not always return true or false?***

because they return the value that stopped processing.And that value might have been treated as truthy or falsy although it was not a Boolean.

### Loops

***There are 3 types of loops:***

1. While loop ( the loop will continue run for as long as the condition in parentheses is true)
2. for loop(loops through a block of code a number of times)
3. Do while loop 



![loop](https://cdn.javascripttutorial.net/wp-content/uploads/2020/01/JavaScript-for-Loop.png)


### How we write a for loop? 


1. Initialization (The initialization expression is executed only once when the loop starts.)

2. Condition (The statement inside the loop is executed only when the condition evaluates to true. The loop is terminated if the condition evaluates to false.)

3. Post-expression



***Infinite loop:*** the code will not stop running until the browser runs out of memory.


#### From the Duckett HTML book:


- The ordered list is created with the < ol > element and each item in the list is placed between an opening < li > tag
and < /li > tag.

- The unordered list is created with the < ul > element and each item in the list is placedbetween an opening < li > tag and  < /li > tag.

- Definition lists are used to define terminology.

- We can put a second list inside an < li > element to create a sublist or nested list. 


#### Chapter 13: Boxes

***Properties that can be adjusted to control its appearance:***
1. Border
 (specified to be 0 pixels wide)The border separates the edge of one box from another.

2. Margin

(we can set the width of a margin to create a gap between the borders of two adjacent boxes.)


3. Padding

(the space betweenthe border of a box and any content contained within it.)

- To center a box on the page we can set the left-margin and right-margin to auto.

- The display (to turn an inline element into a block-level element or vice versa, and can also be use to hide an element from the page)

- The visibility to hide boxes from users but It leaves a space where the element would have been.

- The border-image property applies an image to the border of any box.

![border](https://i2.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/03/border-radius.JPG.png?resize=640%2C281&ssl=1)

- CSS3 introduces the ability to create rounded corners on any box using a  calledborder-radius

- border-radius(we can specify different distances for the horizontal and the vertical parts of the rounded corners.)











