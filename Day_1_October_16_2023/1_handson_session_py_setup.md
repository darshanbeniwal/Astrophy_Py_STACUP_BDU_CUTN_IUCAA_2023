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

<div class="cell markdown" id="9EBkkpoXIxQl">

# 1.Check Python Version

</div>

<div class="cell code" id="bC_BoLoUHS6z">

``` python
!python --version
```

</div>

<div class="cell markdown" id="9KG2RSDnYz8G">

# 2.Using Python as a calculator

</div>

<div class="cell markdown" id="JJ8ykZ-A1f7W">

## 2.1 Arithmetic Operators

</div>

<div class="cell markdown" id="OxtaZ6ytykay">

## 2.2 Comparison Operators

</div>

<div class="cell markdown" id="QAhwNrEl0D-5">

## 2.3.Logical Operators

</div>

<div class="cell markdown" id="cITtqViR9cIE">

# 3.Print Command

</div>

<div class="cell markdown" id="8TKabvLj_oAd">

## 3.1 Print Strings

</div>

<div class="cell code" id="ogQc6xGf9yaZ">

``` python
print(f'Hey there!')
```

</div>

<div class="cell markdown" id="t7FEnMVn__al">

## 3.3 Strings can be joined together

</div>

<div class="cell code" id="MhyZfuEo-mNj">

``` python
print("Hey there!"*3)
```

</div>

<div class="cell code" id="ba3b6QZD-6iB">

``` python
print("print there!" + " How are you?")
```

</div>

<div class="cell markdown" id="gA7-GcNHWRoF">

# 4.Comments

</div>

<div class="cell code" id="xJoKKPq9aYaH">

``` python
#this is comment line
```

</div>

<div class="cell code" id="hh2-yT7LH1Ft">

``` python
print(f'Hey there!') # this is print command
```

</div>

<div class="cell code" id="u33ArBY2bNO1">

``` python
```

</div>

<div class="cell markdown" id="r85CAnHJzofL">

# 5.List, Tuple, Set and Dictionaries

</div>

<div class="cell markdown" id="721Klq5H2Oc5">

## 5.1 List (or Array)

</div>

<div class="cell code" id="Jqq3rQH4zf8U">

``` python
x=[] # Define an empty list
x
```

</div>

<div class="cell code" id="n5bjo3Kc4aM9">

``` python
y=[1,2,3,5,4,5,6,9] #Define a list of numbers
y
```

</div>

<div class="cell code" id="OoOxEQsBfmG3">

``` python
y[::-1] # Reverse the list
```

</div>

<div class="cell code" id="GOz4mLV_7G3c">

``` python
len(y) # Check the length of list
```

</div>

<div class="cell code" id="OigvtQBP5UX1">

``` python
m=['Apple','Boy','Cat',[1,2]] # Define a list of objects with different data types
m[0][1], m[2][2], m[3][0] #Output: 'p','t',1
```

</div>

<div class="cell code" id="KZEp6qMV7Y-q">

``` python
y=[1,2,3,4,5,6,7] #Define a list of numbers
```

</div>

<div class="cell code" id="85z3WqqV7bhE">

``` python
y[2]  #Print an element or number of specific position
```

</div>

<div class="cell code" id="_8Z9rBIL8zC2">

``` python
y[-1]
```

</div>

<div class="cell code" id="TwO6Js6R9Kqo">

``` python
y[0:2]    #Print first two elements
```

</div>

<div class="cell code" id="wDkug5UH9-MF">

``` python
y[2:4]    #Print elements from 2nd position to 4th position
```

</div>

<div class="cell code" id="2luS3fjP5xzv">

``` python
y=[1,2,3] #Define a list of numbers
y[2]=4
y
```

</div>

<div class="cell code" id="mpQd3V9y6-dL">

``` python
'''
Add List Items
'''
y=[1,2,3,4,5]
y.append(8)
print(y)
```

</div>

<div class="cell code" id="1RJwpw05_yPX">

``` python
'''
insert item at a particular position
'''
y=[1,2,3,4,5]
y.insert(1,8)
print(y)
```

</div>

<div class="cell code" id="WaiGAt63__3I">

``` python
'''
Extend List
'''
x=[1,2,3,4]
y=[5,6,7,8]
x.extend(y)
print(x)
```

