## Call stack
***A call stack is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions what function is currently being run and what functions are called from within that function.***

**When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.**

- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.

- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.

- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
- we start with an empty Call Stack. Whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again.

***The JavaScript engine is a single threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.***

**Temporarily store: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack**

**Manage function invocation : The call stack maintains a record of the position of each stack frame. It knows the next function to be executed. This is what makes code execution in JavaScript synchronous.**

**stack overflow :A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.**

### JavaScript error messages
***Types of error messages:***

- Reference errors
- Syntax errors
- Type errors
- Range errors

**JS is not a compiled language like Java so your errors will happen at runtime, that means that you can only see whatever is wrong with your code after your run it.**

***Tools to avoid runtime errors:***

- quokka
- eslint
- TypeScript