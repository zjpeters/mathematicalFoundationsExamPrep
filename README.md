# Topics covered on previous exams
- Vectors
    - Compute length and angle of vectors
    - Compute the products of two vectors, decide if two vectors are orthogonal
    - Show linear independence
    - write a vector as a linear combination of other vectors
    - normalize vector
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018A, 2020, 2021]
- Matrices
    - multiplication
    - transposition
    - Calculating determinant
    - inversion
    - orthogonal
    - Hurwitz criterion, finding a variable for which a matrix is pos or neg definite
    - Find matrix A that defines linear map $L_A$
    - Row echelon and row reduced forms
    - Write quadratic form Q_C(x_1,x_2) of matrix C
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2019, 2020, 2021]
- Computing eigenvalues and eigenvectors
    - Calculate characteristic polynomial
    - Verify that a vector is an eigenvector
    - is a matrix diagonizable
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2019, 2020, 2021]
- Linear equations
    - whether they have solutions and how many (none, one, infinitely many)
    - Solve system of linear equations
    - present in exams: [2014, 2015A, 2015 retake]
- Find complex numbers that solve equation **probably not on exam**
    - present in exams: [2014]
- Derivatives and integrals (definite and indefinite)
    - local linear approximations
    - present in exams: [2014, 2015A, 2015 retake, 2018, 2020, 2021]
- Differential equations
    - Ordinary Differential Equations (ODEs)
    - Partial differential equations
    - Solving initial value problem
    - Finding particular solutions
    - finding general solution
    - Homogenous solutions
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2018A, 2019, 2020, 2021]
- Partial derivatives
    - Find stationary points of f(x,y)
    - Find/verify critical points
    - decide whether f has local maximum or minimum at a given point
    - Calculate gradient vector and hessian matrix
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2018A, 2019]
- Find the euler expression 
    - present in exams: [2015A, 2015 retake]
- Taylor polynomial
    - Find local linear approximations of a function
    - Present in exams: [2018A, 2020, 2021]
# Potential information to include on mathematical foundations test sheet

-Compute the length of a vector: square root of the squares of each value in the vector
```math
\lVert u \rVert = \sqrt{u_1^2 + u_2^2 + ... + u_i^2}
```
- Compute the angle between two vectors: product of the vectors divided by the product of the lengths
```math
\arccos (\frac{a * b}{\lVert a \rVert * \lVert b \rVert})
```
- $u$ and $v$ are linearly dependent if:

$\lambda _1 u + \lambda _2 v = 0$

- where $\lambda _1$ and $\lambda _2$ are not equal to 0
- For a $2 \times 2$ matrix $A$ such that 
```math
\begin{pmatrix}
a   &   b   \\
c   &   d
\end{pmatrix} 
```
$det(A) = ad-bc$
- For a $3 \times 3$ matrix $A$ such that
```math
\begin{pmatrix}
a_{11}    &   a_{12}    &   a_{13}    \\
a_{21}    &   a_{22}    &   a_{23}    \\
a_{31}    &   a_{32}    &   a_{33}
\end{pmatrix}
```
$det(A) = a_{11}(a_{22}a_{33} - a_{23}a_{32}) - a_{12}(a_{21}a_{33} - a_{23}a_{31}) + a_{13}(a_{21}a_{32} - a_{22}a_{31})$
- equation for characteristic polynomial
    - the characteristic polynomial of a matrix $A$ is the determinant of $A$ minus $\lambda$ times the identity matrix    
    $P(\lambda) = det(A - \lambda * I)$


    - The eigenvalues are the roots of the char. polynomial, i.e. the solutions to $\lambda$
    - An $n \times n$ matrix is diagonalizable if it has $n$ different real eigenvalues
    - A matrix is positive definite if all eigenvalues are $> 0$
    - A matrix is positive semi-definite if all eigenvalues are $\ge 0$
    - A matrix is negative definite if all eigenvalues are $< 0$
    - A matrix is negative semi-definite if all eigenvalues are $\le 0$
    - If none of the above are true, matrix is indefinite
