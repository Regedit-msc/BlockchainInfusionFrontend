## GIT

### What is Git?

Git is a Version control System that runs locally on your PC. Bacically it keeps track of changes to your files in versions after each commit so you can rollback, etc. It has other powerful features like branches, ability to view diffs, merging, rebasing etc. It saves you the effort of having to keep track of your code changes manually by duplicating folders/entire projects and versioning them yourself.

- Check if git is installed on your PC. Run `git -v`. If there are no errors. It's installed else visit [git website](https://git-scm.com/downloads) and follow the instructons to download it for your operating system.

## Basic GIT commands

- `git init`: This initializes git in a folder.

- `git add <directory to monitor within folder>`: This tells git what directory to monitor within the folder.

- `git commit -m <commit message>`: This tells git to create a new version for the changes you just made.

- `git remote add <remote name> <remote url>`: This tells git to add a remote which you can push changes to subsequently alongside the versions (Basically copies your folder alongside the versions that git has on tyour local machine and keeps them online so you can use later haowever you like).

- `git log`: See all your versions of your folder changes.

- `git clone <remote url>`: Gets you the folder of a hosted repository from a remote you have previously set up.

## JAVASCRIPT

### What is JavaScript?

Fisrt off, JavaScript is not Java. JavaScript is an interpreted language that **originated** on the web to add functionality to webpages. Nowadays, JavaScript has evolved to run on other platforms outside the web, e.g Mobile (React Native, Ionic, Cordova), Desktop (Electron), on the server (Node.js Runtime, Deno), etc.

### BASICS OF JAVASCRIPT

#### DATA TYPES/PRIMITIVES IN JAVASCRIPT

- `string`: You can think of a string as a word/sentence. It is characterized and denoted by single or double quotes in your code/program.
  e.g:
  ```js
  "This is a string";
  "This is also a string";
  ```
- `number`: This are numeric values used in your code used for computation. e.g:
  ```js
  4;
  5;
  ```
- `boolean`: This represents `true` or `false`. e.g:
  ```js
  true;
  false;
  ```
- `object`: This is used to represent a collection of data in **key-value** pairs. e.g:

```js
 {
    name: "Sola",
    age: 23,
    gender: "Male",
    address: {
      postalCode: "100001",
      state: "Enugu"
    },
    hobbies: ["Cooking", "Eating", "Jumping"]
 }
```

- `array`: Similar to an `object`, it can hold a collection of data but not in **key-value** pairs. e.g:

```js
[
  "Tola",
  23,
  {
    name: "Sola",
    age: 23,
    gender: "Male",
    address: {
      postalCode: "100001",
      state: "Enugu",
    },
  },
  ["One", "Two"],
  [1, 2, 3, 4],
];
```

#### STRUCTURES AND OPERATORS IN JAVASCRIPT

##### STRUCTURES

- `Comment`: This is used to explain or hide code from the interpreter. Bacically anything **commented out** is not regarded as valid code by the interpreter.

- `Variables`: This are used as temporary stores of data for our code.

  In JavaScript we have two mainstream ways of declaring variables.

  - `const`: Used for **constant** variables that do not change (only mutable for _object_ data types).

  - `let`: It is mutable within the program context.

- `Functions`: This enables reuse of logic across code.

##### OPERATORS

- `addition`: This is denoted by the **+** sign, used to add two data types.

- `subtraction`: This is denoted by **-** sign, used to subtract numbers.

- `multiplication`: This is denoted by **\*** sign, used to multiply numbers.

- `division`: This is denoted by **/** sign, used to divide numbers.

- `assignment`: This is denoted by **=** sign, used to assign a value to a **variable**.

- `equality`: This is denoted by **==** sign, used to determine if two values are equal (P.S does not do strict equal or deep equal use `===` for strict equal).

#### EXAMPLES:

```js
const name = "Samuel";
name = "Ayo"; // This will error.

let name1 = "Ayomide";
name1 = "Samuel"; // This will not error;

// This is a comment

// FUNCTION
// It takes in two parameters firstNumber and secondNumber
function addTwoNumbers(firstNumber, secondNumber) {
  console.log(firstNumber + secondNumber); // console.log() is used to output to the console the content of the parenthesis.
}

addTwoNumbers(2, 4); // This is the act of invoking a function.
addTwoNumbers(2, 3); // This is the act of invoking a function.
```

#### LOOPS IN JAVASCRIPT

##### What is a Loop?

A **Loop** is exactly what you think it is, basically it's something that runs **repeatedly** given a **certain condition**. In JavaScript we have two kinds of loops mainly. **for** and **while** (P.S we have various derivatives of these loops in `for...in`,` for...of`, etc.).

##### FOR

```js
// ANATOMY

for (initialState; condition; whatToDoAfterEachIteration) {
  // What To do If the condition is true.
}

// EXAMPLE
const myNumber = 10;
for (let initialValue = 0; initialValue < myNumber; initialValue++) {
  console.log(initialValue);
}

// P.S
//  myNumber--  is the same as myNumber = myNumber - 1;
// initialValue++ is the same as initialValue = initialValue + 1;
```

##### WHILE

```js
// ANATOMY

while (condition) {
  // What To do If the condition is true.
}

// EXAMPLE
// This will keep running until the process is terminated
while (1 < 2) {
  console.log("Yes it is");
}

const myNumber = 10;
let initialValue = 0;
while (initialValue < myNumber) {
  console.log(initialValue);
  initialValue++;
}
```

##### CONTROL FLOW IN JAVASCRIPT

We have four major ways of handling control flow in JavaScript using some **keywords** which are `if`, `else`, `else if`, `switch`;

```js
// ANATOMY
if (condition) {
  // If condition is true
}

// EXAMPLE
if (6 > 5) {
  console.log("yes");
}

// ANATOMY
if (condition) {
  // If condition is true
} else {
  // Run this if condition is not true
}

// EXAMPLE
if (6 > 7) {
  console.log("yes");
} else {
  console.log("no");
}

// ANATOMY
if (condition) {
  // If condition is true
} else if (condition) {
  // Will be checked if the condition in `if` is not true.
} else {
  // Run this if none of the conditions is true.
}

// EXAMPLE
if (6 > 7) {
  console.log("yes");
} else if (9 > 8) {
  console.log("yes");
} else {
  console.log("no");
}

// ANATOMY
switch (value) {
  case condition:
    break;
  default:
    break;
}


// EXAMPLE
let gender = "preferNotToSay";
switch (gender) {
  case "male":
    console.log("male");
    break;
  case "preferNotToSay":
    console.log("preferNotToSay");
    break;
  default:
    console.log("female");
    break;
}
```
