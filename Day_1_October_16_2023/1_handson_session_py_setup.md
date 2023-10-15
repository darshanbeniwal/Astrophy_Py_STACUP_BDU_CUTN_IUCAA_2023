---
STACUP-2023:
  colab:
    toc_visible: true
  kernelspec:
    display_name: Python 3
    name: python3
  language_info:
    name: python
  Location: BDU, Trichy
  Date: OCTOBER 16TH, 2023
---
# 1.Check Python Version


```python
!python --version
```

# 2.Using Python as a calculator

## 2.1 Arithmetic Operators


## 2.2 Comparison Operators

## 2.3.Logical Operators

# 3.Print Command

## 3.1 Print Strings


```python
print(f'Hey there!')
```

## 3.3 Strings can be joined together


```python
print("Hey there!"*3)
```


```python
print("print there!" + " How are you?")
```

# 4.Comments


```python
#this is comment line
```


```python
print(f'Hey there!') # this is print command
```


```python

```

# 5.List, Tuple, Set and Dictionaries

## 5.1 List (or Array)


```python
x=[] # Define an empty list
x
```


```python
y=[1,2,3,5,4,5,6,9] #Define a list of numbers
y
```


```python
y[::-1] # Reverse the list
```


```python
len(y) # Check the length of list
```


```python
m=['Apple','Boy','Cat',[1,2]] # Define a list of objects with different data types
m[0][1], m[2][2], m[3][0] #Output: 'p','t',1

```


```python
y=[1,2,3,4,5,6,7] #Define a list of numbers
```


```python
y[2]  #Print an element or number of specific position
```


```python
y[-1]
```


```python
y[0:2]    #Print first two elements
```


```python
y[2:4]    #Print elements from 2nd position to 4th position
```


```python
y=[1,2,3] #Define a list of numbers
y[2]=4
y
```


```python
'''
Add List Items
'''
y=[1,2,3,4,5]
y.append(8)
print(y)
```


```python
'''
insert item at a particular position
'''
y=[1,2,3,4,5]
y.insert(1,8)
print(y)
```


```python
'''
Extend List
'''
x=[1,2,3,4]
y=[5,6,7,8]
x.extend(y)
print(x)
```


```python
'''
Remove Items from a list
'''
y=[1,3,4,7,8]
y.remove(3)       #Try to remove an unlisted item--Error? Its okay!
print(y)
```


```python
'''
Remove Specified Index use: pop
'''
y=[1,3,4,7,8]
y.pop(2)    #y.del(2)
print(y)
```


```python
'''
Remove Specified Index use: del
'''
y=[1,3,4,7,8]
del y[2]
print(y)
```


```python
'''
Remove a list completely
'''
y=[1,3,4,7,8]
del y        # expected output []
print(y)     #this will cause an error because you have succsesfully deleted "y".
```


```python
'''
Clear a list
'''
y=[1,3,4,7,8]
y.clear()
print(y)
```

## 5.2 Tuples


```python
'''
they’re immutable sequences. This means that you can’t change them after creation.
Tuple items are ordered, unchangeable, and allow duplicate values.
To create a tuple object, can use an assignment operation with a sequence of a
comma-separated items on its right side.
'''
```


```python
x=('Apple','Boy','Cat','Dog')
```

## 5.3 Sets


```python
x={'Apple','Boy','Cat','Dog','Boy'}
print(x)

```


```python
type(x)
```

## 5.4 Dictionaries


```python
'''
Dictionary items are ordered, changeable, and does not allow duplicates.
Dictionary items are presented in key:value pairs, and can be referred to by using the key name.
'''
India={"Name":"India","Continents":"Asia","Capital":"New Delhi"}
prsn=dict(Name="XYZ",Age="20",Height="170cm",Weight="70kg")
India, prsn
```


```python
India["Name"], India["Capital"], prsn["Name"], prsn["Weight"]
```


```python

```

# 6.Vector and Matrix


```python
'''
Now we are going to discuss vectors, matrices and Multidimentional Arrays
'''
import numpy
```

## 6.1 Vectors


```python
import numpy
x=numpy.array([1,2,3])   #a vector as a row
x
```


```python
y=numpy.array([[1],
              [2],
              [3]])   #a vector as a column
y
```


```python
import numpy as np
```

## 6.2 Matrix


```python
m=np.array([[1,2,3],
            [4,5,6]])
m
```


```python
m.shape
```


