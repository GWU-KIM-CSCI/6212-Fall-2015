1. You are given n types of coin denominations of values v(1) < v(2) < ... < v(n) (all integers). Assume v(1) = 1,
so you can always make change for any amount of money C.  Give a dynamic programming algorithm which makes change for a give
n amount of money C with as few coins as possible. Analyze the time complexity of your algorithm and
prove your principle of optimality.
2. The input to this problem is a pair of strings A = a(1) ... a(m) and B = b(1) ... b(n). The goal is
to convert A into B as cheaply as possible. The rules and cost are defined as follow. For a cost of 3
you can delete any letter. For a cost of 4 you can insert a letter in any position. For a cost of 5 you
can replace any letter by any other letter. For example, you can convert A = abcabc to B = abacab
via the following sequence: abcabc at a cost of 5 can be converted to abaabc, which at cost of 3 can be converted to
ababc, which at cost of 3 can be converted to abac, which at cost of 4 can be converted to abacb,
which at cost of 4 can be converted to abacab. Thus the total cost for this conversion would be 19.
This is probably not the cheapest possible conversion. Give a dynamic programming a lgorithm to solve this problem.
Analyze the time complexity of your algorithm and prove your principle of optimality.
(Note that the Unix diff command essentially solves this problem.)
3. Implement a backtracking solution to the Integral Knapsack problem state in the [Lecture7.pdf](https://github.com/GWU-KIM-CSCI/6212-Fall-2015/blob/master/lectures/lecture7.pdf). (Clearly state your fitness function)
4. Implement a backtracking algorithm that solves the game of 9x9 Sudoku described [here](http://en.wikipedia.org/wiki/Sudoku). (Clearly state your fitness function)
