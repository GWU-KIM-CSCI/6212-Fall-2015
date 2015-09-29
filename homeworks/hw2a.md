    1. General idea of the algorithm: Traverse as if you are looking for the item,
       then replace the null with the item.
    2. 
    
        a. Grab the median of L1 (O(1)) and binary search for it in L2 to get the
           partition (O(log n)). Now you know the position of the L2's median in respect
        to both arrays. Repeat until you home in on nth element.
        b. Call algorithm from a. with the value of n/2
        
    3.
    
        a. Sort then for each of the element subtract from x and search for the counter part.
        b. As you traverse through S one by one, use a hashtable to keep track of elements
           that we saw and their counter part. If you encounter the counter part in the
           hashtable, then you are done.
           
    4. a, b, and d values are given below. Apply the master method
    
        a. a = 2, b = 4, d = 0
        b. a = 2, b = 4, d = 1/2
        c. a = 2, b = 4, d = 1
        c. a = 2, b = 4, d = 2
    
        More important than the mechanical solving of these recurrences is implicatoin of these values.
