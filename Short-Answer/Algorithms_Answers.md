#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) `O(n)`

The while loop produces an `O(n^3)` because it runs until `a` reaches `n * n * n`.
Inside the loop, `a` is incremented by `O(n^2)` every iteration it runs.  with the `a` value incrementing by `n * n`  we can subtract `O(n^2)` from the loops `O(n^3)` resulting in `O(n)`

b) `O(n Log(n))`

The outer loop in this instence would have a time complexity of `O(n)` because it is a for loop that iterates over a range of `n`.

The inner loop runs until `j` reaches `n`,  with the `j` doubling every iteration: `j *= 2`  this causes the inner loop to run at `O(log(n))`.  Every time j is doubled ,  the number of times the while loop will run is decreased at more than a linear rate.

we multiple these two together because it is a nested loop, resulting in `O(n log(n))`

c) `O(n)`

In this example the base case is zero bunnies. With every recursive call, the number of bunnies that the `bunnyEars(bunnies)` is called with decreases by 1. This causes the function to run `n` number of times resulting in `O(n)`. 

## Exercise II

I would start by checking the midpoint of the floors and checking if an egg breaks there.  If the egg breaks I would then find the mid point of everything left of the midpoint. However if it doesn't break I would find the mid point of everything to the right.

I would repeat this until there is only two remaining floors to check.
the one that breaks is the return.

The runtime complexity would be `O(log(n))`
