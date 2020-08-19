# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-09) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-11)

## error handling and debugging

Debugging is the process of finding errors. It involves a process of deduction.
JavaScript has 7 different types of errors that create error objects:

* Error : generic error.
* syntax error: syntax not followed
* reference error : reference an undeclared variable (or not in scope).
* type error : unexpected data type.
* range error: numbers not in accepted range
* URI error: encodeURI() and similar methods not used correctly
* eval error : eval() used incorrectly

error objects show the line where the error occured and a message.

debugging can be done by using the developer tools (the console specifically) in the browser.

You can pause the execution of a script on any line using breakpoints.
you can add them from the resourses tab in the dev tools **OR** using the
debugger keyword in the code.
