# Summary of the course
at the moment five classes can be summarized in:

If a matrix is squared form, it has unique solution if its determinant is other number than zero
then
$AX=B$
$(A^{-1}A)X = A^{-1}B$

Inverse matrix properties.

To represent a elemental operation is with the next symbology
$E_{\text{<dest>}\space\text{<orig>}}(number)$

LU Factorization
1. Reducing the matrix ot its pivots, this result is U
2. using its elemental operation make U. having in count the next formula: $U = E1^{-1}E2^{-1}...En^{-1}$
   being each E an elemental operation.

LDU' Factorization

If the reduced matrix is found without using row interchanging then
$A=\space LU\space = \space LDU'$
where U is
$$\begin{pmatrix}
		d_{1}&u_{12}&\cdots&u_{1n}\\
	0     &d_{2}&\cdots&u_{2n}\\
	\vdots&\vdots&\ddots&\vdots\\
	0     &   0  &\cdots&d_{n}\\
\end{pmatrix}$$
D is 
$$\begin{pmatrix}
	d_{1} &  0  &\cdots&    0\\
	0     &d_{2}&\cdots&    0\\
	\vdots&\vdots&\ddots&\vdots\\
	0     &   0  &\cdots&d_{n}\\
\end{pmatrix}$$
and U'
$$\begin{pmatrix}
	1     &u_{12}/d_1&\cdots&u_{1n}/d_1\\
	0     &   1  &\cdots&u_{2n}/d_2\\
	\vdots&\vdots&\ddots&\vdots\\
	0     &   0  &\cdots&d_{n}\\
\end{pmatrix}$$


$L^{-1}$ is also an inferior triangular matrix.
$U^{-1}$ is also a superior triangular matrix.

If A is a symmetric matrix
then $L^{T}$ and $U'$are the same are the same matrix and $A = LDL^{T}$

Cholesky decomposition 
Having a Matrix A symmetric and it has $LDL^T$ factorization
then
$A = VV^T$ where $V = L\sqrt{D}$

**Permutation Matrix**
Is a matrix obtained as the product of all the permutation elemental matrix. Symbolized by P.

If you have to do permutations reducing a matrix, then you need to do the next equation
$PA=LU$

this type of 2