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
# Register No:212225040362
# Developed By:Samantha Shree SV
# 1-Norm of a Matrix
matrix = eval(input())
col_sum = [sum(abs(x) for x in col) for col in zip(*matrix)]
print("{:.2f}".format(max(col_sum)))



# 2-Norm of a Matrix

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
matrix = np.array(eval(input()))
result = np.linalg.norm(matrix,2)
print("{:.3}".format(result))


# Infinity Norm of a Matrix
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
matrix = np.array(eval(input()))
result = np.linalg.norm(matrix,np.inf)
print("{:.3}".format(result))




```
## Output:
### 1-Norm of a Matrix
<img width="1056" height="814" alt="Screenshot 2026-03-23 213718" src="https://github.com/user-attachments/assets/a28c442e-dd82-4c1c-8147-98eefa618f4e" />

<br>
<br>
<br>

### 2-Norm of a Matrix
<img width="1044" height="864" alt="Screenshot 2026-03-23 213734" src="https://github.com/user-attachments/assets/4f269f1d-b184-489e-b6b9-8e440096aa55" />

<br>
<br>
<br>

### Infinity Norm of a Matrix
<img width="940" height="822" alt="Screenshot 2026-03-23 213747" src="https://github.com/user-attachments/assets/58e8066c-2f19-4ef3-b4f9-ec61516e0966" />

<br>
<br>
<br>

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