```python
'''
NumPy actually has a dedicated matrix data structure:
'''
mat=np.mat([[1,2,3],
            [4,5,6]])
mat
```


```python
mat.shape
```


```python
m.size
```


```python
m.ndim

```


```python
vec=np.array((1,2,3,4,5))
```


```python
# Select all elements of a vector
vec[:]
```


```python
# Select everything up to and including the fourth element
vec[:4]
```


```python
# Select everything after the fourth element
vec[4:]
```


```python
# Select the last element
vec[-1]
```


```python
# Select the first two rows and all columns of a matrix
m[:2,:]
```


```python
# Select all rows and the second column
m[:,1:2]
```

## 6.3 Maximum & Minimum values


```python
'''
Finding the Maximum and Minimum Values
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m), np.min(m)
```


```python
'''
Finding the Maximum and Minimum Values from the each axis
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m,axis=1)    #axis=0 max in each column & axis=1 max in each row
```

## 6.4 Reshaping the array


```python
import numpy as np
m=np.array([[1,2,3],
             [4,5,6],
             [7,8,9],
             [10,11,12]
             ])
m.shape
```


```python
m_=m.reshape(2,6)
m_
```


```python
m_.shape
```


```python
# Reshape it as a 1-D array
m__=m_.reshape(12)
m__
```


```python
m__.shape
```


```python
m.resize(2,6)
```


```python
m
```


```python
'''
reshape() does not changes the original array but only returns the changed array,
whereas the resize() method returns nothing and directly changes the original array.
'''
```

## 6.5 Transpose, Rank, Determinant, Diagonal,trace and inverse of a matrix


```python
'''
Transpose
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
m.T
```


```python
'''
Rank
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
np.linalg.matrix_rank(m)      #linear algebra
```


```python
'''
Determinant
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
np.linalg.det(m)
```


```python
'''
Diagonal
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
m.diagonal()

```


```python
# Return diagonal one above the main diagonal
m.diagonal(offset=1)
```


```python
# Return diagonal one below the main diagonal
m.diagonal(offset=-1)
```


```python
'''
Trace
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
m.trace()           # OR sum(m.diagonal())
```


```python
'''
Inverse
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
np.linalg.inv(m)

```

## 6.6 Eigenvalues and Eigenvectors, addition, subtraction,dot product of two matrices.


```python
'''
Eigenvalues and Eigenvectors
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
e_values,e_vectors=np.linalg.eig(m)
```


```python
e_values,e_vectors
```


```python
'''
Addition of two matrices
'''
m_a=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
m_b=np.array([[0,2,1],
            [4,1,3],
            [7,2,6]
            ])
np.add(m_a,m_b)     # m_ab=m_a+m_b
```


```python
'''
Substraction of two matrices
'''
m_a=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
m_b=np.array([[0,2,1],
            [4,1,3],
            [7,2,6]
            ])
np.subtract(m_a,m_b)     # m_ab=m_a+m_b
```


```python
'''
Multiplication or dot product of two matrices
'''
m_a=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
m_b=np.array([[0,2,1],
            [4,1,3],
            [7,2,6]
            ])
np.dot(m_a,m_b)
```


```python
'''
Alternatively, in Python 3.5+, operator @ will also work for mulitplication
'''
m_a@m_b
```


```python
'''
For elementwise multiplications of two matrices
'''
m_a*m_b
```


```python

```

# 7.Python Conditions-Loops


```python
'''
Equals:                   a == b
Not Equals:               a != b
Less than:                a < b
Less than or equal to:    a <= b
Greater than:             a > b
Greater than or equal to: a >= b
'''
```

## 7.1 if.....else


```python
a=4
b=6
if a<b:
  print("b is greater than a")
```


```python
'''
Indentation (whitespace at the beginning of a line) is used by Python to specify
scope in the code. Curly brackets are commonly used in other computer languages
for this reason.
'''
a=4
b=6
if a<b:
print("b is greater than a")
```


```python
a=4
b=6
if a>b:
  print("a is greater than b")
else:
  print("a is not greater than b")
```


```python
'''
Now suppose we have more than two conditions i.e. greater, less and equal
'''
a=4
b=5
if a>b:
  print("a is greater than b")
elif a==b:
  print("a is equal to b")
else:
  print("a is less than b")

'''
else executes the conditions if all previous conditions are not true
'''
```


```python
'''
one line if statement
'''
a=4
b=5
print("A") if a > b else print("=") if a == b else print("B")

```

