# Sprint Challenge: JavaScript Fundamentals

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a survey of problems. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied variables, functions, object literals, arrays, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a survey of JavaScript problems.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in JavaScript fundamentals.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

You will notice there are several JavaScript files being brought into the index.html file.  Each of those files contain JavaScript problems you need to solve.  If you get stuck on something, skip over it and come back to it later.

In meeting the minimum viable product (MVP) specifications listed below, you should have a console full of correct responses to the problems given.

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. Describe the biggest difference between `.forEach` & `.map`.

--> The .forEach() method runs a function on each element in an existing array while .map() runs a function on an existing array but is used to create a new array with those results.  .forEach() does not create a new array but rather modifies an existing one.

2. What is the difference between a function and a method?

--> A function is a collection of executable code closed by {}.  Example would be function speak() {console.log('Hello world!');} and run as speak().  A method is a function stored as a method.  An example of this would be either a method stored on an object created or a pre-defined method on the prototype of something like array or string prototype object.

3. What is closure?

--> Closure is a variable or function scope and its lexical environment.  In a function shown as:
function speak() {
    console.log('Hello world!');
}

the code within the {} is the scope and its lexical environment is the environment in which it was created.  With closure, the code can seek outside for context, for something like variable for example.  However in block level scope, it doesn't go the other way.  Meaning a const variable defined within those curly brackets would only be accessible within that scope and not outside.

4. Describe the four rules of the 'this' keyword.

--> Four rules/principles of the 'this' keyword:
1)Implicit Binding -- This is implied or suggested binding of the this keyword.  Example would be in a constructor function with this.name = name, this would be referring to the object being created or soon to be created from the constructor function.
2)Explicit Binding -- Explicit binding is when the this keyword is specifically binded to an object.  This can be acheived by using .bind(), .call() or .apply().
3)New Binding -- New binding is achieved when creating a new object.  For example, if I had a class of Dog with this.name = name, I would create a variable ex. const jake = new Dog({
    name = 'Jake'
});

with a new object under the class Dog, it would be using the new binding since the new keyword is used to create that class object.
4)Global Binding -- This is the binding to the console window.  If this is not defined in context within Javascript code, this refers to the console window.

5. Why do we need super() in an extended class?

--> super() in an extended class is what enables another class constructor to seek context to an extended class when using the constructor to build that new object.  For example, if this.name = name was under the class Animal and class Dog extends Animal, the super() allows the Animal class to send the parameter/object to Animal to build that object, in this case, assigning the this.name to name in that Dog object.  Without super(), it would not have that context and would not be able to build that object, resulting in a compiling error.

## Project Set up

Follow these steps to set up and work on your project:

- [ ] Create a forked copy of this project.
- [ ] Add PM as collaborator on Github.
- [ ] Clone your OWN version of Repo (Not Lambda's by mistake!).
- [ ] Create a new Branch on the clone: git checkout -b `<firstName-lastName>`.
- [ ] Create a pull request before you start working on the project requirements.  You will continuously push your updates throughout the project.
- [ ] You are now ready to build this project with your preferred IDE
- [ ] Implement the project on your Branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.

Follow these steps for completing your project:

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo).
- [ ] Add your Project Manager as a Reviewer on the Pull-request
- [ ] PM then will count the HW as done by  merging the branch back into master.


## Minimum Viable Product

Your finished project must include all of the following requirements:

**Pro tip for this challenge: If something seems like it isn't working locally, copy and paste your code up to codepen and take another look at the console.**

## Task 1: Objects and Arrays
Test your knowledge of objects and arrays. 
* [ ] Use the [objects-arrays.js](challenges/objects-arrays.js) link to get started.  Read the instructions carefully!

## Task 2: Functions
This challenge takes a look at callbacks and closures as well as scope. 
* [ ] Use the [functions.js](challenges/functions.js) link to get started. Read the instructions carefully!

## Task 3: Prototypes
Create constructors, bind methods, and create cuboids in this prototypes challenge.
* [ ] Use the [prototypes.js](challenges/prototypes.js) link to get started. Read the instructions carefully!

## Task 4: Classes
Once you have completed the prototypes challenge, it's time to convert all your hard work into classes.
* [ ] Use the [classes.js](challenges/classes.js) link to get started. Read the instructions carefully!

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

There are a few stretch problems found throughout the files, don't work on them until you are finished with MVP requirements!
