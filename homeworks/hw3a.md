1.
````
  partition(A, begin, end)
    pivotIndex = choosePivot(A, begin, end)
    pivot = A[pivotIndex]
    // put the chosen pivot at A[end]
    swap A[pivotIndex] and A[end]
    storeIndex = begin
    // Compare remaining array elements against pivot = A[end]
    for i = begin to end−1:
      if A[i] < pivot:
        swap A[i] and A[storeIndex]
        storeIndex = storeIndex + 1
    swap A[storeIndex] and A[end]  // Move pivot to its final place
````
Or some variation

2.
* Naive solution O(n): merge then go to the middle
* O(log n) solution: Do a binary search amongst two arrays. Assume A1[1] to be the median,
  since we know the size of both array, we can check if it is the median by checking the
  second array O(1). Now that we have a split of A1 and A2, we can recurse.

3.
* Naive solution O(n): the scan the array and find a place where the value drops.
* O(log n) solution: Go to the middle, check it against the first element and the last,
  If the first element is greater than the middle, the minimal element is on the left half
  Else it's on the right half. Recurse.
   
