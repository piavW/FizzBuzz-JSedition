# FizzBuzz - JavaScript edition
Built by: [Pia von Wachenfelt](https://github.com/piavW)

This was built over a weekend-challenge in september 2019, the answer to the questions in the course-material is at the bottom of this README. 

## What the code does
This code allows your to play the FizzBuzz-game.

## Dependencies & code
NPM, e2e-training-wheels: (chai, superstatic).
## Setup

## Acknowledgements

## License
MIT-license

# Bootcamp questions:
1. To the best of your knowledge please explain what the following lines of code do: 
global.browser = new BrowserHelpers()
global.expect = chai.expect;
    The code makes it so that whenever the keywords browser or expect are called upon it is understood through chai or e2es functionalities and helpers/assertion styles. Which means we can use those programs built-in helpers and assetion styles when we write our tests.
2. To the best of your knowledge please explain why we are placing the let fizzBuzz = new FizzBuzz outside the it block?
    We're placing it there so that the coded context is true for all the following it-blocks within that descriptions context.
    If we placed it in an it-block it would only happen/give that context to that specific it-block.

3. To the best of your knowledge please explain the difference between using === and == in JS?
    === is also called the identity operator, it  compares if the operators are equal and whether of the same type. The equality operator == compares operators equality and does a typeconversion if neccessary before it checks for equality. Because of this the identity operator is stricter than the equality operator. 

4. To the best of your knowledge please explain why we are moving (number % 5 === 0) to the top?
    Because if we don't the code will start to check if it's divisible by 3 and if it is it'll be satisfied and not check if it's divisible by 5. Since the code reads from top to bottom we need to have the bigger numbers or unlikely if-statements at the top. 

5. To the best of your knowledge please explain the difference between feature and unit test?
    Unit testing is when we test a specific piece of code or a smaller part of an application. We test that the code functions the way we programed it to. 
    
    Feature testing is when we test how an entire application works when it's used by a user, we test if the application does what we want it to do from a user's point of view. We question whether the functionality of the application makes sense to a user, administrator, or other roles.

6. To the best of your knowledge please explain what this following code does (references the describe-block with before, beforeEach and after in application.feature.js)?
    The code first adds a context through the describe, within that context it specifies that before any async function is used the code will wait until the browser visits the page. 
    The code also specifies that after the page has been visited, each beforeEach async function with the await-keyword shall do a reload of page before the code after the await-keyword is run. 
    The code also specifies that after the page has been visited, and after all async-function with an await-keyword has been run the browser shall close. 

7. 