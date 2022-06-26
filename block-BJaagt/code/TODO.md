Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `username`. Where `username` define inside the block using the keyword `const`. const create scope where it is define inside the block so we are not able to access it because it is define using `const`inside the block.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
In above code we are again looking for the variable named `username`. Where `username` define inside `if`. Where `if` is a block and we are using the keyword `let` to create variable and `let create scope inside the block. So we will not to able the access to this code snippet.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```
In above code we are again looking for the variable named `username`. Where `username` define inside `if`. Where `if` is a block and we are using the keyword `var` to create variable and `var` does not create scope inside the block. So we will able to access the above code snippet.

The above code will throw an output `Arya`.


5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```
In above code we are again looking for the variable named `username`. Where `username` define inside `if`. But there is two keyword `let` and `var` two create variable in the same scope because `var` does not create scope inside block So it can we consider outside so in this case we are defining two variable name username in a same scope  thats why its throw an error

The above code will throw an error `username has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
In above code we are again looking for the variable named `username`. Where `username` define inside `if`. But there is two variable name `username` create with same keyword `let` where one is outside of block and another is inside the block so we know `let` is  create scope inside the block so this code snippet work properly and output will be "john" because "john" is in global scope.

The above code will throw an output `John`.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // output
```
In above code we are again looking for the variable named `username`. and we are calling the function "sayHello" calling the function will not do anything because execution context for this function is get created and deleted as soon as execution is over so here the value of `username` is "john".

The above code will throw an output `John`.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 9
}
console.log(i, 'Second'); // 10
```
In above code snippet we are defining the variable inside loop using keyword using `var` and we know `var` does not create scope in a block so we can think `var` i declare outside so in that case the value of i will be the last value and the last value of i is 10

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
In above code snippet we are defining the variable inside loop using keyword using `let` and we know `let` does create scope in a block so we can think `let` i does not declare outside so in that case the value of i will be the last value for inside the block and the last value of i is 9.