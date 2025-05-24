# 19CS301Module-9
### EX: 9.1                                            MATRIX OPERATIONS
### Aim: 
To Write a Python Program to subtract two matrices by reading the matrix from the user.
### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns of the matrix.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create a matrix.

STEP 5 : Define another function to subtract the matrices.

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
                item = A[i][j]-B[i][j]
   R.append(item)
C.append(R)
print(A)
print(B)
print(C)
```
### Output:
![image](https://github.com/user-attachments/assets/b1125b13-d26e-4404-acce-7dd2c1d2011c)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.2 LIST COMPREHENSION
### Aim: 
To Write a Python class program to store all odd numbers between 500 and 600 in a reverse order  using list comprehension.
### Algorithm:
STEP 1: Start.

STEP 2: Create a class.

STEP 3: Create variable a,b, and c for upper limit,lower limit and condition.

STEP 4: Intialise the values in the class.

STEP 5 : Define a method and using list comprehension calculate the result in reverse order.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```
class Generate:
    def __init__(self, first,d,last):
        self.first = first
        self.d = d
        self.last=last
    def Ap_generate(self):
        L=[i for i in range(self.last-1,self.first,self.d)]
        return L


Series = Generate(500,-2,600)

print(Series.Ap_generate())

```
### Output:
 ![image](https://github.com/23013357/19CS301Module-9/blob/main/w.png)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.3 ADVANCED LIST PROCESSING
### Aim: 
To Write a Python program to Find the transpose of a matrix using list Comprehension.

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
![image](https://github.com/user-attachments/assets/411a227a-f44d-4b1a-b489-c7592dddbb67)

### Result: Thus, the given program is implemented and executed successfully .
 


### EX: 9.4       TOEPLITZ MATRIX
### Aim: 
To Write a Python Program to check whether the given matrix is Toeplitz Matrix.


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

![image](https://github.com/user-attachments/assets/0fb8f81b-ab07-4b3e-b273-035a0f38566d)

### Result: Thus, the given program is implemented and executed successfully.


 ### EX: 9.5  search an element in a 2D array
### Aim: 
write a python Program to search an element in a 2D array


### Algorithm:
Start.

Input matrix dimensions (r, c).

Create a matrix M by reading integers into a 2D list.

Print the matrix row by row.

Take the element x to search for.

Search for x in M, print its position if found, otherwise print "Element is not found in the Matrix."

Stop.


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
def printmatrix(M):
    for i in range(len(M)):
        for j in range(len(M[0])):
            print(M[i][j],end=' ')
        print() 
def search(M,x):
    flag=False
    for i in range (len(M)):
        for j in range (len(M[0])):
            if x==M[i][j]:
                print('Element is found in (',i,',',j,')')
                flag=True
    return flag
r,c=input().split()
A=create_matrix(int(r),int(c))
x=int(input())
printmatrix(A)
print('search element is ',x)
if (not search(A,x)):
    print('Element is not found in the Matrix')
```
### Output:

![image](https://github.com/23013357/19CS301Module-9/blob/main/modul%209.png)

### Result: Thus, the given program is implemented and executed successfully.
 

