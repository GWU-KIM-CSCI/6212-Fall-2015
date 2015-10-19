1. Answer is 18. To show work, you should show something like this:
    L1 = 1 , 3 , 13 , 14 , 2    | Sort(L1) = 1 2 3 13 14    | Median = 3  
    L2 = 6 , 18 , 5 , 15 , 16   | Sort(L2) = 5 6 15 16 18   | Median = 15
    L3 = 17 , 18 , 12 , 7 , 8   | Sort(L3) = 7 8 12 17 18   | Median = 12
    L4 = 10 , 12 , 11 , 19 , 20 | Sort(L4) = 10 11 12 19 20 | Median = 12
    L5 = 21 , 22                | Sort(L5) = 21 22 ∞ ∞ ∞    | Median = ∞
    
    Median of Medians = 12  (computed by brute force since our list of median is small)
    
    Partition = [ 1 3 2 6 5 7 8 10 11] + 12 + [13 14 18 15 16 17 18 12 19 20 21 22]
    
    12 is the 10th smalltest.
    
    Now we need to find 7th smallest in [13 14 18 15 16 17 18 12 19 20 21 22]
    
    L1 = [13 14 18 15 16] | sorted(L1) = 13 14 15 16 18
    L2 = [17 18 12 19 20] | sorted(L2) = 12 17 18 19 20
    L3 = [21 22]          | sorted(L3) = 21 22 ∞  ∞  ∞
    
    Median of Medians = median([15 18 ∞]) = 17
    
    Partition = [13 14 15 16 12 17] 18 [18 19 20 21 22]
    
    18 is the 7th smallest. Now we are done.

2. T = [ (1,4), (4,2), (2,3), (3,5), (3,6), (6, 7) ] for both a and b

3. Use scoring function = ci / ri where higher the score the worse. Proof is similar to the fractional knapsack.
