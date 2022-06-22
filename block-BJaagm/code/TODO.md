1. What does thread of execution means in JavaScript?

Ans: Thread of execution means executing the code one line after another.

2. Where the JavaScript code gets executed?

Ans: javaScript Engine

3. What does context means in Global Execution Context?

Ans: Context means environment in which code executed.

4. When do you create a global execution context.

Ans: is the first execution context that gets created by javaScript engine whenever its running your code  for the first time.

5. Execution context consists of what all things?

Ans: Execution context consist of two part one where you going to store all the data, variable functions etc and another where execution happens things like operation, manipulation etc.

6. What are the different types of execution context?

Ans: Global Execution Context and  Function Execution Context.

7. When global and function execution context gets created?

Ans: GEC is the first execution context that gets created by javaScript engine whenever its running your code  for the first time. whereas FEC is gets created whenever you are executing any function.

8. Function execution gets created during function execution or while declaring a function.

Ans: During function execution. 


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](/img/1.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](/img/2.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](/img/3.jpg3.jpg)