## 7.2 while loop


```python
i=1
while i<5:
  print (i)
  i=i+1 #i+=1
```


```python
'''
break statement
'''
i=1
while i<5:
  print (i)
  if i==3:
    break
  i+=1
```

## 7.3 for loop


```python
alpha_b=['Apple','Boy','Cat']
for x in alpha_b: #x is a variable --->For loops iterate over a given sequence
  print(x)
```


```python
'''
exit the loop when x is boy
'''
alpha_b=['Apple','Boy','Cat']
for x in alpha_b:
  if x=='Boy':
    break
  print(x)

```


```python
'''
the range() Function
'''
for x in range(5):    #which means values from 0 to 4 not 0 to 5
  print(x)
```


```python
for x in range(2,5):
  print(x)
```


```python
for x in range(0,40,10):
  print(x)
```


```python
'''
Nested loops
'''
alpha_b=['Apple','Boy','Cat']
fruits=['banana','mango','cherry']
for x in alpha_b:
  for y in fruits:
    print(x,y)
#The inner loop will executed one time for each iteration of the outer loop
```

# 8.Functions


```python
'''
A function is defined using the def keyword in Python
'''
```


```python
def my_fun():
  print("Hey there!")
```


```python
my_fun()
```


```python
'''
now use the return statements to tell a function that a value should be returend
'''
def my_fun(x):
  return(x+5)
```


```python
print(my_fun(1))
print(my_fun(2))
print(my_fun(3))
print(my_fun(4))
print(my_fun(5))
```


```python
i=1
while i<5:
  print(my_fun(i))
  i+=1
```


```python
def my_fun(x):
  '''
  This function return the entered number + 5
  '''
  return(x+5)
```


```python

```

# 9.Math


```python
'''
Sometimes we have to perform mathematical tasks on numbers i.e. minimum, maximum,
 sqrt, ceil.,floor, pi etc.
'''
```


```python
a=(1,2,3,4)
b=[4,3,5,7]
print(min(a))
print(max(b))
```


```python
'''
absolute (positive) value of the spacified number
'''
a=-65
print(abs(a))
```


```python
'''
power of a number
'''
a=pow(3,4)   #3**4
print(a)
```


```python
'''
For some extended mathemaical function, please import math first
'''
import numpy as np
```


```python
x=np.sqrt(64)
x
```


```python
'''ceil or floor'''
x=5.000001
print(np.ceil(x))
print(np.floor(x))
```


```python
x=np.pi+6
x
```

# 10.File handling

## 10.1 Create/write a file


```python
import numpy as np
```


```python
#To create a new file in Python, use the open() method
file = open("my_file.txt", "w")

```


```python
file = open("my_file.txt", "w")
file.write("This is my first text file")
file.close()
```


```python
#Open a Text file and write some 1-D arrays
```


```python
a=np.array([[1],[2],[3],[4],[5],[6]])
```


```python
a_file = open("test.txt", "w")
for row in a:
    np.savetxt(a_file, row)
a_file.close()
```


```python
# Single Line statement to save datapoints
a=np.array([1,2,3,4])
np.savetxt("test.txt", a)
```


```python
aa=np.array([1,2,3,4,5])
bb=np.array([1,2,3,4,5])
np.savetxt("tt.txt", (aa,bb))
# np.savetxt("testt.txt", np.transpose([a,b]))


```


```python
# Add header to Text File
x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("testt.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh')

```


```python
# Add footer to Text File

x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("testt.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh', footer='ff')

```

## 10.2 Read a File


```python
f = open("testt.txt", "r")    #will see the way to define its location
```


```python
f = open("testt.txt", "r")    #will see the way to define its location
print(f.read())
f.close()

```


```python
# read text file using loadtxt
f= np.loadtxt("testt.txt")
```


```python
f
```


```python
f[0]
```


```python
# read text file using loadtxt
f= np.loadtxt("testt.txt",unpack="True")
```


```python
f
```


```python
f[0]
```

## 10.3 Delete a File


```python
#Now to delete a file or folder you have to interact with the operating system

#The OS module in Python provides functions for interacting with the operating system

# The OS module in Python provides functions for creating and removing a directory
#(folder), fetching its contents, changing and identifying the current directory, etc.
```


```python
import os
os.remove("my_file.txt")
```


```python

```

# 11.Plot data using Matplotlib


```python
import matplotlib
```


