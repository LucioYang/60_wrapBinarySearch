# 60_wrapBinarySearch
## Inverse Functions and Logarithms
0. What is meant by y = logBASE(2,x)?
   - y = logBASE(2,x) means *2 raised to the power of y is equal to y*
1. What does its graph look like?
   - The graph looks like a curve with x and y increasing concurrently, though the rate of increase decreases as x increases. The graph has an asymptote of x = 0 and a root at x = 1. 
## Recursive Solution
0. Given a sorted list of length n return the ...
Decision to choose the base case or the recursive cases:
```
Is low > hi?
```
Base Case:
```
If yes, return -2.
```
Recursive Case:
```
If no, compare findMe to the element at index pageToCheck.
- If the comparison returns 0, return pageToCheck.
- If the comparison returns an int less than zero, return the index of the given element in the 
  interval (low) to (pageToCheck - 1).
- If the comparison returns an int greater than zero, return the index of the given element in the 
  interval (pageToCheck + 1) to (hi).
```
