# 'Use Strict'
    Used to include modern behavior of JS i.e ECMA script features.
    It mast be included at the top of Js file in order to apply it.

# Variable in JS
    Most of the time, a JavaScript application needs to work with information. Here are two examples:

    An online shop – the information might include goods being sold and a shopping cart.
    A chat application – the information might include users, messages, and much more.

    Variables are used to store this information.

    The var keyword is almost the same as let. It also declares a variable, but in a slightly different, “old-school” way.

    var message = 'Hello';
    * For instance, the variable message can be imagined as a box labeled "message" with the value "Hello!" in it.

 Naming conventitons
    The name must contain only letters, digits, or the symbols $ and _.
    The first character must not be a digit.

    Examples:- Wrong way of naming. 
            let 1a; // cannot start with a digit

            let my-name; // hyphens '-' aren't allowed in the name

            can not name keywords like let let = 7;

Normally, we need to define a variable before using it. But in the old times, it was technically possible to create a variable by a mere assignment of the value without using let. This still works now if we don’t put use strict in our scripts to maintain compatibility with old scripts.
* Constant
To declare a constant (unchanging) variable, use const instead of let:
const birthday = '31.07.1998';
They cannot be reassigned. An attempt to do so would cause an error

* Summary
We can declare variables to store data by using the var, let, or const keywords.

let – is a modern variable declaration.
var – is an old-school variable declaration. Normally we don’t use it at all, but we’ll cover subtle differences from let in the chapter The old "var", just in case you need them.
const – is like let, but the value of the variable can’t be changed.
Variables should be named in a way that allows us to easily understand what’s inside them.

* Data-type
We can put any type in a variable. For example, a variable can at one moment be a string and then store a number:
let msg = 'hello';
msg = 56789;

String
A string in JavaScript must be surrounded by quotes.

let str = "Hello";
let str2 = 'Single quotes are ok too';
let phrase = `can embed another ${str}`;
In JavaScript, there are 3 types of quotes.

Double quotes: "Hello".
Single quotes: 'Hello'.
Backticks: `Hello`.
Double and single quotes are “simple” quotes. There’s practically no difference between them in JavaScript.

Backticks are “extended functionality” quotes. They allow us to embed variables and expressions into a string by wrapping them in ${…}, for example.
let name = "John";

// embed a variable
alert( `Hello, ${name}!` ); // Hello, John!

// embed an expression
alert( `the result is ${1 + 2}` ); // the result is 3

