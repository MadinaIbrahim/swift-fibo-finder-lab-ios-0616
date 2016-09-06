# Fibonacci Finder

## Objectives

1. Practice storing and retrieving `Int` values in a collection.

## Introduction 

Programmers often utilize mathematical concepts, proofs, and algorithms to give themselves direction in writing an exercise. For this exercise, we're going to challenge ourselves to write a method that will calculate the Fibonacci Sequence to a specified length.

The Fibonacci Sequence is defined by the formula:

F<sub>n</sub> = F<sub>n-1</sub> + F<sub>n-2</sub>

with the accepted seed values as either:

F<sub>0</sub> = 0, F<sub>1</sub> = 1, or

F<sub>1</sub> = 1, F<sub>2</sub> = 1

and begins:

| F<sub>0</sub> | F<sub>1</sub> | F<sub>2</sub> | F<sub>3</sub> | F<sub>4</sub> | F<sub>5</sub> | F<sub>6</sub> | F<sub>7</sub> | F<sub>8</sub> | F<sub>9</sub> | F<sub>10</sub> | F<sub>11</sub> |  F<sub>12</sub> |
|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|
| 0 | 1 | 1 | 2 | 3 | 5 | 8 | 13 | 21 | 34 | 55 | 89 | 144 |

What the above information means is that, following the two initial values (in our case, `0` and `1`), each number is the sum of the two numbers preceding it in the sequence. If `0` is the zeroeth number (**Hint:** remember that arrays start at index `0`), then the first number is `1`, the second number is `0 + 1 = 1`, the third `1 + 1 = 2`, the fourth `1 + 2 = 3`, the fifth `2 + 3 = 5`, and so on into infinity.

Don't get intimidated by the math! Whether or not you recall learning about the Fibonacci Sequence in high school or college math class—if you've ever seen a snail shell or a pine cone you're already familiar with it. One of the amazing aspects of the Fibonacci Sequence (and of much of mathematics as a whole) is how prevalent it can be found in nature. Snail shells follow the Fibonacci Spiral (a geometric representation of the number sequence), while pine cones and sun flowers display the shape of Vogel's model (which relies on numbers in the Fibonacci Sequence).

Take a moment now (or save it for a study break later) to read about the [history of the Fibonacci Sequence](http://en.wikipedia.org/wiki/Fibonacci_number) (its oldest known anthropological roots are actually in Sanskrit prosidy in India dating as far back as 200 BC) and look at some [nature photography detailing Fibonacci geometry](http://www.inspirationgreen.com/fibonacci-sequence-in-nature.html). If you're interested in some numerology, [Arthur Benjamin's TED Talk ](https://www.youtube.com/watch?v=SjSHVDfXHQ4)is a six-minute video detailing how the Fibonacci Spiral and the Golden Ratio (1.618033...) are derived from the sequence.

## Instructions

1. Navigate to the `AppDelegate` file. Declare one function called `arrayWithFibonacciSequenceToIndex` which takes one `Int` argument called `index` and returns an `Array` of `Ints`.

5. Since the sequence requires the two previous numbers to calculate the next one, we need to prime the sequence. To do this, we're going to need to manually pass in `0` and `1` 

6. Now it's time to implement the algorithm. Chain an `else` statement to the `if` and `else if` statements to set a default behavior for every iteration of the loop after the first two. In order to calculate the next fibonacci number in the sequence, we're going to need to:
  * pull the previous two numbers out of the sequence,  
  * calculate the next fibonacci number in the sequence by the finding the sum of the two integers, and 
  * add the new fibonacci number to the sequence.  

##How To test
`Print()` the return of your function call to help you determine when your implementation is correct.

Test your function by calling and inputting the following as the argument:

`var testerIndex = 5`

The following should print in your console. 

`[0,1,1,2,3,5]`

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/ios-fibo-finder' title='Fibonacci Finder'>Fibonacci Finder</a> on Learn.co and start learning to code for free.</p>