</div>

<div class="cell code" id="iwBEihbIAdiy">

``` python
'''
Remove Items from a list
'''
y=[1,3,4,7,8]
y.remove(3)       #Try to remove an unlisted item--Error? Its okay!
print(y)
```

</div>

<div class="cell code" id="uFn_7CGZAzWH">

``` python
'''
Remove Specified Index use: pop
'''
y=[1,3,4,7,8]
y.pop(2)    #y.del(2)
print(y)
```

</div>

<div class="cell code" id="vymb0Rz1CCeS">

``` python
'''
Remove Specified Index use: del
'''
y=[1,3,4,7,8]
del y[2]
print(y)
```

</div>

<div class="cell code" id="xzew2IhvCcXS">

``` python
'''
Remove a list completely
'''
y=[1,3,4,7,8]
del y        # expected output []
print(y)     #this will cause an error because you have succsesfully deleted "y".
```

</div>

<div class="cell code" id="F-n7PW4JDKHC">

``` python
'''
Clear a list
'''
y=[1,3,4,7,8]
y.clear()
print(y)
```

</div>

<div class="cell markdown" id="wRvT8U3mD0AC">

## 5.2 Tuples

</div>

<div class="cell code" id="RdGpYzhSDi_9">

``` python
'''
they’re immutable sequences. This means that you can’t change them after creation.
Tuple items are ordered, unchangeable, and allow duplicate values.
To create a tuple object, can use an assignment operation with a sequence of a
comma-separated items on its right side.
'''
```

</div>

<div class="cell code" id="ObJagnG5EEWv">

``` python
x=('Apple','Boy','Cat','Dog')
```

</div>

<div class="cell markdown" id="_H_1sduxHI4J">

## 5.3 Sets

</div>

<div class="cell code" id="QmV3ULynHTXs">

``` python
x={'Apple','Boy','Cat','Dog','Boy'}
print(x)
```

</div>

<div class="cell code" id="aX7NKTEbHehp">

``` python
type(x)
```

</div>

<div class="cell markdown" id="ely9thUQIYgY">

## 5.4 Dictionaries

</div>

<div class="cell code" id="aAN-EGqrHwF2">

``` python
'''
Dictionary items are ordered, changeable, and does not allow duplicates.
Dictionary items are presented in key:value pairs, and can be referred to by using the key name.
'''
India={"Name":"India","Continents":"Asia","Capital":"New Delhi"}
prsn=dict(Name="XYZ",Age="20",Height="170cm",Weight="70kg")
India, prsn
```

</div>

<div class="cell code" id="igALKvjMJYYP">

``` python
India["Name"], India["Capital"], prsn["Name"], prsn["Weight"]
```

</div>

<div class="cell code" id="J8anwHuWbpx3">

``` python
```

</div>

<div class="cell markdown" id="S2YLVA8XKvy8">

# 6.Vector and Matrix

</div>

<div class="cell code" id="f8-jIYufKBkS">

``` python
'''
Now we are going to discuss vectors, matrices and Multidimentional Arrays
'''
import numpy
```

</div>

<div class="cell markdown" id="Lrdrkbr6MK_K">

## 6.1 Vectors

</div>

<div class="cell code" id="hEXDhWg1KvAw">

``` python
import numpy
x=numpy.array([1,2,3])   #a vector as a row
x
```

</div>

<div class="cell code" id="uRGxZ-6-M4wk">

``` python
y=numpy.array([[1],
              [2],
              [3]])   #a vector as a column
y
```

</div>

<div class="cell code" id="I-V_boN0ht5z">

``` python
import numpy as np
```

</div>

<div class="cell markdown" id="Cwf9oeerOaXL">

## 6.2 Matrix

</div>

<div class="cell code" id="JZzcYJ5KOBS4">

``` python
m=np.array([[1,2,3],
            [4,5,6]])
m
```

</div>

<div class="cell code" id="UJByfVAWNvbN">

``` python
m.shape
```

</div>

<div class="cell code" id="PbteY-YjOKRO">

``` python
'''
NumPy actually has a dedicated matrix data structure:
'''
mat=np.mat([[1,2,3],
            [4,5,6]])
mat
```

</div>

<div class="cell code" id="Y4yTDS5FO4dG">

``` python
mat.shape
```

</div>

