````
1.
    A1 = [0, ∞, ∞, ∞, ∞, ∞, ∞]
    A2 = [0, ∞, ∞, 4, ∞, ∞, ∞]
    A3 = [0, 5, ∞, 4, ∞, ∞, ∞]
    A4 = [0, 5, 7, 4, ∞, ∞, ∞]
    A5 = [0, 5, 7, 4, 8, ∞, ∞]
    A6 = [0, 5, 7, 4, 8, 17, ∞]
    A7 = [0, 5, 7, 4, 8, 17, 18]

2. Case 1: Assume MWIS(G') != S. Then there must be a better MWIS(G') = S'.
This means that we can use MWIS(G') for MWIS(G). But that implies that S is not optimal for MWIS(G),
which is a contradiction. Similar argument can be made for case 2.
3. Similar argument as #2's answer. Please practice writing it out.

5.Given a optimal alignment of two strings, X, Y, there are three cases two consider:

  1. X[last] and Y[Last] line up
  2. X[Last] is paired with a gap
  3. Y[Last] is paired with a gap

Now come up with the optimal sub-structure:

    Let X' = X - X[last], Y' = Y - Y[last]
    
    Given an optimal alignment,
    
    Case 1: It's also optimal for X' and Y'
    Case 2: It's also optimal for X' and Y
    Case 3: It's also optimal for X and Y'

Recurrence:

    P[i,j] = penalty of optimal alignment of X[0:i] and Y[0:i] ( [0:i] means first i letters)
    for all i to |X| and j to |Y|:
      P[i,j] = min {
                    => P[i-1, j-1] + mismatch cost of x[i], y[j]
                    => p[i-1, j] + gap cost
                    => p[i, j-1] + gap cost
                   }
