# Subashree-A-19CS301-Module9

### Register No - 212222020029
### Name - Subashree A

# ExNo: 9.1 MATRIX OPERATIONS
### Aim: To Write a Python Program to add two matrices by reading the matrix from the user.
### Algorithm:
STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns of the matrix.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create a matrix.

STEP 5 : Define another function to  add the matrices.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```
def create_matrix(n,m):
         M = []
         for i in range(n):
                   row = []
                   for j in range(m):
                      x = int(input())
                       row.append(x)
           M.append(row)
         return M
r,c = input().split()
A = create_matrix(int(r),int(c))
B = create_matrix(int(r),int(c))
C = []
for i in range(int(r)):
         R = []
        for j in range(int(c)):
                item = A[i][j]+B[i][j]
        R.append(item)
C.append(R)
print(A)
print(B)
print(C)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/fd1911c9-5a3c-4d50-9a0d-69c4369802df)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 9.2 LIST COMPREHENSION
### Aim: To Write a Python Program to read n elements in the list and separate  odd and even elements in the list.
### Algorithm:
STEP 1: Start the program.

STEP 2: Input the number of elements n.

STEP 3: Initialize an empty list l.

STEP 4: Read n integers from the user and store them in list l.

STEP 5: Create a list l3 by including only elements from l that are odd (i.e., i % 2 != 0).

STEP 6: Create a list l2 by including only elements from l that are even (i.e., i % 2 == 0).

STEP 7: Print the original list l.

STEP 8: Print the odd list l3.

STEP 9: Print the even list l2.

STEP 10: Stop
### Program:
```
n = int(input())
l = [int(input()) for i in range(n)]
l3=[i for i in l if i%2!=0 ]
l2 = [i for i in l if i%2==0 ]
print(l)
print(l3)
print(l2)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/643f3a08-7707-45d9-9fee-d2daaaa117ad)

### Result:Thus, the given program is implemented and executed successfully .
 
# ExNo: 9.3 ADVANCED LIST PROCESSING
### Aim: To Write a Python program to Find the transpose of a matrix using list Comprehension.
### Algorithm:
STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using list comprehension find the transpose of the matrix.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
def create(r,c):
            M=[]
        for i in range(int(r)):
             R = []
        for j in range(int(c)):
             x = int(input())
             R.append(x)
           M.append(R)
 return M
r,c = input().split()
matrix = create(int(r),int(c))
print(matrix)
T = [[r[i]for r in matrix]for i in range(len(matrix[0]))]
 print(T)
```
### Output:
![image](https://github.com/user-attachments/assets/c8c2de03-b9b4-4d50-86ba-51004da688c0)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 9.4 TOEPLITZ MATRIX
### Aim: To Write a Python Program to check whether the given matrix is Toeplitz Matrix.
### Algorithm:
STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create the matrix.

STEP 5 : Using the formula check for TOEPLITZ MATRIX .

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
def create_matrix(n,m):
        M=[]
        for i in range(n):
                row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
      return M
def print_matrix(M):
    for i in range(len(M)):
         for j in range(len(M[0])):
               print(M[i][j], end=' ')
     print()
def isThoeplitz(M):
#Type your code here
for i in range(len(M)):
      for j in range(len(M[0])):
             if i>0 and j>0 and M[i][j]!=M[i-1][j-1]:
                return False
       return True
n,m = input().split()
A = create_matrix(int(n),int(m))
print("A=",A)
if isThoeplitz(A):
      print(A,"is a Toeplitz Matrix")
 else:
       print(A,"is not a Toeplitz Matrix") print_matrix(A)
```
### Output:
![image](https://github.com/user-attachments/assets/0ed7d16f-55eb-4f53-89f2-ceb6e834fd07)

### Result: Thus, the given program is implemented and executed successfully.




