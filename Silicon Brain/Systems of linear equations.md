## Definition
A system of linear equations is a set of linear equations with a finite number of variables equal to the number of linear of equations in the system.

## Solvability
A system of linear equations is solvable if it is
- independent - that is, the system of linear equations is [[Linear dependence#^200e9f|linearly independent]]
- consistent - that is, solutions to subsets of the system do not contradict each other

## Solutions
1. Systems of linear equations can be solved efficiently by considering transforming the following linear system:

$$
\begin{align}
c_{1,1} \cdot x + c_{1, 2} \cdot y + ... + c_{1, i} \cdot z = a_1 \\
c_{2,1} \cdot x + c_{2, 1} \cdot y + ... + c_{2, i} \cdot z = a_2 \\
\vdots \\
c_{j, 1} \cdot x + c_{j, 2} \cdot y + ... + c_{j, i} \cdot z = a_j
\end{align}
$$
To a matrix and vector as follows:
$$
A = 
\begin{bmatrix}
c_{1, 1} & c_{1, 2} & ... & c_{1, i} \\
c_{2, 1} & c{_2, 2} & ... & c_{2, i} \\
\vdots & \vdots & & \vdots\\
c_{j, 1} & c_{j, 2} & ... & c{j, i}
\end{bmatrix}
v =
\begin{bmatrix}
a_1 \\
a_2 \\ 
\vdots\\
a_j
\end{bmatrix}
$$
And then, we simply solve for  the vector $x$  (which contains our solutions) in the following equation:

$$
Ax = v
$$
Which we can do easily by multiplying by the inverse matrix:
$$
\begin{align}
A^{-1}Ax = A^{-1}v \\
x = A^{-1}v
\end{align}
$$