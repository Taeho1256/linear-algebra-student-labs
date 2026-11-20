# Lab 05 Exercise 1: Explanation

Submit this file (or a `.txt` version) alongside your code, filled in with your own explanation.

Explain how floating-point rounding errors affect the orthogonality of the computed basis vectors and identify which of the three error measures captures this effect most clearly.

Floating-point rounding errors can cause the classical Gram-Schmidt process to lose orthogonality, especially when the columns of A are nearly linearly dependent.
As epsilon decreases, rounding errors become more significant, making the computed vectors less orthogonal.
Error2 = ||Q(T)Q − I||_F captures this effect most clearly because it directly measures the loss of orthogonality.
Error1 measures reconstruction accuracy, while error3 measures whether R is upper triangular.
