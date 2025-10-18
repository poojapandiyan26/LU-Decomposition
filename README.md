# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrices

1 Import the required library numpy and scipy.linalg.

2 Read the input matrix A.

3 Use the lu() function to perform LU decomposition.

4 The output will be three matrices: P (permutation matrix), L (lower triangular), U (upper triangular).

5 Print L and U.

### (ii) To solve a system of equations using LU Decomposition
1 Import lu_factor and lu_solve from scipy.linalg.

2 Read the input matrix A and vector b.

3 Perform LU factorization using lu_factor(A).

4 Solve the equation AX = b using lu_solve.

5 Print the solution vector X.


## Program:
(i) To find the L and U matrix
```python
/*
Program to find the L and U matrix.
Developed by: POOJA SRI P
RegisterNumber: 212224230197
*/
import numpy as np
from scipy.linalg import lu
A= np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
/*
Program to find the LU Decomposition of a matrix.
Developed by: POOJA SRI P
RegisterNumber: 212224230197
*/
import numpy as np
from scipy.linalg import lu_factor ,lu_solve
A= np.array(eval(input()))
b= np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)

```

## Output:

<img width="1344" height="587" alt="image" src="https://github.com/user-attachments/assets/4c3cf5b0-19c7-4145-bfca-896a3732e303" />


<img width="1337" height="402" alt="image" src="https://github.com/user-attachments/assets/e466aded-6ad1-49e7-9705-4b0fb230bad2" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

