# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 
        ---  Differences:
                .map();
                        .map(); is used for creating a new array from an already existing array, and applying a function to each one of the elements of the first array.
                                In the callback, only the array "element" is required, though it can take to more arguments which are index and the array itself.

                                Use case:
                                         Say you have an array of ingredients; you want to take those ingredients and make a meal out of them in a new array.
                                         You could use .map() to take the ingredients, use the callback function (that you already created) and make a new array of your choosing.
                                                        Bon Appétit!
                                                                       " map(['Corn', 'Beef', 'Chicken'], cook)
                                                                         => ['Popcorn', 'Steak', 'Eggs'] " 


                .filter();
                        .filter(); takes each element in an array and applies a conditional statement to check if it is true, or false. 
                                   If the conditional returns true, the element gets pushed to the output array.
                                   If the conditional return false, the element does not get pushed.           
                                                 The syntax for filter is similar to .map();, except the callback function must return true to keep the element, or false otherwise.
                                                 In the callback, only the element is required.   

                                Use case:
                                         We'll stick with our current cooking theme. You're now getting orders but someone at the table is vegetarian!
                                         You can use .filter(); to go through and filter out all of the foods that contain meat.

                                                        Now no one has any beef with anyone!

                                                                       " filter(['PopCorn', 'Steak', 'Eggs], isVegetarian)
                                                                            =>  ['Popcorn', 'Eggs'] 


                .reduce();
                        .reduce(); reduces an array of values down to just one value. To get the output value, it runs a 'reducer' function on each element of the array.
                        The callback argument passed in, is a function that well be called on once for every item in the array. 
                        .reduce(); takes four arguments, but most cases only use the first two. 
                        These four arguments are: accumulator, currentValue, index, array; and an optional initialValue. If provided, it will be used as the initial accumulator value in the first call to the callback function.

                                Use case:
                                        After all that great eating, there is something that is inevitable, .reduce();
                                                                Taking it all down to just one value.


                                                                        "reduce(['Popcore', 'Eggs'], eat)
                                                                                => 'waste'





2. Explain the difference between a callback and a higher order function.
        --- Higher Order Function:
                                  A higher-order function, is a function that takes another function(s) as an argument(s) or, returns a function to its callers.
        --- Callback Function:
                                  A callback function is a function that is passed to another function with the expectation that the other function will call it.


3. Explain what a closure is.
        --- Closure:
                    Closure, is when a function inside the lexical scope of another function reaches into the outerfunction to access data.


4. Describe the four principles of the 'this' keyword.
        #1
                Window Binding:
                                When in the global scope, the value of 'this' is the window / console Object.

        #2
                Implicit Binding:
                                Whenever a preceding dot calls a function, the object before the dot is 'this'.

        #3
                New Binding: 
                                Whenever using a constructor function, 'this' refers to the specific instance of the object that is created and returned by the constructor function.


        #4      
                Explicit Binding:
                                Whenever we use the .call(); or, .apply(); this is explicitly defined.




5. Why do we need super() in an extended class?
        --- .super();
                        We need .super(); as it allows us to access and call functions on an object's parent.

                        

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your reop to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/ master your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://lambdaschool.notion.site/lambdaschool/Lambda-School-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) See part 2, submitting an assignment with codegrade