- for matrix multiplication ($A * B = C$) the number of columns in the first matrix ($A$) must equal the number or rows in the second matrix ($B$), the output ($C$) has the number or rows of $A$ and the number of columns of $B$
    - multiply and add rows of A with columns of B
    - Matrix multiplication,for $C=AB$ where $A$ is $m \times n$, and $B$ is $n \times p$:
```math
A = \begin{pmatrix}
a_{11}    &   a_{12}    &   a_{13}    \\
a_{21}    &   a_{22}    &   a_{23}    \\
a_{31}    &   a_{32}    &   a_{33}
\end{pmatrix},
B = \begin{pmatrix}
b_{11}    &   b_{12}    \\
b_{21}    &   b_{22}    \\
b_{31}    &   b_{32}
\end{pmatrix}
```
then $C$ is $m \times p$:
```math
C = \begin{pmatrix}
a_{11}b_{11} + a_{12}b_{21} + a_{13}b_{31}    &   a_{11}b_{12} + a_{12}b_{22} + a_{13}b_{32}   \\
a_{21}b_{11} + a_{22}b_{21} + a_{23}b_{31}    &   a_{21}b_{12} + a_{22}b_{22} + a_{23}b_{32}    \\
a_{31}b_{11} + a_{32}b_{21} + a_{33}b_{31}    &   a_{31}b_{12} + a_{32}b_{22} + a_{33}b_{32}
\end{pmatrix}
```
- quadratic form of matrix
    - Matrix $A$ must be square symmetric, i.e. $n\times n$, with each 

    $Q_A = x^T * A * x$
    - where x is a vector of length $n$
```math
\begin{pmatrix} x\\ y \end{pmatrix}
```
- Gradient vector and hessian matrix organization
    - Gradient vector is a vector of the first order partial derivatives
    - Stationary points are those where $\nabla f(x,y) = (0,0)$
    
```math
\nabla f = (\frac{\partial f}{\partial x}, \frac{\partial f}{\partial y})
```
- Hessian matrix is an $n \times n$ matrix containing the second order partial derivatives 
    - Hessian matrices which are indefinite are saddle points
    - hessian matrices which are negative definite are local maximum
    - hessian matrices which are positive definite are local minimum

```math
H_f = \begin{pmatrix} \frac{\partial ^2 f}{\partial x^2} \frac{\partial ^2 f}{\partial x \partial y} \\
                        \frac{\partial ^2 f}{\partial y \partial x} \frac{\partial ^2 f}{\partial y^2}
        \end{pmatrix}
```
- Taylor series/Taylor polynomial
    - If asked to find the linear approximation of a function, calculate the taylor series
    - calculate to $T_n$ where $n$ is the greatest root of the function, i.e. for the function:
    $x^2 + 3x + 1$
    
    - You would calculate the $T_2$ 
- Taylor polynomial formula
```math
T_n(f,x_0)(x) = \sum_{i=0}^{n}   \frac{f^{i}(x_0)}{i!} * (x-x_0)^i
```

- Chain rule of derivatives, for equations such as:
```math
h(x) = f(g(x))
```

The derivative can be calculated:

```math
h'(x) = f'(g(x)) * g'(x) 
```

- Product rule of derivatives, for equations such as:
```math
h(x) = f(x) * g(x)
```

The derivative can be calculated:

```math
h'(x) = f'(x) * g(x) + f(x) * g'(x)
```
- Integration by parts, inverse to the product rule
```math
\int u\partial v = uv - \int v \partial u
```

- Integration by substitution, inverse to the chain rule

- Ordinary Differential Equations (ODEs)
    - First order linear ODE, consider the inhomogeneous ODE:
    $y'(x) + a(x)y(x) = \psi(x)$
    - Step 1, solve the homogeneous solution $y' + a(x)y = 0$, the solution is:
    
    $y(x) = ce^{-A(x)}$

    - Where $A(x) = \int a(x)dx$, and $c$ is a a constant
    - Step 2, solve the particular solution $y^*(x)$ can be found by guessing or systematically as such, find:

    $W(x) = \int \psi (x)e^{A(x)} \partial x$

    - Then:

    $y^*(x) = W(x)e^{-A(x)}$

    - Alternately, with the homogeneous solution $y_h(x)$:

    $y^*(x) = y_h(x) \int \frac{\psi(x)}{y_h(x)}\partial x$

    - To guess the particular solution, if $\psi (x)$ is a polynomial guess a polynomial, if it is an exponential guess an exponential, if it is trigonometric guess a trigonometric expression, i.e.:
    
    $\psi (x) = 3x + 4$ guess $y^* = Ax + B$

    $\psi (x) = e^3x$ guess $y^* = Ae^3x$

    $\psi (x) = sin(3x)$ guess $y^* = Asin(3x) + Bcos(3x)$
