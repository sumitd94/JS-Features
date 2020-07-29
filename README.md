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
> <b>Important</b>
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

## Imports & Exports

In all modern Javascript projects, we ususally split our codes in multiple files so that we can manage them easily.
To still access functionality in another file , we need to `export` (to make it available) and `import` (to get access).

I will walk you through this with examples, so that it will be clear.

we have two types of exports, `named` and `unnamed (default)`

#### default
``` JavaScript
export default ...;
```

#### named
``` JavaScript
export const someName = ...;
```

We can import `default` exports like 
``` JavaScript
import somenameofyourchoice '../path/to/jsfile';
```

> <b>Note:</b> Here somenameofyourchoice is totally up to you, you can use any name here.

<b>Named Exports</b> have to be imported by their name

``` JavaScript
import {someName} from '../path/to/jsfile';
```

One thing here we need to keep in mind is that, in one file we can have only 1 default export and an unlimited number of named exports.

> while using the keyword export, if we dont mention default keyword, it will automatically condider it as a named export

To read more about exports, check <a href="https://developer.mozilla.org/en-US/docs/web/javascript/reference/statements/export">here</a> \
To read more about imports, check <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import">here</a>