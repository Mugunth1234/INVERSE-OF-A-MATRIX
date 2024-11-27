# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each equations and assign in np.array()
### Step 3: 
Using the np.linalg.matrix_rank(), we can find the inverse of the given matrix
### Step 4: 
End the program
## Program:
```
import numpy as np
def find_matrix_inverse(matrix):
    try:
        matrix_np = np.array(matrix)
        if matrix_np.shape[0] != matrix_np.shape[1]:
            raise ValueError("Matrix must be square (same number of rows and columns).")
        matrix_inverse = np.linalg.inv(matrix_np)
        return matrix_inverse
    except np.linalg.LinAlgError:
        return 
    except ValueError as e:
        return str(e)
matrix = [[2, 1, 1], [1, 1, 1], [1, -1, 2]]
inverse = find_matrix_inverse(matrix)
print(inverse)
```
## output:
![Screenshot (1)](https://github.com/user-attachments/assets/3660eb6f-e105-41cb-aa05-1dd57d7c4eac)




## Result:
Thus the inverse of given matrix is successfully solved using python program

