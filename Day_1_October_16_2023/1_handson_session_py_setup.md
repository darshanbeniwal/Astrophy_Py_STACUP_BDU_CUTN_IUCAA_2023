---
jupyter:
  colab:
    toc_visible: true
  kernelspec:
    display_name: Python 3
    name: python3
  language_info:
    name: python
  nbformat: 4
  nbformat_minor: 0
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

<div class="cell code" execution_count="2"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:36}"
id="6Owcz5w_DGMq" outputId="46f5acfa-77aa-4c8d-c610-b95a3dc94853">

``` python
'''
Sometimes we have to perform mathematical tasks on numbers i.e. minimum, maximum,
 sqrt, ceil.,floor, pi etc.
'''
```

<div class="output execute_result" execution_count="2">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" execution_count="3"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="MdpI3_MCBLRS" outputId="9cbef3ec-0f84-4d2d-b20e-e7f9d1cb5e9d">

``` python
a=(1,2,3,4)
b=[4,3,5,7]
print(min(a))
print(max(b))
```

<div class="output stream stdout">

    1
    7

</div>

</div>

<div class="cell code" execution_count="4"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="8N6oNN12DEZh" outputId="df329172-f31d-48bd-df7d-96a9ab29c84e">

``` python
'''
absolute (positive) value of the spacified number
'''
a=-65
print(abs(a))
```

<div class="output stream stdout">

    65

</div>

</div>

<div class="cell code" execution_count="5"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="SQxUI5YAEbIx" outputId="8ad12d98-bf9e-4977-e8d2-16170665c39c">

``` python
'''
power of a number
'''
a=pow(3,4)   #3**4
print(a)
```

<div class="output stream stdout">

    81

</div>

</div>

<div class="cell code" execution_count="6" id="QknUoMEcEkJ5">

``` python
'''
For some extended mathemaical function, please import math first
'''
import numpy as np
```

</div>

<div class="cell code" execution_count="7"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="MEY5gkEIE2uL" outputId="2f3b12c0-1ec1-4983-9f9b-320c344cdfdd">

``` python
x=np.sqrt(64)
x
```

<div class="output execute_result" execution_count="7">

    8.0

</div>

</div>

<div class="cell code" execution_count="8"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="WhlCoLTvE7EK" outputId="2f9345da-85f2-4b0b-d0c0-9f13fddd0436">

``` python
'''ceil or floor'''
x=5.000001
print(np.ceil(x))
print(np.floor(x))
```

<div class="output stream stdout">

    6.0
    5.0

</div>

</div>

<div class="cell code" execution_count="9"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="gYDM1i0_E9U9" outputId="afbfcfcc-df15-4c4c-97ea-44f3d7dcff94">

``` python
x=np.pi+6
x
```

<div class="output execute_result" execution_count="9">

    9.141592653589793

</div>

</div>

<div class="cell markdown" id="7AX6RCjBrSz6">

# 10.File handling

</div>

<div class="cell markdown" id="0vs3e5u57h_l">

## 10.1 Create/write a file

</div>

<div class="cell code" execution_count="10" id="qvAHh2gZ6-J6">

``` python
import numpy as np
```

</div>

<div class="cell code" execution_count="11" id="I7Bd_kaVrQfz">

``` python
#To create a new file in Python, use the open() method
file = open("my_file.txt", "w")
```

</div>

<div class="cell code" execution_count="12" id="Zny1-PAl7_pq">

``` python
file = open("my_file.txt", "w")
file.write("This is my first text file")
file.close()
```

</div>

<div class="cell code" execution_count="13" id="QTd-Hz6NVz0Y">

``` python
#Open a Text file and write some 1-D arrays
```

</div>

<div class="cell code" execution_count="14" id="Bhs0EOZuURCC">

``` python
a=np.array([[1],[2],[3],[4],[5],[6]])
```

</div>

<div class="cell code" execution_count="15" id="IZQ8eT3aT8X9">

``` python
a_file = open("test.txt", "w")
for row in a:
    np.savetxt(a_file, row)
a_file.close()
```

</div>

<div class="cell code" execution_count="16" id="z9IJIV5SZpzy">

``` python
# Single Line statement to save datapoints
a=np.array([1,2,3,4])
np.savetxt("test.txt", a)
```

</div>

<div class="cell code" execution_count="17" id="jbJn7tkqVsRa">

``` python
aa=np.array([1,2,3,4,5])
bb=np.array([1,2,3,4,5])
np.savetxt("tt.txt", (aa,bb))
# np.savetxt("testt.txt", np.transpose([a,b]))

```

</div>

<div class="cell code" execution_count="18" id="_WIHOMFkdMVz">

``` python
# Add header to Text File
x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("testt.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh')
```

</div>

<div class="cell code" execution_count="19" id="qcZIMhkfk73N">

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

<div class="cell code" execution_count="20" id="7pxqVxR383PC">

``` python
f = open("testt.txt", "r")    #will see the way to define its location
```

</div>

<div class="cell code" execution_count="21"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="iCoPPH639Di5" outputId="a678acc4-7ee8-4813-a1f6-12ab10067506">

``` python
f = open("testt.txt", "r")    #will see the way to define its location
print(f.read())
f.close()
```

<div class="output stream stdout">

    # hhh
    0.000000 0.000000
    0.111111 0.110883
    0.222222 0.220398
    0.333333 0.327195
    0.444444 0.429956
    0.555556 0.527415
    0.666667 0.618370
    0.777778 0.701698
    0.888889 0.776372
    1.000000 0.841471
    # ff

