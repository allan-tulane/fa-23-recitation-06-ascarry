# CMPS 2200 Recitation 06
## Answers

**Name:**_____Abby Scarry________


Place all written answers from `recitation-07.md` here for easier grading.



- **2)**
Write a recurrence for the **work** of this algorithm and solve it. Assume the input is $n$ to compute $F_n$.

W(n) = W(n-1) + W(n-2) + O(1)
W(n) = O(2^n)

- **3)**
Write a recurrence for the **span** of this algorithm and solve it.

S(n) = S(n-1) + S(n-2) + O(1)
S(n) = O(n)

- **4)**
Inspecting the `counts` list, what interesting pattern emerges?

When inspecting the 'counts' list, it shows that the fib_recursive algorithm has a pattern of often duplicating work and computing values in the fibonacci sequence multiple times, because of n-1 and n-2

- **6)**
When computing $F_n$, what is the maximum number of times that `fib_top_down(i)` will be called for any value $i$? Based on this, what is the **work** and **span** of this algorithm?

The maximum number of times it will be called is one time. Both work and span are O(n), because each Fibonacci number is computed once and avoids duplicated work

- **8)**
When computing $F_n$, what is the maximum number of times that $F_i$ will be read for any value $i$? Based on this, what is the **work** and **span** of `fib_bottom_up`?

The maximum number of times it will be called is n times. The work and span are also both O(n) in this case because each Fibonacci number is computed once from the 'fibs' list
