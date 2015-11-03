1. Run the Dijkstra's Algorithm on the following graph. Use vertex 1 as the starting point: http://i.imgur.com/dWZ5cKh.png

2. In formulating the dynamic programming algorithm for the DWIS problem, we observed two recurrence cases. Prove both cases as it was presented in the lecture slides.

3. In formulating the dynamic programming algorithm for the Integral Knapsack problem, we observed two recurrence cases. Prove both cases as it was presented in the lecture slides.

4. Write the reconstruction algorithm for the dynamical programming solution to the Itegral Knapsack problem.

5. Given two strings X and Y of lenght m and n, respectively, defined over a set S = {a1, a2, ... , ak} of
finitely many symbols, we are interested in computing an optimal (minimum cost) alignment of two strings,
where two possible alignments are defined as (i) a mismatch with cost of c<sub>m</sub> and (ii) a gap with
cost c<sub>g</sub>. Alignments are made by inserting gaps to the strings.

Consider the following tow sequences defined over S = {A, G, C, T}, where

* X = A A C A G T T A C C
* Y = T A A G G T C A

In the following alignment, there are two mismatches and four gaps with total cost 2c<sub>m</sub> + 4c<sub>g</sub>:

````
  X: - A A C A G T T A C C
  Y: T A A - G G T - - C A
````

(There are 2 misaligned symbols and 4 gap symbol matches)

Give an dynamic programming algorithm to solve this problem.