</div>

</div>

<div class="cell code" execution_count="22" id="uep8ggcr9J9Z">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt")
```

</div>

<div class="cell code" execution_count="23"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="icEGLrJKqokg" outputId="1cd5e26c-dee7-4a49-c50e-1fd5befeedab">

``` python
f
```

<div class="output execute_result" execution_count="23">

    array([[0.      , 0.      ],
           [0.111111, 0.110883],
           [0.222222, 0.220398],
           [0.333333, 0.327195],
           [0.444444, 0.429956],
           [0.555556, 0.527415],
           [0.666667, 0.61837 ],
           [0.777778, 0.701698],
           [0.888889, 0.776372],
           [1.      , 0.841471]])

</div>

</div>

<div class="cell code" execution_count="24"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="-K9qlqLerNFX" outputId="c2506ce6-5e1b-4c45-e667-7d93f55e8ff7">

``` python
f[0]
```

<div class="output execute_result" execution_count="24">

    array([0., 0.])

</div>

</div>

<div class="cell code" execution_count="25" id="Q5QXORTyrIA5">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt",unpack="True")
```

</div>

<div class="cell code" execution_count="26"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="5PYpY86LrQZQ" outputId="8a136e02-e3c7-4161-d327-ad95b12e7dac">

``` python
f
```

<div class="output execute_result" execution_count="26">

    array([[0.      , 0.111111, 0.222222, 0.333333, 0.444444, 0.555556,
            0.666667, 0.777778, 0.888889, 1.      ],
           [0.      , 0.110883, 0.220398, 0.327195, 0.429956, 0.527415,
            0.61837 , 0.701698, 0.776372, 0.841471]])

</div>

</div>

<div class="cell code" execution_count="27"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="a3g5o-_srSbY" outputId="3e31d217-6df5-427e-a153-ec02267aecb6">

``` python
f[0]
```

<div class="output execute_result" execution_count="27">

    array([0.      , 0.111111, 0.222222, 0.333333, 0.444444, 0.555556,
           0.666667, 0.777778, 0.888889, 1.      ])

</div>

</div>

<div class="cell markdown" id="znk6KjrN91AY">

## 10.3 Delete a File

</div>

<div class="cell code" execution_count="28" id="MyyR-B6O96_I">

``` python
#Now to delete a file or folder you have to interact with the operating system

#The OS module in Python provides functions for interacting with the operating system

# The OS module in Python provides functions for creating and removing a directory
#(folder), fetching its contents, changing and identifying the current directory, etc.
```

</div>

<div class="cell code" execution_count="29" id="xPZF372x967-">

``` python
import os
os.remove("my_file.txt")
```

</div>

<div class="cell code" execution_count="29" id="ifeJ_z9Z960P">

``` python
```

</div>

<div class="cell markdown" id="wTDLQhUYXzxx">

#11.Plot data using Matplotlib

</div>

<div class="cell code" execution_count="30" id="BtXcahFELMfi">

``` python
import matplotlib
```

</div>

<div class="cell code" execution_count="31"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="0JXRjcPpNl_H" outputId="e740eff8-7cb1-425e-eeaa-71388a2ac5c2">

``` python
print(matplotlib.__version__)  ##Check Matplotlib version
```

<div class="output stream stdout">

    3.7.1

</div>

</div>

<div class="cell code" execution_count="32"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="lIzAELlxNsGm" outputId="16138220-21df-40a7-f1d4-1c40ffcd4744">

``` python
'''
Generally we have many submodule of a Python module:
Most of the Matplotlib utilities lies under the pyplot submodule:
and are usually imported under the plt alias:
'''
```

<div class="output execute_result" execution_count="32">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" execution_count="33" id="lrq8JSDwoIfA">

``` python
import matplotlib.pyplot as plt #Now the Pyplot package can be referred to as plt.
import numpy as np
```

</div>

<div class="cell code" execution_count="34"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="KtGZ9Ql5sjV1" outputId="5c0c49d3-1c96-44d4-d195-db9b833be998">

``` python
x=np.array([0,10])
y=np.array([0,250])
plt.plot(x,y)
```

<div class="output execute_result" execution_count="34">

    [<matplotlib.lines.Line2D at 0x7b19a8221a50>]

</div>

<div class="output display_data">

![](efdec09461a636380c9bd8d589eac27dc2e05dfb.png)

</div>

</div>

<div class="cell code" execution_count="35"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="55Zdfyb8uucQ" outputId="2af3fb12-7501-4cc3-9250-78e41590c713">

``` python
'''
Next try to use two submodule of numpy i.e. np.arange and np.linspace along with matplotlib
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.plot(t,fun)
```

<div class="output execute_result" execution_count="35">

    [<matplotlib.lines.Line2D at 0x7b19a810ed40>]

</div>

<div class="output display_data">

![](b3fecf4077926b4df8f201e8a635e5835f3800ea.png)

</div>

</div>

<div class="cell markdown" id="sbohRWzx0mJE">

##Set axis Labels

</div>

<div class="cell code" execution_count="36"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:466}"
id="0LpwPLhgxmMk" outputId="76f39d9f-6782-41e7-c2c7-38f30f44facd">

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

<div class="output execute_result" execution_count="36">

    [<matplotlib.lines.Line2D at 0x7b19a81a3c40>]

</div>

<div class="output display_data">

![](25899ac15dad6f469ff7b87bcdce58a0776cacbb.png)

</div>

</div>

<div class="cell markdown" id="KlL5dkba0rOc">

