# Introductiong to Computer Science - Fall 2017

## Lab 6 - Functions and Change

**Purpose:** The purpose of this lab is to get some experience using functions in JavaScript. You will also practice using the `<script>` HTML element. You will design and write a simple web page that computes the number of coins and their denominations that might be used in making change.

**Practice:** Study the [JavaScript demos](http://itech190.erickuha.com/). Pay attention to the demos under the **function** heading.

**Instructions:** Create a web page called _makeChange.html_ that serves as a way to convert any number of pennies into as few coins as possible, using quarters, dimes, and nickels. The page should start out with a brief description of what the web page does and what the user of the page should do to use the page.

The next part of your page should include a text box that allows a user to enter some number of pennies and a button that will calculate and display the information mentioned about.

When the button is clicked, an output `<div>` should be filled with the following information:

* The minimum number of coins required to make change
* How many of those are quarters
* How many of those are dimes
* How many of those are nickels
* How many of those are pennies

For example, if the user entered 57 pennies, the output would look something like:

```
The total number of coins is 5. They are distributed as follows:
- 2 quarters
- 0 dimes
- 1 nickels
- 2 pennies
```

**Tips and Hints:** If you want to find the maximum number of quarters that can make a certain amount of change, the `Math.floor()` function can help. let's say that `pennies` has a value of 57. If you calculate `pennies / 25` in JavaScript, you will get something like 2.28. That is not quite the right answer because you can never have 0.28 quarters. However, `Math.floor(pennies/25)` gives exactly 2, which is the number of quarters in 57 cents. With a little tweaking, you can do something similar for all of the other coins.
