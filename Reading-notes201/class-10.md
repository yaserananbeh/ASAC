# Error Handling & Debugging


### When we work with javascript there's an object that handle the error called (error object)
This object will be created to show us the error type , the error description and the script or the line that cause the error and the particular file that contain the error 

**Here some type of the errors**
- Syntax Error (This is caused by incorrect use of the rules of the language)
- Reference Error (This is caused by a variable that is not declared or is out of scope)
- Eval Error (INCORRECT USE OF eval() FUNCTION )
- URI Error (INCORRECT USE OF URI FUNCTIONS If these characters are not escaped in URls, they will cause an error: / ? & I : ; )
- Type Error (This is often caused by trying to use an object or method that does not exist. )
- Range Error (If you call a function using numbers outside of its accepted range. )
- Error (The GENERIC ERROR OBJECT )
- Nan (Actually its not an Error it's like datatype in the javascript but we will face it if we trying to do a mathimatical operation using two side one of them not a number )

### DEBUGGING is  eliminating potential causes of an error.

### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE 
The console is the developer friend we can use it to know where is , when and what the kind error we have 
### HANDLING EXCEPTIONS
We can use try , catch and finally to handle any error that we don't expect it 

## Summary 
- If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code. 
- Debugging is the process of finding errors. It involves a process of deduction. 
- The console helps narrow down the area in which the error is located, so you can try to find the exact error. 
- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error. 
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.