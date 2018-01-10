## Problem-solving 

An intuition and feeling for problem solving **CANNOT** be taught.  They are forged through practice and often through the pain of overcoming a particularly difficult problem.  We can,however, be aware of different skills and techniques that will give us a place to start when the going gets tough and when it is difficult to see how to start.


#### Generalising

More often than not we want a solution to a problem that is as **general** as possible.  It would be silly and inefficient if a solution only worked in four different cases.  We want to be able to generalise our solutions so they apply in many different cases.  This is the essence of generalising.

In the following problems, it will be difficult to see a formula or solution straight away and a good strategy will be to start by considering smaller cases and then generalising once you begin to see a pattern.

Do **NOT** give up straight away - especially if there is maths involved.

One correct solution that you arrive at by yourself is worth far more than one that you have tried to emulate off the internet.

#### Problem 1

A digit sum is calculated by taking a number such as 3415 and literally adding the digits to get <br/> 3 + 4 + 1 + 5 = 13.
So we say the digit sum of 3415 is 13.<br/>

What is the digit sum of 10<sup>100</sup> - 1 ? <br/>
What is the digit sum of 10<sup>456</sup> - 1 ?


HINT: <br/> Calculate  10<sup>1</sup> - 1, 10<sup>2</sup> -1 ,10<sup>3</sup> - 1 ... then you can generalise!


#### Problem 2

The sequence of consecutive odd numbers goes something like this:
1, 3, 5, 7, 9, 11,...

What value would we get if we were to add the first 50 consecutive odd numbers together.

HINT: Sum low then think **BIG**

#### Problem 3

A sudoku board is a 9 x 9 grid divided into 9 smaller grids each of which contains the digits 1-9 <br/> http://www.sudokukingdom.com/

A newspaper editor constructs instead a super sudoku grid now which is 100 x 100 and contains 10 smaller grids each of which contain the digits 1 - 100. What is the total of the all the squares in the 100 x 100 sudoku grid added together ?

How would you do this for an n x n sudo grid?

#### Problem 4

I begin counting the fingers on my left hand from 1 to 1000 in the following way:
My thumb is counted as 1, the first finger is 2, middle finger is 3, ring finger is 4 and the the little finger is 5.  I then reverse direction so the ring finger is 6, the middle finger is 7 and so on...<br/>
If I continue in this manner on which finger will I end up ?

#### Problem 5

Today is a Wednesday.  What day of the week will be it be in 100 days time ?<br/>
**DON'T use google calendar.**<br/>
How would you design a function that calculated the day of the week any number of days from now?
Think about which parameters your function should have and what information it would need to store in order for it to work.


#### Problem 6

It is impossible to *dissect a square into 2 smaller squares.
Try it for yourself if you don't believe me.

For which values of n can you disect a square into n smaller squares?  Try to describe in words the algorithm you use to disect the square each time.

*A dissection is just a straight line cut across the shape.

#### Problem 7

A group of 50 soldiers must cross a deep river with no bridge in sight.  They notice two boys with a rowboat at the river bank.  The boat is big enough to hold at most 1 soldier or both of the 2 boys.  How can the soldiers get across the river and leave the boys in joint possession of the boat afterwards?
DRAW A DIAGRAM and describe how your algorithm should work.
How many times should the boat pass across the river in your solution?

How many times will the boat move across if there are 2018 soldiers?

#### Problem 8

A 3 x 3 x 3 cube is built up to form a cube consisting of 27 smaller cubes.
All six faces of the cube are painted green.

How many of the smaller cubes have 3 faces painted green ?
How many of the smaller cubes have 2 faces painted green ?
How many of the smaller cubes have 1 faces painted green ?
How many of the smaller cubes have 0 faces painted green ?

Imagine the cube is now 20 x 20 x 20 ?
How about a cube which is n x n x n ?



**Advanced**

For this problem we are going to think about the following scenario:
We have a number of coins in a row which can be either heads or tails.  We want to investigate the number of ways we can get combinations of heads and tails in this row.<br/><br/>
For example, if there are 3 coins in a row, some possible combinations might be HHT, TTT, HTH etc...<br/>
In particular, we are interested in the number of heads in the different combinations.<br/>
Suppose we have three coins in a row.
Then there is HHH, which means there is only **1 combination** with 3Hs as shown in the table below for 3 coin.<br/><br>
Fill in the tables below by counting the different combinations sysmtematically...


1 coin

|     0H     |     1H     |
|:----------:|:----------:|
|       ?    |      ?     |


2 coins coins

|     0H      |     1H      |  2H   |
|:-----------:|:-----------:| -----:|
|       ?     |      ?      |   ?   |

3 coins

|    0H     |   1H   |  2H   |   3H  |
|:---------:|:------:|------:|:-----:|
|     ?     |    ?   |   ?   |   1   |

4 coins

|    0H     |   1H   |  2H   |   3H  | 4H  |
|:---------:|:------:|------:|:-----:|:---:|
|     ?     |    ?   |   ?   |   ?   | ?   |


Create a recursive function called countCoinCombinations as shown below;

```javascript
const countCoinCombinations = (n,r) => {

    // base case ?
    // recursive step ?
};

```

It should take 2 arguments: n which is the number of coins in a row and r which is the number of heads in the combinations.<br/>
Use your tables to form a **general** relationship for countCoinCombinations that can be used in your function.<br/><br/>



HINT: 
```javascript
 countCoinCombinatons(10,3) = countCombinations(9,?)  + countCoinCombinations(?,?)
 ```


