```
    1. Similar to the knapsack problem.
    There are two cases, either at least 1 of v(n) is part of the answer or v(n)
    is not part of the solution. If S is the optimal solution, then 
       case 1: then we are using at least one v(n), thus we are now solving the
               subproblem of C-v(n),
       case 2: S is the optimal solution for v(1) ... v(n-1) for same C amount.
       
    2. Similar the string alignment problem. Three cases:
       case 1: If you already know how to convert A[1..(i−1)]A[1..(i−1)] to
               B[1..j]B[1..j], you can convert A[1..i]A[1..i] to B[1..j]B[1..j]
               by doing what you did with A[1..(i−1)]A[1..(i−1)], and deleting
               A[i]A[i].
       case 2: If you already know how to convert A[1..i]A[1..i] to
               B[1..(j−1)]B[1..(j−1)], you can convert A[1..i]A[1..i] to
               B[1..j]B[1..j] by doing what you did with A[1..i]A[1..i],
               and adding B[j]B[j].
       case 3: If you already know how to convert A[1..(i−1)]A[1..(i−1)] to
               B[1..(j−1)]B[1..(j−1)], you can do what you did in case 1,
               and replace A[i]A[i] by B[j]B[j]. However, if A[i]A[i] and
               B[j]B[j] are already equal, there's no need to replace it.
               
    3. We'll represent our choices as an array of zeros and ones, A.
        0 = do not take. 1 = take.
       Fitness function: weight of A + weight of next item <= M
    
    4. We'll represent our choices as an array of choices starting from top left
       corner and scanning one row at a time.
       Fitness function: apply the rule of Sudoku.
