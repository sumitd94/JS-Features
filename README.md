# Javascript Features

<b><u>Let & Const</u></b>

`let` and `const` basically replace `var`.
You use `let` instead of `var` , and `const` instead of `var` if you never plan to reassign this "Variable" (Meaning effectively turning it into a constant)

To Read more about this `let` Please visit <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let">here</a>

Also checkout about `const` <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const">here</a>

<b><u>Arrow Functions</u></b>

Arrow functions are a different way of creating functions in JavaScript.

It has a very simple syntax.

This normal JS Function <br />

```JavaScript
function callMe(name) {
    console.log(name);
}
```
becomes:
``` JavaScript
const callMe = (name) => {
    console.log(name)
}
```
<b>Important</b> \
When Having <b>No Arguments</b>, we have to use empty parentheses in the function declaration

Example :
``` JavaScript
const callMe = () => {
    console.log('Sumit')
}
```

If we have just arguments being passed to the function, we can write the functions as

``` JavaScript
const callMe = name => {
    return name;
}
```
So basically there is no need of parentheses, this only applies if there is exactly one arguments being passed. If there are more than one arguments or no arguments .. in that case the above will not make sense \
For Example , this will not work

``` JavaScript
const callMe = name,age => {
    return name;
}
```

If we want to return just a single line of code, then we can use the below syntax
``` JavaScript
const callMe = name => name
```
which is same as
``` Javascript
const callMe = (name) => {
    return name;
}
```
Please refer <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions">here</a> for more information

