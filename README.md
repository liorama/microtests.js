# What are Microtests
Microtests are tiny tests you add inline to your code. They test small bits of code, the smaller the better, optimally single expressions. Microtests run in your IDE (or other development environment) on code change so give you quick feedback when you break something.
## Why? 
Three major reasons:
1. Catch small bugs immediatly, without running the full test suite.
2. Pinpoint the expression or line causing a test to fail easily.
3. Documentaion. Since microtests are incode tests they add lots of useful information on the expected behavior of the code.

# Microtests.js
Microtests.js is a basic tool to run microtests for Javascript. The plan is to have a library that handles takes the tested code, parses it and runs the tests. Then have that wrapped in plugins for VSCode and IntelliJ. We'll see where this will take us.

## Example
A microtest can be added with a test comment (syntax is not set yet):

```

// Test a whole line against an assertion
const myVar = 2.5;  // microtest: assert myVar === true

// Test the expression is true with a given variable/argument value
myVar * 2 === 5  // microtest: assert true | myVar=2.5

// Test an expression within a line - this might be to horrible an idea
const someFunc = x => x^2 
alert(`result of someFunc is ${/*test>*/ someFunc(25) /*<test assert true*/}, wow right?`) 


```
