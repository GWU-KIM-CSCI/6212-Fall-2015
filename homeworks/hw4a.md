1. See class notes. Essentially, sort by earliest ending time.

2. Let the given set of activities be S = {1, 2, 3, ..n} and activities are already sorted by finish time.
Assume that the optimal solution, B, has first activity other than 1,
then we can create a better solution, A, of same size with activity 1 as first activity.
Let the first activity selected by B be k, then there always exist A = (B – k) U {1}.
(Note that the activities in B are independent and k has smallest finishing time among all.
Since k is not 1, finish(k) >= finish(1)).

3. There are many possible counter examples.

4. We have already proven that Prim's algorithm spans G. There will come a point where e1 is considered.
At the point, consider the Cut(X, V-X). Since e1 is smaller than every other edge, it must be the minimal edge
of the crossing edges of the cut. Therefore it must be selected.

5. You should show your work but at the end you should end with the following array: [0, 2, 5, 4, 4, 11, 13, 9, 6]
