# Problem Description

The Romans were a clever bunch. They conquered most of Europe and ruled it for hundreds of years. They invented concrete and straight roads and even bikinis[1]. One thing they never discovered though was the number zero. This made writing and dating extensive histories of their exploits slightly more challenging, but the system of numbers they came up with is still in use today. For example the BBC uses Roman numerals to date their programmes.

The Romans wrote numbers using letters - I, V, X, L, C, D, M. (notice these letters have lots of straight lines and are hence easy to hack into stone tablets)

The Kata says you should write a function to convert from normal numbers to Roman Numerals: eg

     1 --> I
     10 --> X
     7 --> VII
etc.

There is no need to be able to convert numbers larger than about 150.

Part II of the Kata

Write a function to convert in the other direction, ie numeral to digit
Clues

can you make the code really beautiful and highly readable?
* does it help to break out lots of small named functions from the main function, or is it better to keep it all in one function?
if you don't know an algorithm to do this already, can you derive one using strict TDD?
* does the order you take the tests in affect the final design of your algorithm?
* Would it be better to work out an algorithm first before starting with TDD?
if you do know an algorithm already, can you implement it using strict TDD?
* Can you think of another algorithm?
what are the best data structures for storing all the numeral letters? (I, V, D, M etc)
can you define the test cases in a csv file and use FIT, or generate test cases in xUnit?
what is the best way to verify your tests are correct?
Suggested Test Cases

URL: http://codingdojo.org/cgi-bin/wiki.pl?KataRomanNumerals
