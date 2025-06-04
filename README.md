Roman Numerals
==============

About this Kata
---------------

I wasn't there, but I believe this Kata was performed at XP2001 by Kent Beck. Here is [[a video of Karl Scotland doing this Kata in Excel at agile 2008]](http://www.infoq.com/presentations/TDD-Managers-Nicolette-Scotland) Here is [[a video of JonJagger doing this Kata in Ruby using CyberDojo]](http://vimeo.com/15104374)

Problem Description
-------------------

The Romans were a clever bunch. They conquered most of Europe and ruled it for hundreds of years. They invented concrete and straight roads and even bikinis [[1]](http://sights.seindal.dk/sight/456_Roman_Villa_of_Piazza_Armerina.html). One thing they never discovered though was the number zero. This made writing and dating extensive histories of their exploits slightly more challenging, but the system of numbers they came up with is still in use today. For example the BBC uses Roman numerals to date their programmes.

The Romans wrote numbers using letters : `I`, `V`, `X`, `L`, `C`, `D`, `M`. (notice these letters have lots of straight lines and are hence easy to hack into stone tablets)

### Part I

The Kata says you should write a function to convert from normal numbers to Roman Numerals: eg

```
     1 --> I
     10 --> X
     7 --> VII

```

etc.

For a full description of how it works, take a look at [[this useful reference website]](http://www.novaroma.org/via_romana/numbers.html) : which includes an implementation of the Kata in javascript.

There is no need to be able to convert numbers larger than about 3000. (The Romans themselves didn't tend to go any higher)

In order to keep the kata light, we will not check for valid Roman Numeral.

### Part II

Write a function to convert in the other direction, ie numeral to digit

Roman numerals
--------------

Roman numerals, the numeral system of ancient Rome, uses combinations of letters from the Latin alphabet to signify values.
They are based on seven symbols:

| Symbol  | Value    |
| ------- | -------- |
| I       |    1     |
| V       |    5     |
| X       |   10     |
| L       |   50     |
| C       |  100     |
| D       |  500     |
| M       | 1000     |

Numbers are formed by combining symbols together and adding the values.
Generally, symbols are placed in order of value,
starting with the largest values.
When smaller values precede larger values,
the smaller values are subtracted from the larger values,
and the result is added to the total.

Example:

| Roman Number  | Computation                                    | Value      | Comment                         |
| ------------- | ---------------------------------------------- | ---------- | ------------------------------- |
| MMVI          |  1000 + 1000 + 5 + 1                           | 2006       | only addition                   |
| MCMXLIV       |   1000 + (1000 - 100) + (50 - 10) + (5 - 1)    | 1944       | addition and substraction       |

Clues
-----

-   Can you make the code really beautiful and highly readable?
-   does it help to break out lots of small named functions from the main function, or is it better to keep it all in one function?
-   if you don't know an algorithm to do this already, can you derive one using strict TDD?
-   does the order you take the tests in affect the final design of your algorithm?
-   Would it be better to work out an algorithm first before starting with TDD?
-   if you do know an algorithm already, can you implement it using strict TDD?
-   Can you think of another algorithm?
-   what are the best data structures for storing all the numeral letters? (`I`, `V`, `D`, `M` etc)
-   can you define the test cases in a csv file and use FIT, or generate test cases in xUnit?
-   what is the best way to verify your tests are correct?
