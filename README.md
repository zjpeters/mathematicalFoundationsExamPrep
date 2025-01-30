# Topics covered on previous exams
- Vectors
    - Compute length and angle of vectors
    - Compute the products of $u*v^T$ and $u^T*v$, decide if two vectors are perpendicular,
    - Show linear independence
    - write a vector as a linear combination of other vectors
    - normalize vector
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018A, 2020, 2021]
- Matrices
    - multiplication
    - transposition
    - Calculating determinant
    - inversion
    - Hurwitz criterion, finding a variable for which a matrix is pos or neg definite
    - Find matrix A that defines linear map L_A
    - Row echelon and row reduced forms
    - Write quadratic form Q_C(x_1,x_2) associated with matrix C
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2019, 2020]
- Computing eigenvalues and eigenvectors
    - Calculate characteristic polynomial
    - Verify that a vector is an eigenvector
    - is a matrix diagonizable
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2019, 2020, 2021]
- Linear equations
    - whether they have solutions and how many (none, one, infinitely many)
    - Solve system of linear equations
    - present in exams: [2014, 2015A, 2015 retake]
- Find complex numbers that solve equation
    - present in exams: [2014]
- Derivatives and integrals (definite and indefinite)
    - local linear approximations
    - present in exams: [2014, 2015A, 2015 retake, 2018, 2020, 2021]
- Differential equations
    - Solving initial value problem
    - Finding particular solutions
    - finding general solution
    - Homogenous solutions
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2018A, 2019, 2020]
- Partial derivatives
    - Find stationary points of f(x,y)
    - Find/verify critical points
    - decide whether f has local maximum or minimum at a given point
    - Calculate gradient vector and hessian matrix
    - present in exams: [2014, 2015A, 2015 retake, 2017, 2018, 2018A, 2019]
- Find the euler expression 
    - present in exams: [2015A, 2015 retake]
- Taylor polynomial
    - Present in exams: [2018A, 2020]
# Potential information to include on mathematical foundations test sheet
-Compute the length of a vector: square root of the squares of each value in the vector
```math
\lVert u \rVert = \sqrt{u_1^2 + u_2^2 + ... + u_i^2}
```
- Compute the angle between two vectors: product of the vectors divided by the product of the lengths
```math
\arccos (\frac{a*b}{\lVert a \rVert * \lVert b \rVert})
```
- equation for characteristic polynomial
    - the characteristic polynomial of a matrix $A$ is the determinant of $A$ minus $\lambda$ times the identity matrix    
    $P(\lambda) = det(A - \lambda * I)$


    - the eigenvalues are the roots of the char. polynomial, i.e. the solutions to $\lambda$
- for matrix multiplication ($A * B = C$) the number of columns in the first matrix ($A$) must equal the number or rows in the second matrix ($B$), the output ($C$) has the number or rows of $A$ and the number of columns of $B$
    - multiply and add rows of A with columns of B
- quadratic form of matrix
    - Matrix $A$ must be square symmetric, i.e. $n\times n$, with each 

    $Q_A = x^T * A * x$
    - where x is a vector of length $n$
```math
\begin{pmatrix} x\\ y \end{pmatrix}
```
- Gradient vector and hessian matrix organization
    - Gradient vector is a vector of the first order partial derivatives
    
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
    $ x^2 + 3x + 1$
    
    - You would calculate the $T_2$ 
- Taylor polynomial formula
```math
T_n(f,x_0)(x) = \sum_{i=0}^{n}   \frac{f^{i}(x_0)}{i!} * (x-x_0)^i
```

- Chain rule of derivatives
```math
h(x) = f(g(x))\\

h'(x) = f'(g(x)) * g'(x) 
```

- Product rule of derivatives
```math
h(x) = f(x) * g(x)\\
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
    - First, solve the homogeneous solution $y' + a(x)y = 0$, the solution is:
    
    $y(x) = ce^{-A(x)}$

    - Where $A(x) = \int a(x)dx$, and $c$ is a a constant
    - The particular solution $y^*(x)$ can be found by guessing (or systematically)
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
- i.e. $sin(\pi/6) = 1/2$
- Additionally, to calculate inverse functions such as $arcsin$, $arccos$, $arctan$, use the opposite direction, i.e. $arcsin(1/2) = \pi/6$

## Table of derivatives
```math
\begin{array}{ c | c | c }
function, f  &   derivative, f'   &   domain, I    \\  
c (constant)    &   0   &   {\rm I\!R}  \\
x^\alpha, (\alpha \in {\rm I\!R})  &   \alpha x^{\alpha - 1}   &   ]0,\inf[ \\  
ln(x)   &   1/x &   ]0,\inf[    \\  
e^x &   e^x &   {\rm I\!R}  \\  
a^x &   a^xln(a)    &   {\rm I\!R}, a > 0 \\  
sin(x)  &   cos(x)  &   {\rm I\!R}  \\  
cos(x)  &   -sin(x) &   {\rm I\!R}  \\  
tan(x)  &   1/cos^2(x)  &   ](k-1/2)\pi, (k+1/2)\pi[, (k \in \Z)    \\  
cot(x)  &   -1/sin^2(x) &   ]k\pi, (k+1)\pi[, (k \in \Z)    \\  
arcsin(x)   &   1/(\sqrt{1-x^2})  &   ]-1,1[  \\  
arccos(x)   &   -1/(\sqrt{1-x^2}) &   ]-1,1[  \\  
arctan(x)   &   1/(1+x^2)   &   {\rm I\!R}  \\ 
\end{array}
```
## Trigonometric functions
- Periodicity:  $sin(x+2\pi) = sin(x), cos(x+2\pi) = cos(x)$
- Symmetry: $sin(-x) = -sin(x)$
- Pythagorean theorem:
$ sin^2(x) + cos^2(x) = 1 $
- $sin(x+y) = sin(x)cos(y) + cos(x)sin(y)$
- $cos(x+y) = cos(x)cos(y) - sin(x)sin(y)$
