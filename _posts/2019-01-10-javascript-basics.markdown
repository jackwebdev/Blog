---
layout: post
title:  "JavaScript Basics"
date:   2019-01-10 09:22:09 GMT
categories: JavaScript
image: "/Blog/assets/images/javascript.png"
---

## Primitive Data Types
Data types are special data items that values can accept. JavaScript has ​six primitive data types​:

| Data Type     | Definition                                                                                     | Example             |
| ------------- |:----------------------------------------------------------------------------------------------:| -------------------:|
| Boolean       | Represents possible values that true or false                                                  | `true` or `false`   |
| Number        | A number integer or floating-point.                                                            | `26`                |
| String        | A sequence of characters.                                                                      | `"Hello World!"    `|
| Undefined     | A variable that hasn't been assigned a value. Not a good idea to set a variable to undefined.  | `undefined`         |  
| Null          | It is explicitly nothing, safer to set a variable to null.                                     | `null`              |  
| Symbol        | New to ES6. Immutable primitive value that is unique. A value that always changes.             | `Symbol(26)`        |  

## Variables
A good explanation of a variable is explained in [Eloquent JavaScript](https://eloquentjavascript.net/02_program_structure.html){:target="_blank"} book:
> You should imagine bindings as tentacles, rather than boxes. They do not contain values; they grasp them.

Let's start with the basics. We declare a variable called `helloWorld`. `"Hello World!"` is a string that is now binded inside of `helloWorld`.
```javascript
let helloWorld = "Hello World!" 
```
Now let's print this to the console. To print to the console type `console.log()`, any code put inside the parentheses are printed. The comment which starts with `//` is how I will represent console printing. Comments are a way of leaving labels and notes in your code.
```javascript
console.log(helloWorld);
//Hello World!
```
JavaScript is dynamically typed language, this will allow me to change the value at runtime. You can now see that the variable “grasps” hold of the new number value. This is also an example of how **Coercion** works as we can change the data type from a `String` to a `Number`.
```javascript
helloWorld = 26;
console.log(helloWorld);
//26
```
### `Var`, `Let` and `Const`
ES6 introduced `let` and `const` keywords. Here are the main differences. 

`var`: When not declared inside a function, the variable is accessed anywhere in the code. When inside a function it's accessed anywhere inside that function.

`let`: Very similar to `var`. Only accessible inside its local scope. 

`const`: Often declared in capitals to reminds us it's a constant and can't be reassigned, Works like `let`. 

## Operators
There are many different types of operators. Here are the following operators:
- Arithmetic Operators
- Comparison Operators
- Logical (or Relational) Operators
- Assignment Operators
- Conditional (or ternary) Operators



### Arithmetic Operators
Arithmetic Operators allow us to perform mathematical functions.

#### Operand VS Operator
```
44 + 20
```
The operand is the `numbers` and the operator is the `+`.

#### Unary VS Binary Operator
Unary operation​: Only 1 Operand.
Binary operator​: 2 Operands are manipulated to return a result. Such as `44 + 20`.

#### Here are the Arithmetic Operators 
In the examples `let x = 3`

| Name                   | Definition                                                                                                                    | Example.                          |
| -----------------------|:-----------------------------------------------------------------------------------------------------------------------------:| ---------------------------------:|
| Before / After Increment | Depending if you put the operand before the `++` or after. `x++` sets x to 2. `++x` returns and sets to 4.                    |` x++ //4 ++x //4`                 |                                                                         
| Before / After Increment | Depending if you put the operand before the `--` or after. `x--`sets x to 2. `--x` returns and sets to 2.                     |` x-- //2 --x //2`                 |   
| Unary Negation         | Returns the negative value of the operand. x = 3​, ​-x​ returns​ ​-3.                                                              |`-x `                              |   
| Unary Plus             | Will try to convert the operand to a number.                                                                                      |`+false //1 +5 //5`                |   
| Remainder              | Returns the remainder from dividing 2 operands. `12​ ​%​ ​5​ ​=​ ​2 `  5 * 2 = 10 and we have a remainder 2.                          |`12​ ​%​ ​5​ ​=​ ​2 `                      |   

### Comparison Operators
Compare operands that return a boolean (true or false).

|Name                  | Notation            |
|---------------------:|--------------------:|
|Equal                 |`myVar == 0`         |
|Not Equal             |`myVar != 0 `        |
|Greather Than         |`myVar > 0`          |
|Greater Than Or Equal |`myVar >= 0`         |
|Less Than             |`myVar < 0 `         |
|Less Than Or Equal    |`myVar <= 0 `        |
|Strict Equal          |`myVar === 0`        |
|Strict Not Equal      |`myVar !== 0`        |

The main difference between `==` and `===` is type conversion. The Equal Operator `==` will compare if the two operands are the same type. It's safer to stick to Strict Equal `===`.

Here is a simple example of an if statement that runs "This is True!" if the statement is true, as you can see we get different results as Equal `==` will convert the appropriate type in order to compare. The if/else statement executes a block of code if the condition is true, else the else code block will run. 

You will find out more about if statements down the bottom of this article.
```javascript
let myVar = 0;

if(myVar == "0") {
    console.log("This is True!");
} else {
    console.log("This is False!");
}
//This is True!

if(myVar === "0") {
    console.log("This is True!");
} else {
    console.log("This is False!");
}
//This is False!

```

### Logical Operators
Logical Operators may return a boolean value.

**Truthy**: All values are truthy unless they are defined as falsy.

**Falsy**: Evaluate if the value is false. Example of these values: `null, undefined, NaN, 0, "" and false`. (`NaN` means Not a Number).

`Number(0)` is **Truthy**.

`Boolean(false)` is **Falsy**.

|Name                  |Definition                                                                           |Notation                 |
|---------------------:|------------------------------------------------------------------------------------:|------------------------:|
|And                   |Returns `true` if both given operands are `true`                                     |`myVarOne && myVarTwo`   |
|Or                    |Returns `true` if one of the given operands are `true`                               |`myVarOne || myVarTwo`   |
|Not                   |Returns `false` if the operand can be converted to true. Or `false` if it's `true`   |`!myVarOne`              |


### Assignment Operators

Assign a value to the operand on the left.

`x` and `y` are the operands. They both grasp onto the value 5. I then tell JavaScript to add them together using the `x += y` shorthand operator as it's less code compared to the longhand operator of `x = x + y`.
```javascript
let y = 5;
let x = 5;
x += y;

console.log(x)
//10
```

|Name            | Longhand Operator          | Shorthand Opeartor |         
|---------------:|---------------------------:|--------------------|
|Assignment      |`x = y`                     |`x = y`             |
|Addition        |`x = x + y`                 |`x += y`            |
|Subtraction     |`x = x - y`                 |`x -= y`            |
|Multiplication  |`x = x * y`                 |`x *= y`            |
|Division        |`x = x / y`                 |`x /= y`            |
|Remainder       |`x = x % y`                 |`x %= y`            |
|Exponentiation  |`x = x ** y`                |`x %= y`            |


## Conditional (or Ternary) Operators
You may have heard of an if statement, as mentioned above in this article. This is also known as a **Conditional** statement. 
You need your code to be able to make choices, like them game books where you pick your own path.

### `If`, `Else` and `Else If `
The example below is an example of how the syntax looks for an if statement. It's pretty straightforward and in plain English, it reads: If condition is `true` run the first code block, else it must be `false` return the second code block.

```javascript 
if(condition) {
    //Run this code block as it's true!
} else {
    //The condition is not true, this code block will return instead!
}
```

Now it's time to add the `else if` keyword. This is a good way to add another option to your code. For example, we need to check if the students have a pass, merit, distinction or have failed the assignment.

`studentMark` is a variable and holds the data of the student's grade. The if statement will now tell me what their grade is. 

#### How the code works:
The student has received a `Distinction`, If the `studentMark` is a `Pass`, `false`, move on, If the `studentMark` is a `Merit`, `false`, move on, If the `studentMark` is a `Distinction`, `true`, execute the code block!

Lets change the `StudentMark` to `StudentMark =  "Fail"`. We never told the if statement what to do if they failed. The if statement will check the `if` and `else if` parts to see if it matches `true`, but no matches, it must be `false` and the  `else` statement code block is executed.

```javascript 
let studentMark = "Distinction";

if(studentMark === "Pass"){
    console.log("The student has a pass grade.");
} else if (studentMark === "Merit") {
    console.log("The student has a merit grade;");
} else if (studentMark === "Distinction") {
    console.log("The student has a distinction grade.");
} else {
    console.log("This student has no grade and failed.")
}
```

### Ternary Operator
Think of the Ternary Operator as a shorter version of an if statement.

```javascript
let myVar = condition ? val1 : val2
```
