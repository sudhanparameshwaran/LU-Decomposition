# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
5(a)
step 1. Import numpy for multidimensional array operations

step 2. Bring lu from scripy.linalg to handle the actual matrix decomposition.

step 3. Call the lu(A) function. This splits the target matrix into three separate output matrices P,L and U.

step 4. End the program

5(b)

step 1. Import numpy for multidimensional array operations.

step 2. Bring lu from scipy.linalg to handle the actual matrix decomposition.

step 3. Pass the factorized components (lu,p) along with the right-hand side matrix b into the lu_solve() fenction to compute the solution matrix x.

step 4. End the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: sudhan 
RegisterNumber: 26019297
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"]= "1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()),dtype=float)
P,L,U=lu(A)
print(L)
print(U)

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: sudhan 
RegisterNumber: 26019297
*/
```
import os
os.environ["OPENBLAS_NUM_THREADS"]= "!"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a = np.array(eval(input()))
b = np.array(eval(input()))
l,p = lu_factor(a)
x = lu_lu_solve((l,p),b)
print(x)

## Output:
5(a):
<img width="866" height="807" alt="{02705EFA-2CE1-45DF-8818-42019B7A07A6}" src="https://github.com/user-attachments/assets/dc787cb1-f7a4-463a-8ecf-b7afe8708355" />


5(b);
<img width="925" height="794" alt="{796B15E9-970F-4FBF-B1F0-B98DD644E8BF}" src="https://github.com/user-attachments/assets/84767c39-962d-471a-83ae-6b285a400b9c" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

