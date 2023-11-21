## Basics of Javascript

    In this chapter we will learn the basics to get started with Javascipt. This will be the best cheatsheet on the entire internet. So Stay tuned for the upcoming cheatsheets. Let's begin

### Variables

Variables are like containers to store values like numbers or strings, that can further be used in the code.

#### Varible declaration: var, `let` and `const`

In Javascript, there are 3 keywords that can be used to declare a variable, and each has its differences. Those are var, let and const.

##### Short explanation:

The varibles assigned using const can't be changed or reassigned, while let and var can.

<table>
  <tr>
    <th></th>
    <th>Scope</th>
    <th>Reassignable</th>
    <th>Mutable</th>
  </tr>
  <tr>
    <th>const</th>
    <td>Block</td>
    <td>No</td>
    <td>Yes</td>
  
  </tr>
  <tr>
    <th>let</th>
    <td>Block</td>
    <td>Yes</td>
    <td>Yes</td>
    
  </tr>
   <tr>
    <th>var</th>
    <td>Function</td>
    <td>Yes</td>
    <td>Yes</td>
   
  </tr>
</table>

#### Sample code

javascript
const person = "Nick";
person = "John" // Will raise an error, person can't be reassigned

javascript
let person = "Conor";
person = "Khabib";
console.log(person) // "Khabib", reassignment is allowed with let

### Data types

Data types are the different kinds of data we will be using and storing in variables.
It is divided into 2 categories - **Primitive** & **Reference** data types.
Certainly this table will help you understand much better.

| Data Type     | Type      | Uses                                     | Example                                   |
| ------------- | --------- | ---------------------------------------- | ----------------------------------------- |
| **Number**    | Primitive | Numeric values, integers or floats       | `let age = 25;`                           |
| **String**    | Primitive | Text                                     | `let name = "John Doe";`                  |
| **Boolean**   | Primitive | True or false values                     | `let isRaining = false;`                  |
| **Undefined** | Primitive | Default value of uninitialized variables | `let variable;`                           |
| **Null**      | Primitive | Represents the absence of a value        | `let absent = null;`                      |
| **Symbol**    | Primitive | Unique identifiers                       | `let key = Symbol('unique');`             |
| **Array**     | Reference | Ordered list of values                   | `let numbers = [1, 2, 3, 4, 5];`          |
| **Object**    | Reference | Collection of key-value pairs            | `let person = { name: "John", age: 25 };` |
| **Function**  | Reference | Reusable blocks of code                  | `let add = function () {};`               |

### Conditional Statements

Conditional statements allow your program to make decisions and execute different code blocks based on specified conditions. These are the types of conditional statements:

- if
- else
- else if
- switch

##### 1. **if** statement

It evaluates a condition, and if the condition is true, it executes a block of code.

Syntax:

```javascipt
if (condition) {
  //  block of code to be executed if the condition is true
}
```

Sample code:

```javascipt
if (hour < 18) {
  greeting = "Good day";
}
```

##### 2. **else** statement

The code gets executed if the condition is false.

Syntax:

```javascipt
if (condition) {
  //  block of code to be executed if the condition is true
} else {
  //  block of code to be executed if the condition is false
}
```

Sample code:

```javascipt
let age = 18;

if(age >= 18){
  console.log('You are an adult');
} else{
  console.log('You are a minor');
}
```

##### 3. **else if** statement

It is used to specify more than one conditions in the code.

Syntax:

```javascipt
if (condition1) {
  //  block of code to be executed if condition1 is true
} else if (condition2) {
  //  block of code to be executed if the condition1 is false and condition2 is true
} else {
  //  block of code to be executed if the condition1 is false and condition2 is false
}
```

Sample code:

```javascipt
let age = 18;

if(age < 0){
  console.log('You are not born yet');
} else if(age >= 18){
  console.log('You are an adult');
} else{
  console.log('You are a minor');
}
```

##### 4. **switch** statement

The `switch` statement is used when you have multiple conditions to check. It provides a cleaner way to write multiple `if-else` statements.

Syntax:

```javascipt
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

Sample code:

```javascipt
let day = "Monday";

switch (day) {
  case "Monday":
    console.log("It's the start of the week.");
    break;
  case "Friday":
    console.log("TGIF! It's Friday.");
    break;
  default:
    console.log("It's a regular day.");
}

// In this example, it checks the value of the `day` variable and prints a message based on the day.
```

Note: Ternary Operator?

### Loops

Loops are used to run the same code again and again, each time with a different value.
Types of loops are:

- **for** loop
- **while** loop
- **do-while** loop
- **forEach**
- **forin**
