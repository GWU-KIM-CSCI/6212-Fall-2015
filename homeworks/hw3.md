# Homework 3

1. Write the in-place Partition algorithm I demonstrated in class. Below is the first 4 lines of it. 
````
  Partition(A, begin, end):
    pivotIndex = ChoosePivot(A, begin, end)
    pivot = A[pivotIndex]
    swap A[begin] with A[pivotIndex]
    ...
````

2. Given two sorted arrays, A1 and A2, each with n distinct numbers. Design a O(log n) time algorithm to find the median of the 2n numbers. You may safely assume that n is even.

3. A sequence x<sub>1</sub>, x<sub>2</sub>, ... , x<sub>n</sub> is said to be cyclically sorted if the smallest number in the sequence is x<sub>i</sub>, for some unknown i and the sequence x<sub>i</sub>, x<sub>i+1</sub>, ... , x<sub>n</sub>, x<sub>1</sub>, ... ,x<sub>i-1</sub> is sorted in an increasing order. Give an algorithm to find the position of the minimal element, x<sub>i</sub> in a cyclically sorted sequence with n elements.

````
   Example:
      input  A = [5,6,7,8,9,1,2],
             n = 7
             
      output 6th position
````
