What is the recurrence of the recursive function conquer? Leave it in its recurrence form, do not solve.

```
function solve (array A) // assume this runs in 3

function combine(array A1, A2, A3) // runs at 4n^3

function conquer(array A, size n):
	if (n == 1):
		return solve(A)  <— 3
	else:
		A’   = conquer(A[1 .. n/3], n/3)  <— T(n/3)
		A’’  = conquer(A[n/3+1 .. 2n/3], n/3)  <— T(n/3)
		A’’’ = conquer(A[2n/3+1 .. n], n/3)  <— T(n/3)
		return combine(A’, A’’, A’’’)  <— 4n^3
```

Answer:

T(n) = 3  if n == 1, 3T(n/3) + 4n^3 otherwise
