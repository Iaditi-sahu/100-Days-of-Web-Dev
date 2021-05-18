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

# Data-type
We can put any type in a variable. For example, a variable can at one moment be a string and then store a number:
let msg = 'hello';
msg = 56789;

* Numbers
The number type represents both integer and floating point numbers.

There are many operations for numbers, e.g. multiplication *, division /, addition +, subtraction -, and so on.

Besides regular numbers, there are so-called “special numeric values” which also belong to this data type: Infinity, -Infinity and NaN.

In JavaScript, the “number” type cannot represent integer values larger than (2^53-1) (that’s 9007199254740991), or less than -(2^53-1) for negatives. It’s a technical limitation caused by their internal representation.

**Right now, BigInt is supported in Firefox/Chrome/Edge/Safari, but not in IE.

* String
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

* Boolean
As in other language Js booleans also hold true and false value.

* Null
In JavaScript, null is not a “reference to a non-existing object” or a “null pointer” like in some other languages.

It’s just a special value which represents “nothing”, “empty” or “value unknown”.

* Undefined
The special value undefined also stands apart. It makes a type of its own, just like null.

The meaning of undefined is “value is not assigned”.

*let age = 100;
 age = undefined; 
 alert(age);*

* object
The object type is special.

All other types are called “primitive” because their values can contain only a single thing (be it a string or a number or whatever). In contrast, objects are used to store collections of data and more complex entities.

Being that important, objects deserve a special treatment. We’ll deal with them later in the chapter Objects, after we learn more about primitives.

The symbol type is used to create unique identifiers for objects. We have to mention it here for the sake of completeness, but also postpone the details till we know objects.

* Summary
There are 8 basic data types in JavaScript.

number for numbers of any kind: integer or floating-point, integers are limited by ±(253-1).
bigint is for integer numbers of arbitrary length.
string for strings. A string may have zero or more characters, there’s no separate single-character type.
boolean for true/false.
null for unknown values – a standalone type that has a single value null.
undefined for unassigned values – a standalone type that has a single value undefined.
object for more complex data structures.
symbol for unique identifiers.
The typeof operator allows us to see which type is stored in a variable.

Two forms: typeof x or typeof(x).
Returns a string with the name of the type, like "string".
For null returns "object" – this is an error in the language, it’s not actually an object.

# Interaction: alert, prompt, confirm.
* alert
This one we’ve seen already. It shows a message and waits for the user to press “OK”.

alert('Hey!');

* prompt
The visitor can type something in the prompt input field and press OK. Then we get that text in the result. Or they can cancel the input by pressing Cancel or hitting the Esc key, then we get null as the result.

The call to prompt returns the text from the input field or null if the input was canceled.

let behave = prompt('How are you', ok);
alert(`Have a great day hope you are ${behave});

* confirm
The function confirm shows a modal window with a question and two buttons: OK and Cancel.

The result is true if OK is pressed and false otherwise.

let isPath = confirm('Is there a way');
alert(isPath);