<div class="cell code" id="sOxVhkXpQdvc">

``` python
m.size
```

</div>

<div class="cell code" id="NzjjcvTpQgh1">

``` python
m.ndim
```

</div>

<div class="cell code" id="ckkBQJZG5nx3">

``` python
vec=np.array((1,2,3,4,5))
```

</div>

<div class="cell code" id="NLb2skB8Port">

``` python
# Select all elements of a vector
vec[:]
```

</div>

<div class="cell code" id="VH5YHsofPzzF">

``` python
# Select everything up to and including the fourth element
vec[:4]
```

</div>

<div class="cell code" id="e5g8a-mDP02k">

``` python
# Select everything after the fourth element
vec[4:]
```

</div>

<div class="cell code" id="n4paDw2PQDL3">

``` python
# Select the last element
vec[-1]
```

</div>

<div class="cell code" id="3RbNfKmiQLhh">

``` python
# Select the first two rows and all columns of a matrix
m[:2,:]
```

</div>

<div class="cell code" id="Q4Z3uZb5QWWn">

``` python
# Select all rows and the second column
m[:,1:2]
```

</div>

<div class="cell markdown" id="XY6QgUcJ9WwH">

## 6.3 Maximum & Minimum values

</div>

<div class="cell code" id="FZSS5NTuQZ7s">

``` python
'''
Finding the Maximum and Minimum Values
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m), np.min(m)
```

</div>

<div class="cell code" id="xECK2JWjQ1ie">

``` python
'''
Finding the Maximum and Minimum Values from the each axis
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m,axis=1)    #axis=0 max in each column & axis=1 max in each row
```

</div>

<div class="cell markdown" id="B7Muc7yU_Bwj">

## 6.4 Reshaping the array

</div>

<div class="cell code" id="eZ0CpNGBRD52">

``` python
import numpy as np
m=np.array([[1,2,3],
             [4,5,6],
             [7,8,9],
             [10,11,12]
             ])
m.shape
```

</div>

<div class="cell code" id="_AC4aksc_1CM">

``` python
m_=m.reshape(2,6)
m_
```

</div>

<div class="cell code" id="RBMvxLTwAIKG">

``` python
m_.shape
```

</div>

<div class="cell code" id="Eq7xKRMKBUXc">

``` python
# Reshape it as a 1-D array
m__=m_.reshape(12)
m__
```

</div>

<div class="cell code" id="_euhGxjDCUrM">

``` python
m__.shape
```

</div>

<div class="cell code" id="wlkFqb-hCWyx">

``` python
m.resize(2,6)
```

</div>

<div class="cell code" id="imyrh_Z9CbLG">

``` python
m
```

</div>

<div class="cell code" id="yytgIDztCdD-">

``` python
'''
reshape() does not changes the original array but only returns the changed array,
whereas the resize() method returns nothing and directly changes the original array.
'''
```

</div>

<div class="cell markdown" id="frAIekrneEJL">

## 6.5 Transpose, Rank, Determinant, Diagonal,trace and inverse of a matrix

</div>

<div class="cell code" id="xfVtDWvgdx0p">

``` python
'''
Transpose
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
m.T
```

</div>

<div class="cell code" id="fLWc0DkwezfZ">

``` python
'''
Rank
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
np.linalg.matrix_rank(m)      #linear algebra
```

</div>

<div class="cell code" id="_tS-C2_hfwVg">

``` python
'''
Determinant
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
np.linalg.det(m)
```

</div>

<div class="cell code" id="qgSPvyEOiKsk">

``` python
'''
Diagonal
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
m.diagonal()
```

</div>

<div class="cell code" id="mjCYbG8Ric5h">

``` python
# Return diagonal one above the main diagonal
m.diagonal(offset=1)
```

</div>

<div class="cell code" id="aPILSftoixJn">

``` python
# Return diagonal one below the main diagonal
m.diagonal(offset=-1)
```

</div>

<div class="cell code" id="g1hn-jUri17A">

``` python
'''
Trace
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
m.trace()           # OR sum(m.diagonal())
```

</div>

<div class="cell code" id="pFpjLHVNjTqn">

``` python
'''
Inverse
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,1,9]
            ])
np.linalg.inv(m)
```

</div>

<div class="cell markdown" id="KUS4dS7nl4XC">

