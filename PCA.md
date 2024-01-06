# PCA (Principle Component Analysis)

## 1. eigenvalue and eigenvectors
### 1.1 definition
A $n\times n$ square matrix can be seen as a linear transformation defined in $R^n$ space. eigenvectors are vectors that will only be stretched or scaled by the matrix, the direction of the vector will not be changed, such that:

$$
Av=\lambda v
$$

Here, $v$ is one eigenvector of matrix A and $\lambda$ is the corresponding eigenvalues. 

- one eigenvalue can have infinite eigenvectors.
- different eigenvectors of different eigenvalues should be linear independent.
- If the matrix A is real symmetric, then the eigenvectors of different eigenvalues will be orthogonal.

### 1.2 why they are important and how to find them
the reason why eigenvectors are important is because the direction of these vectors will not be changed by the linear transformation represented by matrix $A$, and they will only be stretched or scaled. 

from $Ax=\lambda x$ we need to solve $(A-\lambda I)x=0$. we can have the characterisitc polynomial $p(\lambda)=det(A-\lambda I)$, by finding non-zero solution of the determinant of the equation we can have $\lambda_1,\lambda_2,...,\lambda_n$, which are eigenvalues we want, and replace $\lambda$ into the equation $(A-\lambda I)x$ we can solve for the eigenvectors.

## 2. eigendecomposition
### 2.1 definition
eigendecomposition means to write the square matrix in the form of $A=Q^T\Lambda Q$, where Q is the matrix of linear independent eigenvectors and $\Lambda$ is a diagonal matirx with diagonal elements as eigenvalues. eigendecomposition is related to the diagnonaliziable. eigendecomposition is to represent the linear transformation A by using a new set of basis, where the linear transformation on this set of basis will only stretch or scale each direction.

### 2.2 real symmetric matrix has eigenvectors that are orthogonal
suppose A is a real symmetric matrix,


$$
Ap_1=\lambda_1 p_1\ \ Ap_2=\lambda_2 p_2
$$

$$
p_1^T\lambda_1=p_1^T A^T=p_1^T A
$$

$$
p_1^T\lambda_1 p_2=p_1^T A p_2=p_1^T \lambda_2 p_2
$$

$$
(\lambda_1-\lambda_2)p_1^Tp_2=0\to p_1^T p_2=0
$$

## 3. SVD (singular value decomposition)

$A=U\Sigma V^T$

## 4. PCA