##Set Title of plot

</div>

<div class="cell code" execution_count="37"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="jNIVTgFE3bwR" outputId="2fb9d55f-805f-4a81-fb0d-490055312245">

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

<div class="output execute_result" execution_count="37">

    [<matplotlib.lines.Line2D at 0x7b1998fbf880>]

</div>

<div class="output display_data">

![](c5feed8cdb7aeb9b6abfbed252d0d9b84d8ee27b.png)

</div>

</div>

<div class="cell code" execution_count="38"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="qcPSDD6r6nij" outputId="941e9272-0fb5-4ac7-d279-7036e7d35a21">

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

<div class="output execute_result" execution_count="38">

    [<matplotlib.lines.Line2D at 0x7b199838a2c0>]

</div>

<div class="output display_data">

![](c5feed8cdb7aeb9b6abfbed252d0d9b84d8ee27b.png)

</div>

</div>

<div class="cell markdown" id="x4p9hTHK0y2o">

##Change color of plot curve

</div>

<div class="cell code" execution_count="39"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="_Z6sgHnD66Cp" outputId="9b2f5b89-1b5d-4662-cf22-d0306af8fe14">

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

<div class="output execute_result" execution_count="39">

    [<matplotlib.lines.Line2D at 0x7b1998f02ce0>]

</div>

<div class="output display_data">

![](69c7a54f6bf455bf88639cd94aa1d59f4fae6a08.png)

</div>

</div>

<div class="cell code" execution_count="40"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="rsVxmp8U7QCR" outputId="02942569-a17a-47df-9443-cff142688244">

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

<div class="output execute_result" execution_count="40">

    [<matplotlib.lines.Line2D at 0x7b199829d4e0>]

</div>

<div class="output display_data">

![](ebc96a109c3d62a36c9816b02a6474ac03f0bbd9.png)

</div>

</div>

<div class="cell code" execution_count="41"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:70}"
id="Pk3VEVdG9440" outputId="3bb3a16a-e63d-407a-8494-6140943de6f5">

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

<div class="output execute_result" execution_count="41">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" execution_count="42"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="h5v3ACb_AjWH" outputId="ea9503a7-2578-4420-fbd3-f6df7a8448a3">

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

<div class="output execute_result" execution_count="42">

    [<matplotlib.lines.Line2D at 0x7b199814c3d0>]

</div>

<div class="output display_data">

![](7cb03316adea4318df0f94cc93ce1625281c0f37.png)

</div>

</div>

<div class="cell code" execution_count="43"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="IVF0-i3UKD0P" outputId="06307e25-dd16-460c-b627-e230172a4bd3">

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

<div class="output execute_result" execution_count="43">

    [<matplotlib.lines.Line2D at 0x7b19981d7a90>]

</div>

<div class="output display_data">

![](611caee9f5d67d03c372cf627eb6de40e9669147.png)

</div>

</div>

<div class="cell markdown" id="TJ9lv75ahdM6">

##MultiPlot in a single plot

</div>

<div class="cell code" execution_count="44"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="5vsCTtxpNlv4" outputId="471b1caf-99a8-45d4-ff14-e09f113496dc">

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

<div class="output execute_result" execution_count="44">

    [<matplotlib.lines.Line2D at 0x7b1975f91de0>]

</div>

<div class="output display_data">

![](9e4bce0aa666b983d6ffb428c15ecf7768c5d71a.png)

</div>

</div>

<div class="cell markdown" id="rzzXp1r0kJW4">

## Add Legands

</div>

<div class="cell code" execution_count="45"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="q2dZ0erDh1-e" outputId="535eea23-c547-4583-b36b-e7fdd9b69e51">

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

<div class="output execute_result" execution_count="45">

    <matplotlib.legend.Legend at 0x7b1975e40820>

</div>

<div class="output display_data">

![](52ebdaf45c4a9cb0e53903d2c2d3fde9c320a1c3.png)

</div>

</div>

<div class="cell code" execution_count="46"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="CI_SlwjjkX6e" outputId="4a13d3e3-118c-4434-df77-b05f92d3ba5e">

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

<div class="output execute_result" execution_count="46">

    <matplotlib.legend.Legend at 0x7b1975e41ff0>

</div>

<div class="output display_data">

![](37efd18e6422db69fa705a3e1df6a515a93d4204.png)

</div>

</div>

<div class="cell code" execution_count="47"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="xAAPPrXQm_47" outputId="5b65db41-caad-413d-fa78-ea5d97f35121">

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

<div class="output execute_result" execution_count="47">

    <matplotlib.legend.Legend at 0x7b197556e5f0>

</div>

<div class="output display_data">

![](109a24a58add344e21b7cfc58b1d475051454feb.png)

</div>

</div>

<div class="cell markdown" id="IbWFnmIbtMhI">

## Add Grid

</div>

<div class="cell code" execution_count="48"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:474}"
id="IYERRUFJn2hT" outputId="28c32e81-09eb-4e6d-ad10-2448fa8be6d6">

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

<div class="output display_data">

![](861949dc492275bd81ebe52bbb7073c0af2eadea.png)

</div>

</div>

<div class="cell markdown" id="sgPjNwlNvfBs">

##Rezise the image

</div>

<div class="cell code" execution_count="49"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:720}"
id="5cHDdWu9uZ7y" outputId="bc8b4d91-6944-47e1-d2fb-4fea1457c456">

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

<div class="output display_data">

![](6f79c66b475d4189204e3ba3d0f93face300b7e6.png)

</div>

</div>

