---
reference: "[[Class]]"
date: 16/08/2023
type: 1 #evergreen
alias: DIE00, Inverse Matrix
tags: mathematics, vectorial
code: DIE00
---
# DIE00 Inverse Matrix

Having $A \in M_{n\times n}$ its **Inverse Matrix**, symbolized by $A^{-1}$, is one that multiplying A with it the result will be the [[Identity Matrix]] $I_{n\times n}$. ^1

This type can be useful to resolve a equation system of the type $AX=B$, because Multiplying both sides by $A^{-1}$ you will obtain $X=A^{-1}B$ ^2

To find the [[#^1|Inverse]] of a $A$ matrix, you just need to apply [[Gauss-Jordan]] method to $A$ augmented by $I$, finished the process, the right side matrix will be $A^{-1}$. In symbols: $$\begin{pmatrix}
	a_{11}&a_{12}&\cdots&a_{1n}&\mid&  1   &  0   &\cdots&  0   \\
	a_{21}&a_{22}&\cdots&a_{2n}&\mid&  0   &  1   &\cdots&  0   \\
	\vdots&\vdots&\ddots&\vdots&\mid&\vdots&\vdots&\ddots&\vdots\\
	a_{n1}&a_{n2}&\cdots&a_{nn}&\mid&  0   &  0   &\cdots&  1   \\
\end{pmatrix}
\rightarrow
\begin{pmatrix}
	  1   &  0   &\cdots&  0   &\mid&a'_{11}&a'_{12}&\cdots&a'_{1n}\\
	  0   &  1   &\cdots&  0   &\mid&a'_{21}&a'_{22}&\cdots&a'_{2n}\\
	\vdots&\vdots&\ddots&\vdots&\mid&\vdots&\vdots&\ddots&\vdots\\
	  0   &  0   &\cdots&  1   &\mid&a'_{n1}&a'_{n2}&\cdots&a'_{nn}\\
\end{pmatrix}$$ ^3

[[#^1|Inverse Matrices]] have some properties. Being $A$, $B$ $\in$ $M_{n\times n}$ and $\alpha$ a scalar:
- $(AB)^{-1} = B^{-1}A^{-1}$
- $(A^{-1})^T = (A^T)^{-1}$
- $(A^{-1})^{-1} = A$
- $(\alpha A)^{-1} = \frac{1}{\alpha}A^{-1}$ ^4

# Links
<<[[DIE00A Elemental Matrix|DIE00A]]>>

**Related notes:**
- [[MPU01 Vector|Vector]] 