# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
        2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No:212224040195
# Developed By:R.Mohamed Rafi
```
# 1-Norm of a Matrix
```
def matrix_norm(matrix):
    columns =zip(*matrix)
    col_sums=[sum(abs(x) for x in col) for col in columns]
    return f"{max(col_sums):.2f}"
matrix=eval(input())
result=matrix_norm(matrix)
print(result)
 ```
# 2-Norm of a Matrix

```
import numpy as np
import math 
import ast
mat=np.array(eval(input()))
ans=np.linalg.norm(mat,2)
norm_matr="{:.2f}".format(ans)
print(norm_matr)
```


# Infinity Norm of a Matrix
```
import numpy as np
mat=np.array(eval(input()))
ans=np.linalg.norm(mat,np.inf)
print("{:.2f}".format(ans))
```

## Output:
### 1-Norm of a Matrix

![image](https://github.com/user-attachments/assets/53c1b4df-8d97-4881-8d48-c26163ae5032)

### 2-Norm of a Matrix

![image](https://github.com/user-attachments/assets/47bd4fdd-0770-46af-9382-16fb51e0522a)

### Infinity Norm of a Matrix

![image](https://github.com/user-attachments/assets/01f3ffac-e137-4e4a-9840-9b7d3e9fba20)

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