## Table of trigonometric functions
```math
\begin{array}{ c | c | c | c | c | c }
    &   0   &   \pi /6  &   \pi /4  &   \pi /3  &   \pi /2  \\ \hline
sin &   0   &   1/2 &   \sqrt{2}/2    &    \sqrt{3}/2   &   1   \\  \hline
cos &   1   &   \sqrt{3}/2  &   \sqrt{2}/2  &   1/2 &   0   \\  \hline
tan &   0   &   \sqrt{3}/3  &   1   &   \sqrt{3}    &   --- \\  \hline
cot &   --- &   \sqrt{3}    &   1   &   \sqrt{3}/3  &   0   \\  \hline
\end{array}
```
- Where $0 = 0\degree, \pi/6 = 30\degree, \pi/4 = 45\degree, \pi/3 = 60\degree, \pi/2 = 90\degree$
- i.e. $sin(\pi/6) = 1/2$
- To calculate inverse functions such as $arcsin$, $arccos$, $arctan$, use the opposite direction, i.e. $arcsin(1/2) = \pi/6$

## Table of derivatives
```math
\begin{array}{ c | c | c }
function, f  &   derivative, f'   &   domain, I    \\  \hline
c (constant)    &   0   &   {\rm I\!R}  \\  \hline
x^\alpha, (\alpha \in {\rm I\!R})  &   \alpha x^{\alpha - 1}   &   ]0,\inf[ \\  \hline
ln(x)   &   1/x &   ]0,\inf[    \\  \hline
e^x &   e^x &   {\rm I\!R}  \\  \hline
a^x &   a^xln(a)    &   {\rm I\!R}, a > 0 \\  \hline
sin(x)  &   cos(x)  &   {\rm I\!R}  \\  \hline
cos(x)  &   -sin(x) &   {\rm I\!R}  \\  \hline
tan(x)  &   1/cos^2(x)  &   ](k-1/2)\pi, (k+1/2)\pi[, (k \in Z)    \\  \hline
cot(x)  &   -1/sin^2(x) &   ]k\pi, (k+1)\pi[, (k \in Z)    \\  \hline
arcsin(x)   &   1/(\sqrt{1-x^2})  &   ]-1,1[  \\  \hline
arccos(x)   &   -1/(\sqrt{1-x^2}) &   ]-1,1[  \\  \hline
arctan(x)   &   1/(1+x^2)   &   {\rm I\!R}  \\ \hline
\end{array}
```

- In this table, $Z$ is all integers, and R is all real numbers
## Trigonometric functions
- Periodicity:  $sin(x+2\pi) = sin(x), cos(x+2\pi) = cos(x)$
- Symmetry: $sin(-x) = -sin(x)$
- Pythagorean theorem:
$sin^2(x) + cos^2(x) = 1$
- $sin(x+y) = sin(x)cos(y) + cos(x)sin(y)$
- $cos(x+y) = cos(x)cos(y) - sin(x)sin(y)$
- $tan(x) = \frac{sin(x)}{cos(x)}$
- $cot(x) = \frac{cos(x)}{sin(x)}$
## Exponential functions
```math
\begin{array}{ c | c }
(a^b)^c = a^{bc}  &   ln(\sqrt{e}) = 1/2  \\  \hline
a^{\frac{b}{c}} = \sqrt[c]{a^b} &   ln(e^n) = n \\  \hline
a^b * a^c = a^{b+c}   &   ln(1) = ln(e^0) = 0   \\  \hline
a^{-b} = \frac{1}{a^{b}}   &   ln(0)  \text{ does not exist}   \\  \hline

\end{array}
```