```python
print(matplotlib.__version__)  ##Check Matplotlib version
```


```python
'''
Generally we have many submodule of a Python module:
Most of the Matplotlib utilities lies under the pyplot submodule:
and are usually imported under the plt alias:
'''
```


```python
import matplotlib.pyplot as plt #Now the Pyplot package can be referred to as plt.
import numpy as np
```


```python
x=np.array([0,10])
y=np.array([0,250])
plt.plot(x,y)
```


```python
'''
Next try to use two submodule of numpy i.e. np.arange and np.linspace along with matplotlib
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.plot(t,fun)
```

## Set axis Labels


```python
'''
Set matplot labels
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun)
```

## Set Title of plot


```python
'''
Set Title of plot
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$") #loc = 'left'
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun)
```


```python
'''
Set Title of plot
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun)
```

## Change color of plot curve


```python
'''
Change the color of plot curve
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun,color='black')    # Or you can use color='k'
```


```python
'''
Change the markers plot curve:
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun,color='red',marker='o')
```


```python
"""
'o'	Circle
'*'	Star
'.'	Point
','	Pixel
'x'	X
'X'	X (filled)
'+'	Plus
'P'	Plus (filled)
's'	Square
'D'	Diamond
'd'	Diamond (thin)
'p'	Pentagon
'H'	Hexagon
'h'	Hexagon
'v'	Triangle Down
'^'	Triangle Up
'<'	Triangle Left
'>'	Triangle Right
'1'	Tri Down
'2'	Tri Up
'3'	Tri Left
'4'	Tri Right
'|'	Vline
'_'	Hline
"""
```


```python
'''
You can also use linestyle to change the plot curve format i.e.
'''
t=np.arange(-10,10,0.1)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun,color='red',linestyle='dotted')  #dashed
```


```python
'''
Control the line width
'''
t=np.arange(-10,10,0.1)
fun=np.sin(t)
plt.title("A Plot: $\sin(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun,color='red',linestyle='dotted',linewidth='5')  #dashed

```

## MultiPlot in a single plot


```python
'''
Control the line width
'''
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3')  #dashed

```

## Add Legands


```python
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend()
```


```python
'''
Here we can see there is not much space to drop curve label
==================>>>>>>First Method<<<<<<=================
'''
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
plt.ylim(-1,1.5)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend() #loc ="lower left"
```


```python
'''
Here we can see there is not much space to drop curve label
=================>>>>>>Second Method<<<<<<=================
'''
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
# plt.ylim(-1,1.5)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend(bbox_to_anchor =(1, 1)) #loc ="lower left" #fontsize = 18 # shadow = True # facecolor = 'yellow'
```

## Add Grid


```python
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
# plt.ylim(-1,1.5)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend(bbox_to_anchor =(1, 1)) #loc ="lower left" #fontsize = 18 # shadow = True # facecolor = 'yellow'
plt.grid() #axis = 'x' #color = 'green', linestyle = '--', linewidth = 0.5

```

## Rezise the image


```python
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
fig = plt.figure(figsize=(10, 8)) #dpi=80
# plt.ylim(-1,1.5)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend(bbox_to_anchor =(1, 1)) #loc ="lower left" #fontsize = 18 # shadow = True # facecolor = 'yellow'
plt.grid() #axis = 'x' #color = 'green', linestyle = '--', linewidth = 0.5

```

## Save Plot


```python
t=np.arange(-10,10,0.1)
fun1=np.sin(t)
fun2=np.cos(t)
fig = plt.figure(figsize=(10, 8)) #dpi=80
# plt.ylim(-1,1.5)
plt.title("A Plot: $\sin(t)$ and $\cos(t)$ versus $t$")
plt.xlabel("t")
plt.ylabel("Function")
plt.plot(t,fun1,color='red',linestyle='dotted',linewidth='2',label='$\sin(x)$ Function')  #dashed
plt.plot(t,fun2,color='blue',linestyle='dashed',linewidth='3',label='$\cos(x)$ Function')  #dashed
plt.legend(bbox_to_anchor =(1, 1)) #loc ="lower left" #fontsize = 18 # shadow = True # facecolor = 'yellow'
plt.grid() #axis = 'x' #color = 'green', linestyle = '--', linewidth = 0.5
plt.savefig('Sample_Outplot.png')
```


```python

```

## Errorbar Plots


