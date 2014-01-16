# Homework 1

1. How many lines does the following program print? Write a recursive function and solve it. You may assume *n* is a power of 2.

        function p(n)
            if n > 1:
                print("still going")
                p(n/2)
                p(n/2)

2. Solve the recurrenc: T(n) = 1/n + T(n-1), where T(0) = 0

3. Prove or disprove that 2^n+1 = O(2^n)
4. Prove or disprove that 2^(2n) = O(2^n)
5. Let P be a problem. The worst-case time complexity of P is O(n^2). The worst-case time complexity of P is also Ω(n logn). The first statement means that P can be solved in O(n^2) time even in the worst case using a certain algorithm. The second statement means that no algorithm can solve P in less than O(n logn) time in the worst case. Now, let A be an algorithm that solves P . Which statements of the following statements are consistent with this information about the complexity of P?

        a) A has worst-case time complexity O(n^2).
        b) A has worst-case time complexity O(n^(3/2))
        c) A has worst-case time complexity O(n).
        d) A has worst-case time complexity ϴ(n^2).
        e) A has worst-case time complexity ϴ(n^3).

3. Let f(n) = O(s(n)) and g(n) = O(t(n)). Prove or disprove the following.

        a) f(n) + g(n) = O(s(n) + t(n))
        b) s(n) * t(n) = Ω(f(n) * g(n))
        c) f(n) - g(n) = O(s(n) - t(n))
        d) s(n)/t(n) = Ω(f(n)/g(n))
    
4. Implement Queue data structure using stacks by implementing the following two operations: Queue and Dequeue

5. We discussed three algorithms to perform Find and Union operation on disjoint sets. Consider the following algorithm: Make the root of the tree with lower depth be a son of the root of the tree
with higher depth. (If two trees have the same depth, choose arbitrarily.) Show that Union can be done O(1) time and Find can be done in O(logn) time.