## 6.6 Eigenvalues and Eigenvectors, addition, subtraction,dot product of two matrices.

</div>

<div class="cell code" id="4UFlhkpVjisQ">

``` python
'''
Eigenvalues and Eigenvectors
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]
            ])
e_values,e_vectors=np.linalg.eig(m)
```

</div>

<div class="cell code" id="4XT8c6oWmN4P">

``` python
e_values,e_vectors
```

</div>

<div class="cell code" id="IkhHwdDYmSP9">

``` python
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

</div>

<div class="cell code" id="6IowJEHkne45">

``` python
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

</div>

<div class="cell code" id="QmJ9pp11nuZR">

``` python
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

</div>

<div class="cell code" id="7U0ATU2QoGn4">

``` python
'''
Alternatively, in Python 3.5+, operator @ will also work for mulitplication
'''
m_a@m_b
```

</div>

<div class="cell code" id="t7OJsHPKoZt3">

``` python
'''
For elementwise multiplications of two matrices
'''
m_a*m_b
```

</div>

<div class="cell code" id="86WZ8xIOcfS2">

``` python
```

</div>

<div class="cell markdown" id="Ojj25A1IsAlJ">

# 7.Python Conditions-Loops

</div>

<div class="cell code" id="8sWLP9bxomK2">

``` python
'''
Equals:                   a == b
Not Equals:               a != b
Less than:                a < b
Less than or equal to:    a <= b
Greater than:             a > b
Greater than or equal to: a >= b
'''
```

</div>

<div class="cell markdown" id="ASHuTB8lsklc">

## 7.1 if.....else

</div>

<div class="cell code" id="VDh56uILsrpU">

``` python
a=4
b=6
if a<b:
  print("b is greater than a")
```

</div>

<div class="cell code" id="Zz1YPC5Es3Kn">

``` python
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

</div>

<div class="cell code" id="FRaLzq2ztxly">

``` python
a=4
b=6
if a>b:
  print("a is greater than b")
else:
  print("a is not greater than b")
```

</div>

<div class="cell code" id="MLc64VW4uM1-">

``` python
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

</div>

<div class="cell code" id="7kX3E8dGvQED">

``` python
'''
one line if statement
'''
a=4
b=5
print("A") if a > b else print("=") if a == b else print("B")
```

</div>

<div class="cell markdown" id="Tonh1YnqwXWU">

## 7.2 while loop

</div>

<div class="cell code" id="13n_FMKrwBND">

``` python
i=1
while i<5:
  print (i)
  i=i+1 #i+=1
```

</div>

<div class="cell code" id="-qnos4OXwmFb">

``` python
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

</div>

<div class="cell markdown" id="fEM5XStTxncL">

## 7.3 for loop

</div>

<div class="cell code" id="6ToHUOORxkie">

``` python
alpha_b=['Apple','Boy','Cat']
for x in alpha_b: #x is a variable --->For loops iterate over a given sequence
  print(x)
```

</div>

<div class="cell code" id="Pl7QKgAmyKlg">

``` python
'''
exit the loop when x is boy
'''
alpha_b=['Apple','Boy','Cat']
for x in alpha_b:
  if x=='Boy':
    break
  print(x)
```

</div>

<div class="cell code" id="knH7LwVmzAvp">

``` python
'''
the range() Function
'''
for x in range(5):    #which means values from 0 to 4 not 0 to 5
  print(x)
```

</div>

<div class="cell code" id="boL7I2P1zTkw">

``` python
for x in range(2,5):
  print(x)
```

</div>

<div class="cell code" id="3XDBZAsnzaFs">

``` python
for x in range(0,40,10):
  print(x)
```

</div>

<div class="cell code" id="xbJI6HdSz1Oy">

``` python
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

</div>

<div class="cell markdown" id="NlL6jyjh1WVD">

# 8.Functions

</div>

<div class="cell code" id="ux-huCkH0cd9">

``` python
'''
A function is defined using the def keyword in Python
'''
```

</div>

<div class="cell code" id="JDq-U1zy482U">

``` python
def my_fun():
  print("Hey there!")
```

</div>

<div class="cell code" id="R3wws0Dzsr7B">

``` python
my_fun()
```

</div>

<div class="cell code" id="QFQrzyhV5HXT">

``` python
'''
now use the return statements to tell a function that a value should be returend
'''
def my_fun(x):
  return(x+5)
