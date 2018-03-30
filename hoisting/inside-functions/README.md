# Hoisting Inside a Function

This is a tricky bug because there is no way to figure it out logically by tracing the code.  You have to understand how JS declares and assigns variables at runtime in order to fix it.

### Index
* [Solution](#solution)
* [Buggy Code](#buggy-code)
* [Test Cases](#test-cases)
* [Fix](#fix)
* [Resources](#resources)
* [The Challenge](direct link to the challenge issue)

___

## Solution

It wasn't entirely clear what the bug was because I wasn't sure what the code was _supposed to_ do. 

So I took a guess that it was expected to print "global" and then "local".  To make it do this I removed the variable declaration inside of the _if_ statement so there wouldn't be an undefined myVar hoisted above the "local" value assignment.

[TOP](#hoisting-inside-a-function)
___

## Buggy Code

[import, 1.js](./bug.js)

[TOP](#hoisting-inside-a-function)

___

## Test Cases

[import, test-cases.js](./test-cases.js)

[TOP](#hoisting-inside-a-function)

___

## Fix


[import, fix.js](./fix.js)

[TOP](#hoisting-inside-a-function)

___


## Resources

* [A Guide to Hoisting](https://medium.freecodecamp.org/what-is-variable-hoisting-differentiating-between-var-let-and-const-in-es6-f1a70bb43d)



[TOP](#resources)

___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>