```python
x=np.arange(0,10,1)
y=np.array((1,3,2,6,5,3,4,5,9,3))
y_err=y*0.3
# plt.errorbar(x,y,y_err)
# plt.errorbar(x,y,y_err,fmt='b.')
# plt.errorbar(x,y,y_err,fmt='b.',capsize=3)
# plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r')
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.xlabel('x')
plt.ylabel('y')
```

## Confidence levels regions


```python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
y_err=y*0.1
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.fill_between(x, y+1.*y_err, y-1.*y_err, facecolor='#F08080', alpha=0.99)
plt.fill_between(x, y+2.*y_err, y-2.*y_err, facecolor='#F08080', alpha=0.59)
plt.fill_between(x, y+3.*y_err, y-3.*y_err, facecolor='#F08080', alpha=0.39)

```


```python

```

## Scatter Plot


```python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
plt.scatter(x,y)
```

## Histogram Plot


```python
x=np.array((1,2,1,2,5,3,4,5,7,8,6,7,8,3,2,1))
plt.hist(x)
```

## Pie Chart Plot


```python
x=(45,23,37,5)
plt.pie(x)
```


```python
#Add Label
x=(45,23,37,5)
plt.pie(x,labels=["Sample(x1)", "Sample(x2)", "Sample(x3)", "Sample(x4)"])
```

## Three-dimensional Contour Plots


```python
def f(x, y):
    return np.sin(np.sqrt(x ** 2 + y ** 2))

x = np.linspace(-6, 6, 30)
y = np.linspace(-6, 6, 30)

X, Y = np.meshgrid(x, y)
Z = f(X, Y)

fig = plt.figure()
ax = plt.axes(projection='3d')
ax.contour3D(X, Y, Z, 60, cmap='binary')
ax.set_xlabel('x')
ax.set_ylabel('y')
ax.set_zlabel('z');
```

# 12.Dataframe using Pandas

## Import Packages


```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

## Create a dataframe


```python
df=pd.DataFrame(
    {
        "Name":["Tom","Jerry","Sam"],
        "Age" :[2,5,8],
     "Color":["Black","White","Brown"]
    }
)
```


```python
df
```


```python
df['Age']
```


```python
df['Color']
```


```python
df['Age'].max()
```

## Print Full Dataframe


```python
df_covid=pd.read_csv("https://raw.githubusercontent.com/darshanbeniwal/Statistical_Cosmology_using_Python_ICARD_2021/main/Week_9_Feb_01_2022/Covid_19_Jan_16_2022.csv")
```


```python
df_covid
```


```python
df_covid.dtypes
```

## Print the selected Column


```python
df_covid.head(5)
```


```python
df_covid.tail(5)
```


```python
df=df_covid['Total_Cases']
```


```python
df
```


```python
df_covid[['Country','Total_Cases']]
```


```python
df_covid[['Country','Total_Cases']].head(5)
```


```python
df_covid.loc[df_covid['Total_Cases']<1000]
```


```python
len(df_covid.loc[df_covid['Total_Cases']<1000])
```


```python
df_covid.corr()
```


```python

```

# 13.Random Number Operations


```python
import random
```

## Random Items from list, tuple \& string


```python
list=[0,2,4,6,8]
string="cosmology"
tuple=('Astronomy', 'Astrophysics', 'Cosmology', 'Dark Energy', 'Dark Matter')
```


```python
print(random.choice(list))
```


```python
print(random.choice(string))
```


```python
print(random.choice(tuple))
```


```python
random.random()
```

## Random Shuffle


```python
random.shuffle(list)  #shuffle will only work in list-->It changes the original list
print(list)
```

## Random Sampling


```python
list=[0,2,4,6,8]
random.sample(list,3) #return a particluar list of items without any chnage in origi list
```

## Generate Random Numbers


```python
print(random.randint(0,5))  #Generate a Random Number
```


```python
print([random.randint(0,10) for i in range(5)]) #Generate a list of Random Number List
```


```python
#Alternatively, for Random number list, you can use numpy as
np.random.randint(0,10,5)
```


```python
np.random.randint(0,10,size=5) #Basically the last arguments denotes the size of list
```


```python
np.random.randint(0,10,size=(2,5))
```


```python
#Suppose you want to generate random floating values using randint
np.random.randint(0,10,size=(2,5)).astype("float")/10
```


```python
#Alternatively, one can use random_sample
np.random.random_sample(size=(2,5))
```


```python
from IPython.display import clear_output
clear_output(wait=True)

```


```python

```