```

</div>

<div class="cell code" id="9uHFIrrx63ZG">

``` python
print(my_fun(1))
print(my_fun(2))
print(my_fun(3))
print(my_fun(4))
print(my_fun(5))
```

</div>

<div class="cell code" id="txCAGD7r6e4Q">

``` python
i=1
while i<5:
  print(my_fun(i))
  i+=1
```

</div>

<div class="cell code" id="sUTPkhhG6iqh">

``` python
def my_fun(x):
  '''
  This function return the entered number + 5
  '''
  return(x+5)
```

</div>

<div class="cell code" id="zT-Qrp1Uc9Yt">

``` python
```

</div>

<div class="cell markdown" id="KnPfxEYTCs9K">

# 9.Math

</div>

<div class="cell code" id="6Owcz5w_DGMq">

``` python
'''
Sometimes we have to perform mathematical tasks on numbers i.e. minimum, maximum,
 sqrt, ceil.,floor, pi etc.
'''
```

</div>

<div class="cell code" id="MdpI3_MCBLRS">

``` python
a=(1,2,3,4)
b=[4,3,5,7]
print(min(a))
print(max(b))
```

</div>

<div class="cell code" id="8N6oNN12DEZh">

``` python
'''
absolute (positive) value of the spacified number
'''
a=-65
print(abs(a))
```

</div>

<div class="cell code" id="SQxUI5YAEbIx">

``` python
'''
power of a number
'''
a=pow(3,4)   #3**4
print(a)
```

</div>

<div class="cell code" id="QknUoMEcEkJ5">

``` python
'''
For some extended mathemaical function, please import math first
'''
import numpy as np
```

</div>

<div class="cell code" id="MEY5gkEIE2uL">

``` python
x=np.sqrt(64)
x
```

</div>

<div class="cell code" id="WhlCoLTvE7EK">

``` python
'''ceil or floor'''
x=5.000001
print(np.ceil(x))
print(np.floor(x))
```

</div>

<div class="cell code" id="gYDM1i0_E9U9">

``` python
x=np.pi+6
x
```

</div>

<div class="cell markdown" id="7AX6RCjBrSz6">

# 10.File handling

</div>

<div class="cell markdown" id="0vs3e5u57h_l">

## 10.1 Create/write a file

</div>

<div class="cell code" id="qvAHh2gZ6-J6">

``` python
import numpy as np
```

</div>

<div class="cell code" id="I7Bd_kaVrQfz">

``` python
#To create a new file in Python, use the open() method
file = open("my_file.txt", "w")
```

</div>

<div class="cell code" id="Zny1-PAl7_pq">

``` python
file = open("my_file.txt", "w")
file.write("This is my first text file")
file.close()
```

</div>

<div class="cell code" id="QTd-Hz6NVz0Y">

``` python
#Open a Text file and write some 1-D arrays
```

</div>

<div class="cell code" id="Bhs0EOZuURCC">

``` python
a=np.array([[1],[2],[3],[4],[5],[6]])
```

</div>

<div class="cell code" id="IZQ8eT3aT8X9">

``` python
a_file = open("test.txt", "w")
for row in a:
    np.savetxt(a_file, row)
a_file.close()
```

</div>

<div class="cell code" id="z9IJIV5SZpzy">

``` python
# Single Line statement to save datapoints
a=np.array([1,2,3,4])
np.savetxt("test.txt", a)
```

</div>

<div class="cell code" id="jbJn7tkqVsRa">

``` python
aa=np.array([1,2,3,4,5])
bb=np.array([1,2,3,4,5])
np.savetxt("tt.txt", (aa,bb))
# np.savetxt("testt.txt", np.transpose([a,b]))

