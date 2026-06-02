# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To Find the L and U Matrices

Step 1: Start the program.

Step 2: Import the required libraries (numpy and scipy.linalg).

Step 3: Read the input matrix from the user.

Step 4: Convert the input matrix into a NumPy array.

Step 5: Apply the lu() function to perform LU decomposition.

Step 6: Obtain the permutation matrix (P), lower triangular matrix (L), and upper triangular matrix (U).

Step 7: Print the L matrix.

Step 8: Print the U matrix.

Step 9: Stop the program.

(ii) To Find the Solution Using LU Decomposition

Step 1: Start the program.

Step 2: Import the required libraries (numpy, lu_factor, and lu_solve).

Step 3: Read the coefficient matrix from the user.

Step 4: Read the constant matrix (right-hand side vector) from the user.

Step 5: Convert the inputs into NumPy arrays.

Step 6: Perform LU factorization of the coefficient matrix using lu_factor().


Step 7: Obtain the LU factors and pivot indices.

Step 8: Use lu_solve() to solve the system of equations.

Step 9: Store the computed solution in a variable.

Step 10: Print the solution vector.

Step 11: Stop the program.

## Program:
(i) To find the L and U matrix
/*
Program to find the L and U matrix.
Developed by: GOPIKA G
RegisterNumber: 212225230081
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix

/*
Program to find the LU Decomposition of a matrix.
Developed by: GOPIKA G
RegisterNumber: 212225230081
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
![lu decomposition]()
![alt text](image.png)
![alt text](image-1.png)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

