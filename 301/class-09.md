## FUNCTIONAL PROGRAMMING

- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable datA

- If a function reads external files, it’s not a pure function — the file’s contents can change.

- Any function that relies on a random number generator cannot be pure.

**To know if a function is pure :**

- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects

**Pure functions benefits:**
The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

Given a parameter A → expect the function to return value B

Given a parameter C → expect the function to return value D


- toLowerCase: converts the string to all lower case trim: removes whitespace from both ends of a string split and join: replaces all instances of match with replacement in a given string

Filter
Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection. Basically, if the callback expression is true, the filter function will include the element in the result collection. Otherwise, it will not.
Map
The idea of map is to transform a collection.
The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.