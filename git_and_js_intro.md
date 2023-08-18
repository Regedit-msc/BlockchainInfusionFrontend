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

- `Comment`: This is used to explain or hide code from the interpreter.Bacically anything **commented out** is not regarded as valid code by the interpreter.


- `Variables`: This are used as temporary stores of data for our code.

  In JavaScript we have two ways of declearing variables.

  - `const`: Used for **constant** variables that do not change (only mutable for _object_ data types).

  - `let`: It is mutable within the program context.

- `Functions`: This enables reuse of logic across code.

##### OPERATORS

- `addition`: This is denoted by the **+** sign, used to add two data types.

- `subtraction`: This is denoted by **-** sign, used to subtract numbers.

- `multiplication`: This is denoted by __*__ sign, used to multiply numbers.


- `division`: This is denoted by __/__ sign, used to divide numbers.


- `assignment`: This is denoted by __=__ sign, used to assign a value to a __variable__.

- `equality`: This is denoted by __==__ sign, used to determine if two values are equal (P.S does not do strict equal or deep equal use `===` for strict equal).

#### EXAMPLES:

```js
const name = "Samuel";
name = "Ayo"; // This will error.

let name1 = "Ayomide";
name1 = "Samuel"; // This will not error;


// This is a comment

// FUNCTION
// It takes in two parameters firstNumber and secondNumber
function addTwoNumbers(firstNumber, secondNumber){
    console.log(firstNumber + secondNumber); // console.log() is used to output to the console the content of the parenthesis.
}

addTwoNumbers(2, 4); // This is the act of invoking a function.
addTwoNumbers(2, 3); // This is the act of invoking a function.
```

