# Quiz 2

What is the running time of the following algorithm? Use the master method to derive your answer in big O notation:

```
Solve(array A) // assume this runs in 3

Combine(array A1, A2, A3) // runs at 4n^3

Conquer(array A, size n):
	if (n == 1):
		return solve(A)
	else:
		A’   = Conquer(A[1 .. n/3], n/3)
		A’’  = Conquer(A[n/3+1 .. 2n/3], n/3)
		A’’’ = Conquer(A[2n/3+1 .. n], n/3)
		return Combine(A’, A’’, A’’’)
```
