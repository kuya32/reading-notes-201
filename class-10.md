# Read: 10 - JS Debugging

## JS Ch. 10, “Error Handling & Debugging”

- If you understand execution context (which have two stages) and stacks, you are more likely to find the error in your code.
  - Global context vs function context
  - Global scope vs function-level scope
    - **Global Scope** - a variable is declared outside a function, it can be used anywhere 
    - **Function-level scope** - a variable is declared within a function, it can only be used within that function
  - Understand the process when a statement needs data from another function, it **stacks** the new function on top of the current tasks. 
- Debugging is the process of finding errors. It invokes a process of deduction.
- The console helps narrow down the area in which the error is located, so you can try to find the exact error.
  - Other console methods
    - console.info()
      - Used for general information
    - console.warn()
      - Used for warning
    - console.error()
      - Used to hold errors
    - console.table()
      - Lets you output a table showing
        - Used for objects and arrays
  - Debugger keyword
    - Creates a breakpoint of JavaScript and calls a debugging function.
- Javascript has 7 different types of errors. Errors are shown and described on p. 460-461
  - Each creates its own error object, which can tell you its line number and gives a description of the error.
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements
  - Use them to give your users helpful feedback. 


[Back to README](README.md)