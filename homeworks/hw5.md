1. Apply the Select algorithm to the following example: L = { 1 , 3 , 13 , 14 , 2 , 6 , 18 , 5 , 15 , 16 , 17 , 18 , 12 , 7 , 8 , 10 , 12 , 11 , 19 , 20 , 21 , 22 } and k = 17. In other words find the 17th smallest element.

2. Do the following problems based on Graph G: http://i.imgur.com/dWZ5cKh.png
  - (a) Find a minimum spanning tree of G obtained using the Prim’s algorithm.
  - (b) Find a minimum spanning tree of G obtained using the Kruskal’s algorithm.
  
3. A source node of a data communication network has n communication lines connected to its destination node. Each line *i* has a transmission  rate *r<sub>i</sub>* representing  the  number  of  bits that can be transmitted per second.  A data needs to be transmitted with transmission rate at least M bits per second  from  the  source  node  to  its  destination  node.   If  a  fraction x<sub>i</sub> (where 0 <= x<sub>i</sub> <= 1) of line i is used (for example, a fraction x<sub>i</sub> of the full bandwidths of line i is used), the transmission rate through line i becomes x<sub>i</sub> * r<sub>i</sub> and a cost c<sub>i</sub> * x<sub>i</sub> is incurred.  Assume that the costs, c<sub>i</sub> (1 <= i <= n) are given.  The objective of the problem is to compute x<sub>i</sub> , for 1 <= i <= n , such that Sum of r<sub>i</sub> * x<sub>i</sub> >= M and Sum of c<sub>i</sub> * x<sub>i</sub> is minimized.
  - (a) Describe an outline of a greedy algorithm to solve the problem
  - (b) Prove that your algorithm is optimal


