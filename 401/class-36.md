Iterators
Iterators provide a sequence interface to Python objects that’s memory efficient and considered Pythonic. Behold the beauty of the for-in loop!

To support iteration an object needs to implement the iterator protocol by providing the iter and next dunder methods.

Class-based iterators are only one way to write iterable objects in Python. Also consider generators and generator expressions.

***What Are Python Generators?***

Generators are a tricky subject in Python.generators look like regular functions but instead of using the return statement, they use yield to pass data back to the caller.

- Generator functions are syntactic sugar for writing objects that support the iterator protocol. Generators abstract away much of the boilerplate code needed when writing class-based iterators.
- The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
- Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.