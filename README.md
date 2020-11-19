# Codeworks coding style guide

This is a reference to the style conventions that we use at [Codeworks](https://codeworks.me/).

## General

Set up your code editor to:

- Indent with 2 spaces.
- Use only spaces for indentation (no tabs).
- Use Unix [line endings](https://en.wikipedia.org/wiki/Newline).
- Avoid trailing whitespace.

Then make sure to respect correct indentation.

## HTML

- Write classes and ids in lowercase, separating words with dashes.
```html
<div class="my-class" id="my-id"></div>
```

## JavaScript

- Put semicolons at the end of your statements.
```js
// Bad
var letter = 'a'

// Good
var letter = 'a';
```
- Assign each variable on a separate line.
```js
// Bad
var letter = 'a', number = 1;

var letter = 'a',
    number = 1;

// Good
var letter = 'a';
var number = 1;
```
- Use "camel case" for variable naming (if it's for a class the first letter is uppercase). 
```js
// Bad
var myboolean = true;

// Good
var myBoolean = true;

function MyClass (name) {
  this.name = name;
}
```
- Be descriptive with your variable names.
```js
// Bad
var nos = 100;

// Good
var numberOfStudents = 100;
```
- Use function declarations, not expressions.
```js
// Bad
var hello = function () {
  console.log('hello');
};

// Good
function hello () {
  console.log('hello');
}
```
- Put a space before the parentheses when you write anonymous functions.
```js
// Bad
const callback = function(str) {
  console.log(str);
}

// Good
const callback = function (str) {
  console.log(str);
}
```
- Don't put a space before the parentheses when you write named functions.
```js
// Bad
function callback (str) => {
  console.log(str);
}

// Good
function callback(str) => {
  console.log(str);
}
```
- Put a space after `async` keyword for asynchronous functions.
```js
// Bad
const callback = async(str) => {
  await Promise.resolve(str);
}

// Good
const callback = async (str) => {
  await Promise.resolve(str);
}
```
- Put a space before blocks, and around keywords.
```js
// Bad
if (a){
  b();
}

if (foo) {
    //...
}else {
    //...
}

// Good
if (a) {
  b();
}

if (foo) {
    //...
} else {
    //...
}
```
- Use single quotes for strings.
```js
// Bad
var myString = "Hello world";

// Good
var myString = 'Hello world';
```