<div class="cell markdown" id="xtqLwZQTxUOy">

##Save Plot

</div>

<div class="cell code" execution_count="50"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:720}"
id="XPpZbA-8voWy" outputId="bb44f6b8-e6f5-4e7a-d628-d6de44dc7e3c">

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

<div class="output display_data">

![](6f79c66b475d4189204e3ba3d0f93face300b7e6.png)

</div>

</div>

<div class="cell code" execution_count="50" id="bS31gmnOd4q8">

``` python
```

</div>

<div class="cell markdown" id="9zQJ4R510WXR">

##Errorbar Plots

</div>

<div class="cell code" execution_count="51"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:466}"
id="F0lG-aGzzP_Z" outputId="bf014733-6272-47a9-ea74-3abaa9b56822">

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

<div class="output execute_result" execution_count="51">

    Text(0, 0.5, 'y')

</div>

<div class="output display_data">

![](c4051b3dfc9b6105f48e90ca93ca890e46a6ab01.png)

</div>

</div>

<div class="cell markdown" id="vTzJBq0L0gou">

##Confidence levels regions

</div>

<div class="cell code" execution_count="52"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="MP2JfL8D0jlm" outputId="ae9bb29d-e927-405c-97c9-d5caec4b7c9b">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
y_err=y*0.1
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.fill_between(x, y+1.*y_err, y-1.*y_err, facecolor='#F08080', alpha=0.99)
plt.fill_between(x, y+2.*y_err, y-2.*y_err, facecolor='#F08080', alpha=0.59)
plt.fill_between(x, y+3.*y_err, y-3.*y_err, facecolor='#F08080', alpha=0.39)
```

<div class="output execute_result" execution_count="52">

    <matplotlib.collections.PolyCollection at 0x7b1974f2f4f0>

</div>

<div class="output display_data">

![](abbcfc82307ac0ca2ea18ff7dbccd9a0ba4dc6ec.png)

</div>

</div>

<div class="cell code" execution_count="52" id="iz5063RLemgm">

``` python
```

</div>

<div class="cell markdown" id="KMcpsJvQ0qGN">

##Scatter Plot

</div>

<div class="cell code" execution_count="53"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="I3fRMxkR0qf1" outputId="a00eebbf-898b-4459-9aed-5a55fd7d7066">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
plt.scatter(x,y)
```

<div class="output execute_result" execution_count="53">

    <matplotlib.collections.PathCollection at 0x7b19751d3fd0>

</div>

<div class="output display_data">

![](b084fb6ac9ccd77797e2f0e4f3642c03c6c96cc0.png)

</div>

</div>

<div class="cell markdown" id="_dvN4iwh0rQF">

##Histogram Plot

</div>

<div class="cell code" execution_count="54"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:482}"
id="bltHawb10tF1" outputId="bfbb1fc7-1bf7-46a4-82c0-38f77fbb8862">

``` python
x=np.array((1,2,1,2,5,3,4,5,7,8,6,7,8,3,2,1))
plt.hist(x)
```

<div class="output execute_result" execution_count="54">

    (array([3., 3., 2., 0., 1., 2., 0., 1., 2., 2.]),
     array([1. , 1.7, 2.4, 3.1, 3.8, 4.5, 5.2, 5.9, 6.6, 7.3, 8. ]),
     <BarContainer object of 10 artists>)

</div>

<div class="output display_data">

![](87b82aa8399ca23bf05c4d32b35140d7dab8da63.png)

</div>

</div>

<div class="cell markdown" id="PNKgB7Ec0tkF">

## Pie Chart Plot

</div>

<div class="cell code" execution_count="55"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:545}"
id="Gs5HtfKC0wAW" outputId="2229e049-0d7b-41e9-86aa-74638597c8a1">

``` python
x=(45,23,37,5)
plt.pie(x)
```

<div class="output execute_result" execution_count="55">

    ([<matplotlib.patches.Wedge at 0x7b197519d120>,
      <matplotlib.patches.Wedge at 0x7b197519d030>,
      <matplotlib.patches.Wedge at 0x7b197519d9f0>,
      <matplotlib.patches.Wedge at 0x7b197519de70>],
     [Text(0.30990582150899426, 1.0554422683381766, ''),
      Text(-1.0959649072339253, -0.09413247108056673, ''),
      Text(0.24914641133865234, -1.0714131162707834, ''),
      Text(1.0888035854028022, -0.15654632673430272, '')])

</div>

<div class="output display_data">

![](166917faf2f3d09385975c218609869246fa8360.png)

</div>

</div>

<div class="cell code" execution_count="56"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:545}"
id="E_NKbh8lV-uW" outputId="a1702f96-f141-4e08-882e-35efb5650ab4">

``` python
#Add Label
x=(45,23,37,5)
plt.pie(x,labels=["Sample(x1)", "Sample(x2)", "Sample(x3)", "Sample(x4)"])
```

<div class="output execute_result" execution_count="56">

    ([<matplotlib.patches.Wedge at 0x7b1974fcf610>,
      <matplotlib.patches.Wedge at 0x7b1974fcf520>,
      <matplotlib.patches.Wedge at 0x7b1974fcfee0>,
      <matplotlib.patches.Wedge at 0x7b197500c3a0>],
     [Text(0.30990582150899426, 1.0554422683381766, 'Sample(x1)'),
      Text(-1.0959649072339253, -0.09413247108056673, 'Sample(x2)'),
      Text(0.24914641133865234, -1.0714131162707834, 'Sample(x3)'),
      Text(1.0888035854028022, -0.15654632673430272, 'Sample(x4)')])