```

</div>

<div class="cell code" id="_WIHOMFkdMVz">

``` python
# Add header to Text File
x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("testt.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh')
```

</div>

<div class="cell code" id="qcZIMhkfk73N">

``` python
# Add footer to Text File

x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("testt.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh', footer='ff')
```

</div>

<div class="cell markdown" id="lUciek_v8ueI">

## 10.2 Read a File

</div>

<div class="cell code" id="7pxqVxR383PC">

``` python
f = open("testt.txt", "r")    #will see the way to define its location
```

</div>

<div class="cell code" id="iCoPPH639Di5">

``` python
f = open("testt.txt", "r")    #will see the way to define its location
print(f.read())
f.close()
```

</div>

<div class="cell code" id="uep8ggcr9J9Z">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt")
```

</div>

<div class="cell code" id="icEGLrJKqokg">

``` python
f
```

</div>

<div class="cell code" id="-K9qlqLerNFX">

``` python
f[0]
```

</div>

<div class="cell code" id="Q5QXORTyrIA5">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt",unpack="True")
```

</div>

<div class="cell code" id="5PYpY86LrQZQ">

``` python
f
```

</div>

<div class="cell code" id="a3g5o-_srSbY">

``` python
f[0]
```

</div>

<div class="cell markdown" id="znk6KjrN91AY">

## 10.3 Delete a File

</div>

<div class="cell code" id="MyyR-B6O96_I">

``` python
#Now to delete a file or folder you have to interact with the operating system

#The OS module in Python provides functions for interacting with the operating system

# The OS module in Python provides functions for creating and removing a directory
#(folder), fetching its contents, changing and identifying the current directory, etc.
```

</div>

<div class="cell code" id="xPZF372x967-">

``` python
import os
os.remove("my_file.txt")
```

</div>

<div class="cell code" id="ifeJ_z9Z960P">

``` python
```

</div>

<div class="cell markdown" id="wTDLQhUYXzxx">

#11.Plot data using Matplotlib

</div>

<div class="cell code" id="BtXcahFELMfi">

``` python
import matplotlib
```

</div>

<div class="cell code" id="0JXRjcPpNl_H">

``` python
print(matplotlib.__version__)  ##Check Matplotlib version
```

</div>

<div class="cell code" id="lIzAELlxNsGm">

``` python
'''
Generally we have many submodule of a Python module:
Most of the Matplotlib utilities lies under the pyplot submodule:
and are usually imported under the plt alias:
'''
```

</div>

<div class="cell code" id="lrq8JSDwoIfA">

``` python
import matplotlib.pyplot as plt #Now the Pyplot package can be referred to as plt.
import numpy as np
```

</div>

<div class="cell code" id="KtGZ9Ql5sjV1">

``` python
x=np.array([0,10])
y=np.array([0,250])
plt.plot(x,y)
```

</div>

<div class="cell code" id="55Zdfyb8uucQ">

``` python
'''
Next try to use two submodule of numpy i.e. np.arange and np.linspace along with matplotlib
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.plot(t,fun)
```

</div>

<div class="cell markdown" id="sbohRWzx0mJE">

##Set axis Labels

</div>

<div class="cell code" id="0LpwPLhgxmMk">

``` python
'''
Set matplot labels
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.xlabel("t")
plt.ylabel("$\sin(t)$")
plt.plot(t,fun)
```

</div>

<div class="cell markdown" id="KlL5dkba0rOc">

##Set Title of plot

</div>

<div class="cell code" id="jNIVTgFE3bwR">

``` python
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

</div>

<div class="cell code" id="qcPSDD6r6nij">

``` python
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

</div>

<div class="cell markdown" id="x4p9hTHK0y2o">

##Change color of plot curve

</div>

<div class="cell code" id="_Z6sgHnD66Cp">

``` python
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

</div>

<div class="cell code" id="rsVxmp8U7QCR">

``` python
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

</div>

<div class="cell code" id="Pk3VEVdG9440">

``` python
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

</div>

<div class="cell code" id="h5v3ACb_AjWH">

``` python
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

</div>

<div class="cell code" id="IVF0-i3UKD0P">

``` python
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

</div>

<div class="cell markdown" id="TJ9lv75ahdM6">

##MultiPlot in a single plot

</div>

<div class="cell code" id="5vsCTtxpNlv4">

``` python
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

</div>

<div class="cell markdown" id="rzzXp1r0kJW4">

## Add Legands

</div>

<div class="cell code" id="q2dZ0erDh1-e">

``` python
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

</div>

<div class="cell code" id="CI_SlwjjkX6e">

``` python
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

</div>

<div class="cell code" id="xAAPPrXQm_47">

``` python
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

</div>

<div class="cell markdown" id="IbWFnmIbtMhI">

## Add Grid

</div>

<div class="cell code" id="IYERRUFJn2hT">

``` python
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

</div>

<div class="cell markdown" id="sgPjNwlNvfBs">

##Rezise the image

</div>

<div class="cell code" id="5cHDdWu9uZ7y">

``` python
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

</div>

<div class="cell markdown" id="xtqLwZQTxUOy">

##Save Plot

</div>

<div class="cell code" id="XPpZbA-8voWy">

``` python
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

</div>

<div class="cell code" id="bS31gmnOd4q8">

``` python
```

</div>

<div class="cell markdown" id="9zQJ4R510WXR">

##Errorbar Plots

</div>

<div class="cell code" id="F0lG-aGzzP_Z">

``` python
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

</div>

<div class="cell markdown" id="vTzJBq0L0gou">

##Confidence levels regions

</div>

<div class="cell code" id="MP2JfL8D0jlm">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
y_err=y*0.1
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.fill_between(x, y+1.*y_err, y-1.*y_err, facecolor='#F08080', alpha=0.99)
plt.fill_between(x, y+2.*y_err, y-2.*y_err, facecolor='#F08080', alpha=0.59)
plt.fill_between(x, y+3.*y_err, y-3.*y_err, facecolor='#F08080', alpha=0.39)
```

</div>

<div class="cell code" id="iz5063RLemgm">

``` python
```

</div>

<div class="cell markdown" id="KMcpsJvQ0qGN">

##Scatter Plot

</div>

<div class="cell code" id="I3fRMxkR0qf1">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
plt.scatter(x,y)
```

</div>

<div class="cell markdown" id="_dvN4iwh0rQF">

##Histogram Plot

</div>

<div class="cell code" id="bltHawb10tF1">

``` python
x=np.array((1,2,1,2,5,3,4,5,7,8,6,7,8,3,2,1))
plt.hist(x)
```

</div>

<div class="cell markdown" id="PNKgB7Ec0tkF">

## Pie Chart Plot

</div>

<div class="cell code" id="Gs5HtfKC0wAW">

``` python
x=(45,23,37,5)
plt.pie(x)
```

</div>

<div class="cell code" id="E_NKbh8lV-uW">

``` python
#Add Label
x=(45,23,37,5)
plt.pie(x,labels=["Sample(x1)", "Sample(x2)", "Sample(x3)", "Sample(x4)"])
```

</div>

<div class="cell markdown" id="kkxpBTn2kUCX">

##Three-dimensional Contour Plots

</div>

<div class="cell code" id="Dlj2mC8TkKOe">

``` python
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

</div>

<div class="cell markdown" id="avRmmpigfECg">

#12.Dataframe using Pandas

</div>

<div class="cell markdown" id="Qv29RWEOf-0o">

## Import Packages

</div>

<div class="cell code" id="LMLmh-_cgA18">

``` python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

</div>

<div class="cell markdown" id="bS6Xg3Nowmao">

##Create a dataframe

</div>

<div class="cell code" id="v_0wp4Z5vqrG">

``` python
df=pd.DataFrame(
    {
        "Name":["Tom","Jerry","Sam"],
        "Age" :[2,5,8],
     "Color":["Black","White","Brown"]
    }
)
```

</div>

<div class="cell code" id="LPlk8AkmCJ8l">

``` python
df
```

</div>

<div class="cell code" id="lulcy-dJCT6S">

``` python
df['Age']
```

</div>

<div class="cell code" id="8YiBCCB0R6IS">

``` python
df['Color']
```

</div>

<div class="cell code" id="uUCKXo5IR9w8">

``` python
df['Age'].max()
```

</div>

<div class="cell markdown" id="t6eCk9RFxhkH">

##Print Full Dataframe

</div>

<div class="cell code" id="-KZonCgDgGvv">

``` python
df_covid=pd.read_csv("https://raw.githubusercontent.com/darshanbeniwal/Statistical_Cosmology_using_Python_ICARD_2021/main/Week_9_Feb_01_2022/Covid_19_Jan_16_2022.csv")
```

</div>

<div class="cell code" id="p9955jIJSlHV">

``` python
df_covid
```

</div>

<div class="cell code" id="DWgwQzq-Styp">

``` python
df_covid.dtypes
```

</div>

<div class="cell markdown" id="Wet5qTepxkrk">

## Print the selected Column

</div>

<div class="cell code" id="jHuaBGTGkNAN">

``` python
df_covid.head(5)
```

</div>

<div class="cell code" id="ulrTr0HtkZqi">

``` python
df_covid.tail(5)
```

</div>

<div class="cell code" id="XkUsLqWvy6Xp">

``` python
df=df_covid['Total_Cases']
```

</div>

<div class="cell code" id="A8E4KdJFTPu8">

``` python
df
```

</div>

<div class="cell code" id="JSvkM9wRTSc2">

``` python
df_covid[['Country','Total_Cases']]
```

</div>

<div class="cell code" id="QkqXI2riTSZa">

``` python
df_covid[['Country','Total_Cases']].head(5)
```

</div>

<div class="cell code" id="pKQTOxtCTSVV">

``` python
df_covid.loc[df_covid['Total_Cases']<1000]
```

</div>

<div class="cell code" id="-k2lEojTT4fC">

``` python
len(df_covid.loc[df_covid['Total_Cases']<1000])
```

</div>

<div class="cell code" id="0QL_QCVAT4aS">

``` python
df_covid.corr()
```

</div>

<div class="cell code" id="Tkf9Tfa1hJZe">

``` python
```

</div>

<div class="cell markdown" id="4QpzJINEfsP7">

#13.Random Number Operations

</div>

<div class="cell code" id="-EKzy78pixq_">

``` python
import random
```

</div>

<div class="cell markdown" id="zo-I4JvIfzia">

## Random Items from list, tuple & string

</div>

<div class="cell code" id="Rt3S5doxjQCX">

``` python
list=[0,2,4,6,8]
string="cosmology"
tuple=('Astronomy', 'Astrophysics', 'Cosmology', 'Dark Energy', 'Dark Matter')
```

</div>

<div class="cell code" id="WJ9AD15ZgCbv">

``` python
print(random.choice(list))
```

</div>

<div class="cell code" id="AWGM8PBOgCY2">

``` python
print(random.choice(string))
```

</div>

<div class="cell code" id="YNgq2bwngCVI">

``` python
print(random.choice(tuple))
```

</div>

<div class="cell code" id="GuJNXHu9e-56">

``` python
random.random()
```

</div>

<div class="cell markdown" id="JoX5hDsKjCe4">

## Random Shuffle

</div>

<div class="cell code" id="dZ5GNKCRiXlS">

``` python
random.shuffle(list)  #shuffle will only work in list-->It changes the original list
print(list)
```

</div>

<div class="cell markdown" id="rBo4nkqB-x6P">

##Random Sampling

</div>

<div class="cell code" id="Qx0hicv3-vtW">

``` python
list=[0,2,4,6,8]
random.sample(list,3) #return a particluar list of items without any chnage in origi list
```

</div>

<div class="cell markdown" id="nMwo06xIwyQ3">

## Generate Random Numbers

</div>

<div class="cell code" id="xBu0GoHpuYOG">

``` python
print(random.randint(0,5))  #Generate a Random Number
```

</div>

<div class="cell code" id="PYs7Wd-fwtdJ">

``` python
print([random.randint(0,10) for i in range(5)]) #Generate a list of Random Number List
```

</div>

<div class="cell code" id="PyZ2pKvxxVHR">

``` python
#Alternatively, for Random number list, you can use numpy as
np.random.randint(0,10,5)
```

</div>

<div class="cell code" id="lKOw4TsDzz6i">

``` python
np.random.randint(0,10,size=5) #Basically the last arguments denotes the size of list
```

</div>

<div class="cell code" id="eNMKtneY4Tnr">

``` python
np.random.randint(0,10,size=(2,5))
```

</div>

<div class="cell code" id="nRFje-EE-QLO">

``` python
#Suppose you want to generate random floating values using randint
np.random.randint(0,10,size=(2,5)).astype("float")/10
```

</div>

<div class="cell code" id="y8SMKj3O4smL">

``` python
#Alternatively, one can use random_sample
np.random.random_sample(size=(2,5))
```

</div>

<div class="cell code" id="Fmj3yyKVi1FD">

``` python
from IPython.display import clear_output
clear_output(wait=True)
```

</div>

<div class="cell code" id="HoKxdn8yAxwa">

``` python
```

</div>
