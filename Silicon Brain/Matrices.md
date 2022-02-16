## Definition
A matrix is a 2-dimensional grid of numbers. They can be used as representations of [[Systems of linear equations|systems of linear equations]], linear mappings, and more.

They are defined as follows:

$$
M = \begin{bmatrix}
a_{1, 1} & a_{1, 2} & \cdots & a_{1, c} \\
a_{2, 1} & a_{2, 2} & \cdots & a_{2, c} \\
\vdots & \vdots & \ddots & \vdots \\
a_{r, 1} & a_{r, 2} & \cdots & a_{r, c}
\end{bmatrix}
$$
where $c, r \in \mathbb{N}$ and $a$ is a $c \cdot r$ tuple of real numbers.

A matrix can be thought of as a vector of vectors, although it may not be a mathematically sound representation:

$$
M = \begin{bmatrix}
a_1 & b_1 & \cdots & z_1 \\
a_2 & b_2 & \cdots & z_2 \\
\vdots & \vdots & \ddots & \vdots \\
a_i & b_i & \cdots & z_i
\end{bmatrix}
$$
where $i \in \mathbb{Z}^+$  and $a, b, \dots,z \in R^i$

A much more concise definition can be used using the following convention:
$$
r, c \in \mathbb{N}, M \in \mathbb{R}^{r \times c}
$$

### Matrix addition
Matrix addition is a very simple operation, simply the element-wise sum:
$$
A + B := \begin{bmatrix}
A_{1, 1} + B_{1, 1} & \cdots & A_{1, c} + B_{1, c} \\
\vdots & \vdots & \vdots \\
A_{r, 1} + B_{r, 2} & \cdots & A_{r, c} + B_{r, c}
\end{bmatrix}
$$
where $r, c \in \mathbb{N}$ and $A, B \in \mathbb{R}^{r \times c}$.

### Matrix multiplication

^dc9aff

Matrix multiplication is a less trivial operation, defined as:
$$
C_{i, j} = \sum_{k=1}^{n}A_{i, k}B_{k,j}
$$
where $C = AB$.

An easier way of thinking about this is that each column $C_c$ is $A \cdot B_c$.
![[Matrices_2022-02-04 20.29.42.excalidraw]]
Then, it's easy to think of multiplying a matrix with a column [[Vectors|vector]] as the summation of scalar products with each element of the column vector and its corresponding vector in the matrix:
![[Matrices_2022-02-04 21.33.19.excalidraw]]
In effect, the matrix represents a [[Vectors#Vector spaces|vector space]] with each column vector being a basis vector in that [[Vectors#Vector spaces|vector space]]. Then, multiplying that matrix with another column vector represents the transformation of that column vector (which represents a vector in the standard vector space) considering each column of the matrix as a new basis vector. This is why matrices are usually used to represent linear mappings/transformations. Then, it is easy to think of matrix multiplication as stacking linear transformations.