</div>

<div class="output display_data">

![](9dfae562602df0f62e8cf71269a49e6ed26ffa82.png)

</div>

</div>

<div class="cell markdown" id="kkxpBTn2kUCX">

##Three-dimensional Contour Plots

</div>

<div class="cell code" execution_count="57"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:415}"
id="Dlj2mC8TkKOe" outputId="4daa11b4-d8f1-4125-b013-025969e823a2">

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

<div class="output display_data">

![](dd3826f8cd3666fc4e6678daffe50e1da3b254b5.png)

</div>

</div>

<div class="cell markdown" id="avRmmpigfECg">

#12.Dataframe using Pandas

</div>

<div class="cell markdown" id="Qv29RWEOf-0o">

## Import Packages

</div>

<div class="cell code" execution_count="58" id="LMLmh-_cgA18">

``` python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

</div>

<div class="cell markdown" id="bS6Xg3Nowmao">

##Create a dataframe

</div>

<div class="cell code" execution_count="59" id="v_0wp4Z5vqrG">

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

<div class="cell code" execution_count="60"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
id="LPlk8AkmCJ8l" outputId="f006035c-3085-45ce-a399-6b8eab09ce35">

``` python
df
```

<div class="output execute_result" execution_count="60">

        Name  Age  Color
    0    Tom    2  Black
    1  Jerry    5  White
    2    Sam    8  Brown

</div>

</div>

<div class="cell code" execution_count="61"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="lulcy-dJCT6S" outputId="ad2419c9-0e30-4bbd-a0bc-9100f752b1f6">

``` python
df['Age']
```

<div class="output execute_result" execution_count="61">

    0    2
    1    5
    2    8
    Name: Age, dtype: int64

</div>

</div>

<div class="cell code" execution_count="62"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="8YiBCCB0R6IS" outputId="7186879d-8740-419a-ccea-fb858fd36aba">

``` python
df['Color']
```

<div class="output execute_result" execution_count="62">

    0    Black
    1    White
    2    Brown
    Name: Color, dtype: object

</div>

</div>

<div class="cell code" execution_count="63"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="uUCKXo5IR9w8" outputId="6eadce9f-5ee1-42c2-db03-22f241d59194">

``` python
df['Age'].max()
```

<div class="output execute_result" execution_count="63">

    8

</div>

</div>

<div class="cell markdown" id="t6eCk9RFxhkH">

##Print Full Dataframe

</div>

<div class="cell code" execution_count="64" id="-KZonCgDgGvv">

``` python
df_covid=pd.read_csv("https://raw.githubusercontent.com/darshanbeniwal/Statistical_Cosmology_using_Python_ICARD_2021/main/Week_9_Feb_01_2022/Covid_19_Jan_16_2022.csv")
```

</div>

<div class="cell code" execution_count="65"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:513}"
id="p9955jIJSlHV" outputId="2c1dd2fe-bf4f-41cd-d751-00d4ff30deef">

``` python
df_covid
```

<div class="output execute_result" execution_count="65">

         Sr. No.           Country  Total_Cases  Total_Deaths  Total_Recovered  \
    0          0             World    326673326     5553522.0      266411376.0   
    1          1               USA     66664283      873149.0       43059089.0   
    2          2             India     37122164      486094.0       35085721.0   
    3          3            Brazil     22975723      621007.0       21710831.0   
    4          4                UK     15146356      151899.0       11299374.0   
    ..       ...               ...          ...           ...              ...   
    220      220  Marshall Islands            7           NaN              4.0   
    221      221             Samoa            3           NaN              3.0   
    222      222      Saint Helena            2           NaN              2.0   
    223      223        Micronesia            1           NaN              1.0   
    224      224             Tonga            1           NaN              1.0   

         Active_Cases  Tot Cases_per_1M pop  Deaths_per_1M pop  Total_Tests  \
    0      54708428.0               41909.0              713.0          NaN   
    1      22732045.0              199601.0             2614.0  857726168.0   
    2       1550349.0               26499.0              347.0  700712824.0   
    3        643885.0              106922.0             2890.0   63776166.0   
    4       3695083.0              221326.0             2220.0  430233640.0   
    ..            ...                   ...                ...          ...   
    220           3.0                 117.0                NaN          NaN   
    221           0.0                  15.0                NaN          NaN   
    222           0.0                 328.0                NaN          NaN   
    223           0.0                   9.0                NaN          NaN   
    224           0.0                   9.0                NaN          NaN   

         Tests_per_1M pop    Population  
    0                 NaN           NaN  
    1           2568137.0  3.339877e+08  
    2            500200.0  1.400865e+09  
    3            296795.0  2.148830e+08  
    4           6286799.0  6.843446e+07  
    ..                ...           ...  
    220               NaN  5.980400e+04  
    221               NaN  2.004420e+05  
    222               NaN  6.105000e+03  
    223               NaN  1.168770e+05  
    224               NaN  1.075370e+05  

    [225 rows x 11 columns]

</div>

</div>

<div class="cell code" execution_count="66"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="DWgwQzq-Styp" outputId="d32ecf2b-c1d9-46ac-9986-75b997d62ced">

``` python
df_covid.dtypes
```

<div class="output execute_result" execution_count="66">

    Sr. No.                   int64
    Country                  object
    Total_Cases               int64
    Total_Deaths            float64
    Total_Recovered         float64
    Active_Cases            float64
    Tot Cases_per_1M pop    float64
    Deaths_per_1M pop       float64
    Total_Tests             float64
    Tests_per_1M pop        float64
    Population              float64
    dtype: object

</div>

</div>

<div class="cell markdown" id="Wet5qTepxkrk">

## Print the selected Column

</div>

<div class="cell code" execution_count="67"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:261}"
id="jHuaBGTGkNAN" outputId="a4f00341-ea96-4e33-887e-3f6918c63d24">

``` python
df_covid.head(5)
```

<div class="output execute_result" execution_count="67">

       Sr. No. Country  Total_Cases  Total_Deaths  Total_Recovered  Active_Cases  \
    0        0   World    326673326     5553522.0      266411376.0    54708428.0   
    1        1     USA     66664283      873149.0       43059089.0    22732045.0   
    2        2   India     37122164      486094.0       35085721.0     1550349.0   
    3        3  Brazil     22975723      621007.0       21710831.0      643885.0   
    4        4      UK     15146356      151899.0       11299374.0     3695083.0   

       Tot Cases_per_1M pop  Deaths_per_1M pop  Total_Tests  Tests_per_1M pop  \
    0               41909.0              713.0          NaN               NaN   
    1              199601.0             2614.0  857726168.0         2568137.0   
    2               26499.0              347.0  700712824.0          500200.0   
    3              106922.0             2890.0   63776166.0          296795.0   
    4              221326.0             2220.0  430233640.0         6286799.0   

         Population  
    0           NaN  
    1  3.339877e+08  
    2  1.400865e+09  
    3  2.148830e+08  
    4  6.843446e+07  

</div>

</div>

<div class="cell code" execution_count="68"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:295}"
id="ulrTr0HtkZqi" outputId="44824a4e-eb62-4d6a-d013-d7a9102b613e">

``` python
df_covid.tail(5)
```

<div class="output execute_result" execution_count="68">

         Sr. No.           Country  Total_Cases  Total_Deaths  Total_Recovered  \
    220      220  Marshall Islands            7           NaN              4.0   
    221      221             Samoa            3           NaN              3.0   
    222      222      Saint Helena            2           NaN              2.0   
    223      223        Micronesia            1           NaN              1.0   
    224      224             Tonga            1           NaN              1.0   

         Active_Cases  Tot Cases_per_1M pop  Deaths_per_1M pop  Total_Tests  \
    220           3.0                 117.0                NaN          NaN   
    221           0.0                  15.0                NaN          NaN   
    222           0.0                 328.0                NaN          NaN   
    223           0.0                   9.0                NaN          NaN   
    224           0.0                   9.0                NaN          NaN   

         Tests_per_1M pop  Population  
    220               NaN     59804.0  
    221               NaN    200442.0  
    222               NaN      6105.0  
    223               NaN    116877.0  
    224               NaN    107537.0  

</div>

</div>

<div class="cell code" execution_count="69" id="XkUsLqWvy6Xp">

``` python
df=df_covid['Total_Cases']
```

</div>

<div class="cell code" execution_count="70"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="A8E4KdJFTPu8" outputId="5f04812b-2722-4665-8775-36ebcee295d7">

``` python
df
```

<div class="output execute_result" execution_count="70">

    0      326673326
    1       66664283
    2       37122164
    3       22975723
    4       15146356
             ...    
    220            7
    221            3
    222            2
    223            1
    224            1
    Name: Total_Cases, Length: 225, dtype: int64

</div>

</div>

<div class="cell code" execution_count="71"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:423}"
id="JSvkM9wRTSc2" outputId="991822ac-8eed-4522-fe83-bf0144e08cab">

``` python
df_covid[['Country','Total_Cases']]
```

<div class="output execute_result" execution_count="71">

                  Country  Total_Cases
    0               World    326673326
    1                 USA     66664283
    2               India     37122164
    3              Brazil     22975723
    4                  UK     15146356
    ..                ...          ...
    220  Marshall Islands            7
    221             Samoa            3
    222      Saint Helena            2
    223        Micronesia            1
    224             Tonga            1

    [225 rows x 2 columns]

</div>

</div>

<div class="cell code" execution_count="72"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:206}"
id="QkqXI2riTSZa" outputId="4311e3ef-83e2-4540-9296-363a441c497b">

``` python
df_covid[['Country','Total_Cases']].head(5)
```

<div class="output execute_result" execution_count="72">

      Country  Total_Cases
    0   World    326673326
    1     USA     66664283
    2   India     37122164
    3  Brazil     22975723
    4      UK     15146356

</div>

</div>

<div class="cell code" execution_count="73"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:828}"
id="pKQTOxtCTSVV" outputId="14eecf4a-8bf4-4f79-9cc9-9597e05dfa79">

``` python
df_covid.loc[df_covid['Total_Cases']<1000]
```

<div class="output execute_result" execution_count="73">

         Sr. No.                Country  Total_Cases  Total_Deaths  \
    208      208       Diamond Princess          712          13.0   
    209      209      Wallis and Futuna          454           7.0   
    210      210  Saint Pierre Miquelon          415           NaN   
    211      211             Montserrat          129           1.0   
    212      212       Falkland Islands           85           NaN   
    213      213                  Macao           79           NaN   
    214      214                  Palau           64           NaN   
    215      215           Vatican City           27           NaN   
    216      216        Solomon Islands           25           NaN   
    217      217         Western Sahara           10           1.0   
    218      218             MS Zaandam            9           2.0   
    219      219                Vanuatu            7           1.0   
    220      220       Marshall Islands            7           NaN   
    221      221                  Samoa            3           NaN   
    222      222           Saint Helena            2           NaN   
    223      223             Micronesia            1           NaN   
    224      224                  Tonga            1           NaN   

         Total_Recovered  Active_Cases  Tot Cases_per_1M pop  Deaths_per_1M pop  \
    208            699.0           0.0                   NaN                NaN   
    209            438.0           9.0               41514.0              640.0   
    210            217.0         198.0               72174.0                NaN   
    211             61.0          67.0               25815.0              200.0   
    212              NaN           NaN               23377.0                NaN   
    213             77.0           2.0                 119.0                NaN   
    214             14.0          50.0                3511.0                NaN   
    215             27.0           0.0               33582.0                NaN   
    216             20.0           5.0                  35.0                NaN   
    217              8.0           1.0                  16.0                2.0   
    218              7.0           0.0                   NaN                NaN   
    219              6.0           0.0                  22.0                3.0   
    220              4.0           3.0                 117.0                NaN   
    221              3.0           0.0                  15.0                NaN   
    222              2.0           0.0                 328.0                NaN   
    223              1.0           0.0                   9.0                NaN   
    224              1.0           0.0                   9.0                NaN   

         Total_Tests  Tests_per_1M pop  Population  
    208          NaN               NaN         NaN  
    209      20508.0         1875274.0     10936.0  
    210      15956.0         2774957.0      5750.0  
    211       7277.0         1456274.0      4997.0  
    212       8528.0         2345435.0      3636.0  
    213       5075.0            7655.0    662941.0  
    214      19159.0         1051133.0     18227.0  
    215          NaN               NaN       804.0  
    216       4500.0            6314.0    712751.0  
    217          NaN               NaN    619892.0  
    218          NaN               NaN         NaN  
    219      23000.0           72289.0    318168.0  
    220          NaN               NaN     59804.0  
    221          NaN               NaN    200442.0  
    222          NaN               NaN      6105.0  
    223          NaN               NaN    116877.0  
    224          NaN               NaN    107537.0  

</div>

</div>

<div class="cell code" execution_count="74"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="-k2lEojTT4fC" outputId="30fbf0d5-6b19-4906-a0ee-6170bc1cb101">

``` python
len(df_covid.loc[df_covid['Total_Cases']<1000])
```

<div class="output execute_result" execution_count="74">

    17

</div>

</div>

<div class="cell code" execution_count="75"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:521}"
id="0QL_QCVAT4aS" outputId="01846b81-466f-462f-a997-9f3eeb1c59f4">

``` python
df_covid.corr()
```

<div class="output stream stderr">

    <ipython-input-75-0cef49a8a48f>:1: FutureWarning: The default value of numeric_only in DataFrame.corr is deprecated. In a future version, it will default to False. Select only valid columns or specify the value of numeric_only to silence this warning.
      df_covid.corr()

</div>

<div class="output execute_result" execution_count="75">

                           Sr. No.  Total_Cases  Total_Deaths  Total_Recovered  \
    Sr. No.               1.000000    -0.207751     -0.212229        -0.210033   
    Total_Cases          -0.207751     1.000000      0.995500         0.998822   
    Total_Deaths         -0.212229     0.995500      1.000000         0.996961   
    Total_Recovered      -0.210033     0.998822      0.996961         1.000000   
    Active_Cases         -0.200434     0.973870      0.958855         0.961711   
    Tot Cases_per_1M pop -0.189565     0.002248     -0.017414        -0.003425   
    Deaths_per_1M pop    -0.386589     0.031219      0.048106         0.030109   
    Total_Tests          -0.363319     0.917590      0.786937         0.907856   
    Tests_per_1M pop     -0.012995     0.029477     -0.021140         0.019397   
    Population           -0.223055     0.458154      0.433351         0.526329   

                          Active_Cases  Tot Cases_per_1M pop  Deaths_per_1M pop  \
    Sr. No.                  -0.200434             -0.189565          -0.386589   
    Total_Cases               0.973870              0.002248           0.031219   
    Total_Deaths              0.958855             -0.017414           0.048106   
    Total_Recovered           0.961711             -0.003425           0.030109   
    Active_Cases              1.000000              0.035189           0.049085   
    Tot Cases_per_1M pop      0.035189              1.000000           0.605399   
    Deaths_per_1M pop         0.049085              0.605399           1.000000   
    Total_Tests               0.779986              0.120034           0.121517   
    Tests_per_1M pop          0.062791              0.520018           0.143323   
    Population                0.191062             -0.125015          -0.075910   

                          Total_Tests  Tests_per_1M pop  Population  
    Sr. No.                 -0.363319         -0.012995   -0.223055  
    Total_Cases              0.917590          0.029477    0.458154  
    Total_Deaths             0.786937         -0.021140    0.433351  
    Total_Recovered          0.907856          0.019397    0.526329  
    Active_Cases             0.779986          0.062791    0.191062  
    Tot Cases_per_1M pop     0.120034          0.520018   -0.125015  
    Deaths_per_1M pop        0.121517          0.143323   -0.075910  
    Total_Tests              1.000000          0.157303    0.581538  
    Tests_per_1M pop         0.157303          1.000000   -0.088075  
    Population               0.581538         -0.088075    1.000000  

</div>

</div>

<div class="cell code" execution_count="75" id="Tkf9Tfa1hJZe">

``` python
```

</div>

<div class="cell markdown" id="4QpzJINEfsP7">

#13.Random Number Operations

</div>

<div class="cell code" execution_count="76" id="-EKzy78pixq_">

``` python
import random
```

</div>

<div class="cell markdown" id="zo-I4JvIfzia">

## Random Items from list, tuple & string

</div>

<div class="cell code" execution_count="77" id="Rt3S5doxjQCX">

``` python
list=[0,2,4,6,8]
string="cosmology"
tuple=('Astronomy', 'Astrophysics', 'Cosmology', 'Dark Energy', 'Dark Matter')
```

</div>

<div class="cell code" execution_count="78"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="WJ9AD15ZgCbv" outputId="bffa63cc-4ca5-4a4b-b635-49f1b9fded38">

``` python
print(random.choice(list))
```

<div class="output stream stdout">

    8

</div>

</div>

<div class="cell code" execution_count="79"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="AWGM8PBOgCY2" outputId="86cf622b-3d7f-4eba-9450-319d1a69f3a6">

``` python
print(random.choice(string))
```

<div class="output stream stdout">

    g

</div>

</div>

<div class="cell code" execution_count="80"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="YNgq2bwngCVI" outputId="4c18d642-2da0-48aa-c9db-b0676c6d88da">

``` python
print(random.choice(tuple))
```

<div class="output stream stdout">

    Dark Matter

</div>

</div>

<div class="cell code" execution_count="81"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="GuJNXHu9e-56" outputId="0d91d5db-7cc6-4bf8-e3fa-cbdb919b38b7">

``` python
random.random()
```

<div class="output execute_result" execution_count="81">

    0.5757975274900848

</div>

</div>

<div class="cell markdown" id="JoX5hDsKjCe4">

## Random Shuffle

</div>

<div class="cell code" execution_count="82"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="dZ5GNKCRiXlS" outputId="eb000aa7-2b13-4bc5-85c2-0bd784018b9b">

``` python
random.shuffle(list)  #shuffle will only work in list-->It changes the original list
print(list)
```

<div class="output stream stdout">

    [4, 6, 2, 8, 0]

</div>

</div>

<div class="cell markdown" id="rBo4nkqB-x6P">

##Random Sampling

</div>

<div class="cell code" execution_count="83"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Qx0hicv3-vtW" outputId="973f8eaf-f8c7-4e0c-d219-5cfccecb4726">

``` python
list=[0,2,4,6,8]
random.sample(list,3) #return a particluar list of items without any chnage in origi list
```

<div class="output execute_result" execution_count="83">

    [4, 6, 2]

</div>

</div>

<div class="cell markdown" id="nMwo06xIwyQ3">

## Generate Random Numbers

</div>

<div class="cell code" execution_count="84"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="xBu0GoHpuYOG" outputId="20c4a712-3c01-41df-8fdb-7f473793b0ff">

``` python
print(random.randint(0,5))  #Generate a Random Number
```

<div class="output stream stdout">

    2

</div>

</div>

<div class="cell code" execution_count="85"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="PYs7Wd-fwtdJ" outputId="57144835-4aa1-4b9d-d99a-b93ecf1fb3e8">

``` python
print([random.randint(0,10) for i in range(5)]) #Generate a list of Random Number List
```

<div class="output stream stdout">

    [0, 5, 8, 1, 8]

</div>

</div>

<div class="cell code" execution_count="86"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="PyZ2pKvxxVHR" outputId="d51b6c2b-cf55-4338-af69-732bc5c76e92">

``` python
#Alternatively, for Random number list, you can use numpy as
np.random.randint(0,10,5)
```

<div class="output execute_result" execution_count="86">

    array([0, 3, 9, 9, 9])

</div>

</div>

<div class="cell code" execution_count="87"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="lKOw4TsDzz6i" outputId="b205acb8-df46-437c-f80c-dd3700c85cd5">

``` python
np.random.randint(0,10,size=5) #Basically the last arguments denotes the size of list
```

<div class="output execute_result" execution_count="87">

    array([5, 4, 7, 9, 0])

</div>

</div>

<div class="cell code" execution_count="88"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="eNMKtneY4Tnr" outputId="fafe4e42-3ce2-44e7-e91a-b033838c6dd6">

``` python
np.random.randint(0,10,size=(2,5))
```

<div class="output execute_result" execution_count="88">

    array([[5, 3, 1, 0, 3],
           [6, 2, 5, 5, 6]])

</div>

</div>

<div class="cell code" execution_count="89"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="nRFje-EE-QLO" outputId="14a0528e-2a9f-4988-dfd0-b64b5ad08624">

``` python
#Suppose you want to generate random floating values using randint
np.random.randint(0,10,size=(2,5)).astype("float")/10
```

<div class="output execute_result" execution_count="89">

    array([[0.5, 0.6, 0.8, 0.9, 0.4],
           [0.9, 0.9, 0.6, 0.5, 0.2]])

</div>

</div>

<div class="cell code" execution_count="90"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="y8SMKj3O4smL" outputId="7c08f894-80de-4ca7-ef30-8fd58466d17a">

``` python
#Alternatively, one can use random_sample
np.random.random_sample(size=(2,5))
```

<div class="output execute_result" execution_count="90">

    array([[0.23313149, 0.50765889, 0.20986721, 0.34910242, 0.00545842],
           [0.2904978 , 0.56475768, 0.67072328, 0.28949258, 0.70499719]])

</div>

</div>

<div class="cell code" execution_count="91" id="Fmj3yyKVi1FD">

``` python
from IPython.display import clear_output
clear_output(wait=True)
```

</div>

<div class="cell code" execution_count="91" id="HoKxdn8yAxwa">

``` python
```

</div>
