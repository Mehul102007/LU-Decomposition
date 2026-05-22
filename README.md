# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## Step 1:Import the numpy module to use the built-in functions for calculation

## Step 2:Prepare the lists from matrix and assign in np.array()

## Step 3:Using the np.linalg.solve(), we can find the solutions.

## Step 4:End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: mehul narayanan v
RegisterNumber: 212225040231
'''
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: mehul Narayanan
RegisterNumber: 212225040231
'''
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)

```

## Output:

<img width="1243" height="569" alt="image" src="https://github.com/user-attachments/assets/cf86321d-ce84-4482-a417-4c168025a807" />
<img width="1332" height="219" alt="image" src="https://github.com/user-attachments/assets/9364d3a5-2bfa-4bea-8f0e-098df4063663" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

