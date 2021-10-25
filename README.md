## 15

[Fifteen](https://en.wikipedia.org/wiki/15_puzzle) is a popular game which each can play without preparation.
But it cannot be solved in polynomial time nowadays. This is a try to approximate the solution.

At the beginning part of positions has not any solution because of parity.
For example, the solved puzzle with swapped 14 and 15. At first this code will exclude these cases.

The code works with 4x4 field and tries to continue the game 
from the nearest condition for the result - [Manhattan distance](https://en.wiktionary.org/wiki/Manhattan_distance)
to find the best one. After a limited count of iterations without any result it stops.
