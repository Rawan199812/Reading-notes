## EJS Partials
**Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.**

For Example :

***Most of the web sites has the same navbar and the same footer, so insted of repeating the HTML DOM for the them inside each HTML page we can just put them in ejs files and include these files whereever we want.***

- Partials are like a function for reusing same HTML across multiple pages.

- Ypu cam use the same partials in different page using include function and then add it wherever you need it to be added to.

- We can use that for repititive elements such as header and footer.

- we can create partial files inside views/partials/nameOfThing.ejs and that file will contain only the thing that we want to reuse, like a navigation bar for example.

- Now we can use that file inside other HTML files by including them in the strawberry tags

- we can include a partial file with <%-include(partial_file_name)%> where we insert partial file name.

- And its that simple how we can easily add chunks of reusable elements using EJS,express and NodeJS!