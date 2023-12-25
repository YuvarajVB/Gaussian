# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Get the size of the system(n)
2. Initialize matrices for the argumented system and the solution
3. Perform the gaussian elimination to convert the matrix to upper triangular form 
4. perform back substitution

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Yuvarj V
RegisterNumber: 23013769
import numpy as np 
n=int(input())
arr=np.zeros((n,n+1))
res=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
res[n-1]=arr[n-1][n]/arr[n-1][n-1]
for i in range(n-1,-1,-1):
    res[i]=arr[i][n]
    for j in range(i+1,n):
        res[i]=res[i]-arr[i][j]*res[j]
    res[i]=res[i]/arr[i][i]
for i in range(n):
    print("X%d = %0.2f"%(i,res[i]),end=" ")
*/
```

## Output:
![gaussian elimination]()
![Screenshot 2023-12-25 060135](https://github.com/YuvarajVB/Gaussian/assets/151488375/a4a8be72-a3aa-4077-9b5b-b4de3d3e3eb3)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

