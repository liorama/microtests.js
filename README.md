# What are Microtests
Microtests are tiny tests you add inline to your code. They test small bits of code, the smaller the better, optimally single expressions. Microtests run in your IDE (or other development environment) on code change so give you quick feedback when you break something.
## why? 
Three major reasons:
1. Catch small bugs immediatly, without running the full test suite.
2. Pinpoint the expression or line causing a test to fail easily.
3. Documentaion. Since microtests are incode tests they add lots of useful information on the expected behavior of the code.

# Microtests.js
Microtests.js is a basic tool to run microtests for Javascript. The plan is to have a library that handles takes the tested code, parses it and runs the tests. Then have that wrapped in plugins for VSCode and IntelliJ. We'll see where this will take us.

