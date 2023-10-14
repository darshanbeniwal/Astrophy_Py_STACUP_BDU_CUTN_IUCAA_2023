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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="bC_BoLoUHS6z" outputId="a92d5292-4986-4633-f5bb-d62d37d67c4f">

``` python
!python --version
```

<div class="output stream stdout">

    Python 3.10.12

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="ogQc6xGf9yaZ" outputId="ab3fa230-5095-4bd9-9151-4aaf53c75d12">

``` python
print(f'Hey there!')
```

<div class="output stream stdout">

    Hey there!

</div>

</div>

<div class="cell markdown" id="t7FEnMVn__al">

## 3.3 Strings can be joined together

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="MhyZfuEo-mNj" outputId="c8f06a90-3806-4683-8a2b-647e09467374">

``` python
print("Hey there!"*3)
```

<div class="output stream stdout">

    Hey there!Hey there!Hey there!

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="ba3b6QZD-6iB" outputId="a98e6403-3722-4313-bd26-4df2867af27b">

``` python
print("print there!" + " How are you?")
```

<div class="output stream stdout">

    print there! How are you?

</div>

</div>

<div class="cell markdown" id="gA7-GcNHWRoF">

# 4.Comments

</div>

<div class="cell code" id="xJoKKPq9aYaH">

``` python
#this is comment line
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="hh2-yT7LH1Ft" outputId="558ed17b-91b4-4132-b07e-4db94d157379">

``` python
print(f'Hey there!') # this is print command
```

<div class="output stream stdout">

    Hey there!

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Jqq3rQH4zf8U" outputId="d160299a-678f-4ff9-d3f3-82ad143dc484">

``` python
x=[] # Define an empty list
x
```

<div class="output execute_result" execution_count="7">

    []

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="n5bjo3Kc4aM9" outputId="e5593839-3091-4cd3-baca-07b75e9cd35a">

``` python
y=[1,2,3,5,4,5,6,9] #Define a list of numbers
y
```

<div class="output execute_result" execution_count="8">

    [1, 2, 3, 5, 4, 5, 6, 9]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="OoOxEQsBfmG3" outputId="8473b6ad-6ec8-447a-d10c-55bbcec91f9e">

``` python
y[::-1] # Reverse the list
```

<div class="output execute_result" execution_count="9">

    [9, 6, 5, 4, 5, 3, 2, 1]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="GOz4mLV_7G3c" outputId="a62befc0-6078-4857-ff18-dc7372228f06">

``` python
len(y) # Check the length of list
```

<div class="output execute_result" execution_count="10">

    8

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="OigvtQBP5UX1" outputId="2028c903-7d2b-4690-c695-92374b8a2660">

``` python
m=['Apple','Boy','Cat',[1,2]] # Define a list of objects with different data types
m[0][1], m[2][2], m[3][0] #Output: 'p','t',1
```

<div class="output execute_result" execution_count="11">

    ('p', 't', 1)

</div>

</div>

<div class="cell code" id="KZEp6qMV7Y-q">

``` python
y=[1,2,3,4,5,6,7] #Define a list of numbers
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="85z3WqqV7bhE" outputId="2909c646-ecdf-439c-f236-9bf221e313a5">

``` python
y[2]  #Print an element or number of specific position
```

<div class="output execute_result" execution_count="13">

    3

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="_8Z9rBIL8zC2" outputId="63702a34-764c-4c45-a83a-d4aac8828a1d">

``` python
y[-1]
```

<div class="output execute_result" execution_count="14">

    7

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="TwO6Js6R9Kqo" outputId="f5d66622-5c36-41cf-88ee-51c73606b699">

``` python
y[0:2]    #Print first two elements
```

<div class="output execute_result" execution_count="15">

    [1, 2]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="wDkug5UH9-MF" outputId="3b2463ec-ed25-4a8f-a27b-5170d9bc42d9">

``` python
y[2:4]    #Print elements from 2nd position to 4th position
```

<div class="output execute_result" execution_count="16">

    [3, 4]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="2luS3fjP5xzv" outputId="7cd4e6f6-a3f8-4034-84ba-6adad63ded5b">

``` python
y=[1,2,3] #Define a list of numbers
y[2]=4
y
```

<div class="output execute_result" execution_count="17">

    [1, 2, 4]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="mpQd3V9y6-dL" outputId="4e34f950-29e7-4e7c-b66a-c41b6a2ecc9a">

``` python
'''
Add List Items
'''
y=[1,2,3,4,5]
y.append(8)
print(y)
```

<div class="output stream stdout">

    [1, 2, 3, 4, 5, 8]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="1RJwpw05_yPX" outputId="b0728e3e-95fb-4304-a8bd-384bb2d9916c">

``` python
'''
insert item at a particular position
'''
y=[1,2,3,4,5]
y.insert(1,8)
print(y)
```

<div class="output stream stdout">

    [1, 8, 2, 3, 4, 5]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="WaiGAt63__3I" outputId="2dd6d4f4-897a-440c-fcb8-b36015ef1a50">

``` python
'''
Extend List
'''
x=[1,2,3,4]
y=[5,6,7,8]
x.extend(y)
print(x)
```

<div class="output stream stdout">

    [1, 2, 3, 4, 5, 6, 7, 8]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="iwBEihbIAdiy" outputId="57e07d9a-5055-41f3-d4c6-ea0ac220059c">

``` python
'''
Remove Items from a list
'''
y=[1,3,4,7,8]
y.remove(3)       #Try to remove an unlisted item--Error? Its okay!
print(y)
```

<div class="output stream stdout">

    [1, 4, 7, 8]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="uFn_7CGZAzWH" outputId="832f9290-93f7-47b2-aeb0-7f5636d13244">

``` python
'''
Remove Specified Index use: pop
'''
y=[1,3,4,7,8]
y.pop(2)    #y.del(2)
print(y)
```

<div class="output stream stdout">

    [1, 3, 7, 8]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="vymb0Rz1CCeS" outputId="9aa16df2-dcc7-4112-e84b-e9ea0526cf9f">

``` python
'''
Remove Specified Index use: del
'''
y=[1,3,4,7,8]
del y[2]
print(y)
```

<div class="output stream stdout">

    [1, 3, 7, 8]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:211}"
id="xzew2IhvCcXS" outputId="c84ada68-d6cc-4b41-b908-d990516903a7">

``` python
'''
Remove a list completely
'''
y=[1,3,4,7,8]
del y        # expected output []
print(y)     #this will cause an error because you have succsesfully deleted "y".
```

<div class="output error" ename="NameError" evalue="ignored">

    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    <ipython-input-24-9d918515cb4a> in <cell line: 6>()
          4 y=[1,3,4,7,8]
          5 del y        # expected output []
    ----> 6 print(y)     #this will cause an error because you have succsesfully deleted "y".

    NameError: name 'y' is not defined

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="F-n7PW4JDKHC" outputId="36316d9f-0fe7-40b8-e264-ec4f64f3fe07">

``` python
'''
Clear a list
'''
y=[1,3,4,7,8]
y.clear()
print(y)
```

<div class="output stream stdout">

    []

</div>

</div>

<div class="cell markdown" id="wRvT8U3mD0AC">

## 5.2 Tuples

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:70}"
id="RdGpYzhSDi_9" outputId="b4c7c72d-f06b-448b-e237-bdd9bc877098">

``` python
'''
they’re immutable sequences. This means that you can’t change them after creation.
Tuple items are ordered, unchangeable, and allow duplicate values.
To create a tuple object, can use an assignment operation with a sequence of a
comma-separated items on its right side.
'''
```

<div class="output execute_result" execution_count="26">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" id="ObJagnG5EEWv">

``` python
x=('Apple','Boy','Cat','Dog')
```

</div>

<div class="cell markdown" id="_H_1sduxHI4J">

## 5.3 Sets

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="QmV3ULynHTXs" outputId="b110d8ba-df34-4dae-e131-a6ecdf17a4dd">

``` python
x={'Apple','Boy','Cat','Dog','Boy'}
print(x)
```

<div class="output stream stdout">

    {'Boy', 'Dog', 'Apple', 'Cat'}

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="aX7NKTEbHehp" outputId="cb53bc52-1c9a-4999-c0bd-3a32965e8e3d">

``` python
type(x)
```

<div class="output execute_result" execution_count="31">

    set

</div>

</div>

<div class="cell markdown" id="ely9thUQIYgY">

## 5.4 Dictionaries

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="aAN-EGqrHwF2" outputId="033bb9c8-5a78-4c5b-fea0-ae190c2912f0">

``` python
'''
Dictionary items are ordered, changeable, and does not allow duplicates.
Dictionary items are presented in key:value pairs, and can be referred to by using the key name.
'''
India={"Name":"India","Continents":"Asia","Capital":"New Delhi"}
prsn=dict(Name="XYZ",Age="20",Height="170cm",Weight="70kg")
India, prsn
```

<div class="output execute_result" execution_count="32">

    ({'Name': 'India', 'Continents': 'Asia', 'Capital': 'New Delhi'},
     {'Name': 'XYZ', 'Age': '20', 'Height': '170cm', 'Weight': '70kg'})

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="igALKvjMJYYP" outputId="1ac10995-bb21-4df1-ada0-b9eb1f1090dc">

``` python
India["Name"], India["Capital"], prsn["Name"], prsn["Weight"]
```

<div class="output execute_result" execution_count="33">

    ('India', 'New Delhi', 'XYZ', '70kg')

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="hEXDhWg1KvAw" outputId="6c5bd2f7-1ebc-4f6a-c243-74bee1bbff72">

``` python
import numpy
x=numpy.array([1,2,3])   #a vector as a row
x
```

<div class="output execute_result" execution_count="35">

    array([1, 2, 3])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="uRGxZ-6-M4wk" outputId="46b85745-54c0-4ea4-b86a-e6725a19a168">

``` python
y=numpy.array([[1],
              [2],
              [3]])   #a vector as a column
y
```

<div class="output execute_result" execution_count="36">

    array([[1],
           [2],
           [3]])

</div>

</div>

<div class="cell code" id="I-V_boN0ht5z">

``` python
import numpy as np
```

</div>

<div class="cell markdown" id="Cwf9oeerOaXL">

## 6.2 Matrix

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="JZzcYJ5KOBS4" outputId="0a71538a-b526-47ed-afbe-5a643ded175a">

``` python
m=np.array([[1,2,3],
            [4,5,6]])
m
```

<div class="output execute_result" execution_count="40">

    array([[1, 2, 3],
           [4, 5, 6]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="UJByfVAWNvbN" outputId="6c4e79c0-8324-4e90-bfb3-17c02036340d">

``` python
m.shape
```

<div class="output execute_result" execution_count="41">

    (2, 3)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="PbteY-YjOKRO" outputId="c8976e15-316b-4b2c-f18c-ae44ed296209">

``` python
'''
NumPy actually has a dedicated matrix data structure:
'''
mat=np.mat([[1,2,3],
            [4,5,6]])
mat
```

<div class="output execute_result" execution_count="42">

    matrix([[1, 2, 3],
            [4, 5, 6]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Y4yTDS5FO4dG" outputId="51f94e94-87e3-4406-ec34-4008e6c37a5d">

``` python
mat.shape
```

<div class="output execute_result" execution_count="43">

    (2, 3)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="sOxVhkXpQdvc" outputId="f74d73c2-c42f-4929-f126-63089ff68c85">

``` python
m.size
```

<div class="output execute_result" execution_count="44">

    6

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="NzjjcvTpQgh1" outputId="b1de0965-b27a-4a7c-bb75-33695a9bf52a">

``` python
m.ndim
```

<div class="output execute_result" execution_count="45">

    2

</div>

</div>

<div class="cell code" id="ckkBQJZG5nx3">

``` python
vec=np.array((1,2,3,4,5))
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="NLb2skB8Port" outputId="91178ab7-56dc-4447-ef8c-a0a6d3dd632e">

``` python
# Select all elements of a vector
vec[:]
```

<div class="output execute_result" execution_count="47">

    array([1, 2, 3, 4, 5])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="VH5YHsofPzzF" outputId="48662c16-e91c-4054-c714-cd0a91a5cb4e">

``` python
# Select everything up to and including the fourth element
vec[:4]
```

<div class="output execute_result" execution_count="48">

    array([1, 2, 3, 4])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="e5g8a-mDP02k" outputId="226ffdcc-4e44-4724-dbfd-626055d115ca">

``` python
# Select everything after the fourth element
vec[4:]
```

<div class="output execute_result" execution_count="49">

    array([5])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="n4paDw2PQDL3" outputId="35dfd1a7-c942-4226-ad3a-b1a194ee28f2">

``` python
# Select the last element
vec[-1]
```

<div class="output execute_result" execution_count="50">

    5

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="3RbNfKmiQLhh" outputId="4ba90275-f3b2-4e91-c403-f8ce16aa9ff8">

``` python
# Select the first two rows and all columns of a matrix
m[:2,:]
```

<div class="output execute_result" execution_count="51">

    array([[1, 2, 3],
           [4, 5, 6]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Q4Z3uZb5QWWn" outputId="88317810-af10-44a1-a6de-3c22c2b1e7da">

``` python
# Select all rows and the second column
m[:,1:2]
```

<div class="output execute_result" execution_count="52">

    array([[2],
           [5]])

</div>

</div>

<div class="cell markdown" id="XY6QgUcJ9WwH">

## 6.3 Maximum & Minimum values

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="FZSS5NTuQZ7s" outputId="0c2eea25-f8c6-4077-a8e4-5e5ab6561421">

``` python
'''
Finding the Maximum and Minimum Values
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m), np.min(m)
```

<div class="output execute_result" execution_count="53">

    (9, 1)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="xECK2JWjQ1ie" outputId="b1783566-8bb9-4d4c-d95e-26896c7a624e">

``` python
'''
Finding the Maximum and Minimum Values from the each axis
'''
m=np.array([[1,2,3],
            [4,5,6],
            [7,8,9]])
np.max(m,axis=1)    #axis=0 max in each column & axis=1 max in each row
```

<div class="output execute_result" execution_count="54">

    array([3, 6, 9])

</div>

</div>

<div class="cell markdown" id="B7Muc7yU_Bwj">

## 6.4 Reshaping the array

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="eZ0CpNGBRD52" outputId="c3859f8b-f124-4019-d88f-73af25d7f5db">

``` python
import numpy as np
m=np.array([[1,2,3],
             [4,5,6],
             [7,8,9],
             [10,11,12]
             ])
m.shape
```

<div class="output execute_result" execution_count="55">

    (4, 3)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="_AC4aksc_1CM" outputId="07c602b2-5105-40e6-d137-d947c915aad7">

``` python
m_=m.reshape(2,6)
m_
```

<div class="output execute_result" execution_count="56">

    array([[ 1,  2,  3,  4,  5,  6],
           [ 7,  8,  9, 10, 11, 12]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="RBMvxLTwAIKG" outputId="9fad333e-54ae-4dd2-fccc-37d5dc6ba200">

``` python
m_.shape
```

<div class="output execute_result" execution_count="57">

    (2, 6)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Eq7xKRMKBUXc" outputId="5fa7f57a-8bb1-4851-be87-01bcd8cbcf93">

``` python
# Reshape it as a 1-D array
m__=m_.reshape(12)
m__
```

<div class="output execute_result" execution_count="58">

    array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="_euhGxjDCUrM" outputId="1023d504-6ce5-40e6-c720-a679f3f9490f">

``` python
m__.shape
```

<div class="output execute_result" execution_count="59">

    (12,)

</div>

</div>

<div class="cell code" id="wlkFqb-hCWyx">

``` python
m.resize(2,6)
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="imyrh_Z9CbLG" outputId="63da10f3-5fd7-4c94-8534-360a79887967">

``` python
m
```

<div class="output execute_result" execution_count="61">

    array([[ 1,  2,  3,  4,  5,  6],
           [ 7,  8,  9, 10, 11, 12]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="yytgIDztCdD-" outputId="20a8b185-317b-4f43-9a02-8598caba23c7">

``` python
'''
reshape() does not changes the original array but only returns the changed array,
whereas the resize() method returns nothing and directly changes the original array.
'''
```

<div class="output execute_result" execution_count="62">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell markdown" id="frAIekrneEJL">

## 6.5 Transpose, Rank, Determinant, Diagonal,trace and inverse of a matrix

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="xfVtDWvgdx0p" outputId="434d3a9c-6134-4886-8639-10a36eb25fc2">

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

<div class="output execute_result" execution_count="63">

    array([[1, 4, 7],
           [2, 5, 8],
           [3, 6, 9]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="fLWc0DkwezfZ" outputId="e6a20faa-3d78-431a-b380-16294a321d2f">

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

<div class="output execute_result" execution_count="64">

    2

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="_tS-C2_hfwVg" outputId="1dc5e4b8-0972-412b-d9ff-320f84eba90b">

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

<div class="output execute_result" execution_count="65">

    -42.00000000000001

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="qgSPvyEOiKsk" outputId="c7463113-1f0f-48df-ef8f-aabf0d796c12">

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

<div class="output execute_result" execution_count="66">

    array([1, 5, 9])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="mjCYbG8Ric5h" outputId="a3c235ab-4e21-4bbd-e985-ca0aec1dca46">

``` python
# Return diagonal one above the main diagonal
m.diagonal(offset=1)
```

<div class="output execute_result" execution_count="67">

    array([2, 6])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="aPILSftoixJn" outputId="7bc9935b-8a08-4b7a-8923-ef95340ae836">

``` python
# Return diagonal one below the main diagonal
m.diagonal(offset=-1)
```

<div class="output execute_result" execution_count="68">

    array([4, 1])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="g1hn-jUri17A" outputId="6f1f8a58-63fa-480b-c6fe-7be52f374fcf">

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

<div class="output execute_result" execution_count="69">

    15

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="pFpjLHVNjTqn" outputId="b6785440-59cb-4bab-b717-dcd5eb22db60">

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

<div class="output execute_result" execution_count="70">

    array([[-0.92857143,  0.35714286,  0.07142857],
           [-0.14285714,  0.28571429, -0.14285714],
           [ 0.73809524, -0.30952381,  0.07142857]])

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="4XT8c6oWmN4P" outputId="df933e99-f89a-4a60-b77d-e2d115ff029e">

``` python
e_values,e_vectors
```

<div class="output execute_result" execution_count="72">

    (array([ 1.61168440e+01, -1.11684397e+00, -1.30367773e-15]),
     array([[-0.23197069, -0.78583024,  0.40824829],
            [-0.52532209, -0.08675134, -0.81649658],
            [-0.8186735 ,  0.61232756,  0.40824829]]))

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="IkhHwdDYmSP9" outputId="d8a629fc-0186-4481-fef1-68be80d32100">

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

<div class="output execute_result" execution_count="73">

    array([[ 1,  4,  4],
           [ 8,  6,  9],
           [14, 10, 15]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="6IowJEHkne45" outputId="51a571a2-4795-4a54-d9d7-75f677a07e98">

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

<div class="output execute_result" execution_count="74">

    array([[1, 0, 2],
           [0, 4, 3],
           [0, 6, 3]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="QmJ9pp11nuZR" outputId="c3629fe2-f661-4c13-a258-842f5594c2ee">

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

<div class="output execute_result" execution_count="75">

    array([[29, 10, 25],
           [62, 25, 55],
           [95, 40, 85]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="7U0ATU2QoGn4" outputId="04e6aa56-b1af-41c1-aac9-98fa673078f1">

``` python
'''
Alternatively, in Python 3.5+, operator @ will also work for mulitplication
'''
m_a@m_b
```

<div class="output execute_result" execution_count="76">

    array([[29, 10, 25],
           [62, 25, 55],
           [95, 40, 85]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="t7OJsHPKoZt3" outputId="7f123b2c-2e34-49f7-ca64-71f8b7a8b25b">

``` python
'''
For elementwise multiplications of two matrices
'''
m_a*m_b
```

<div class="output execute_result" execution_count="77">

    array([[ 0,  4,  3],
           [16,  5, 18],
           [49, 16, 54]])

</div>

</div>

<div class="cell code" id="86WZ8xIOcfS2">

``` python
```

</div>

<div class="cell markdown" id="Ojj25A1IsAlJ">

# 7.Python Conditions-Loops

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="8sWLP9bxomK2" outputId="2e987977-a8e8-4df7-ea3b-20f03524a155">

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

<div class="output execute_result" execution_count="78">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell markdown" id="ASHuTB8lsklc">

## 7.1 if.....else

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="VDh56uILsrpU" outputId="42ad2334-08e1-4ded-ead4-10548c912aba">

``` python
a=4
b=6
if a<b:
  print("b is greater than a")
```

<div class="output stream stdout">

    b is greater than a

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:141}"
id="Zz1YPC5Es3Kn" outputId="2458a658-def5-4860-c333-700dad24846f">

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

<div class="output error" ename="IndentationError" evalue="ignored">

      File "<ipython-input-80-10c7333a111a>", line 9
        print("b is greater than a")
        ^
    IndentationError: expected an indented block after 'if' statement on line 8

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="FRaLzq2ztxly" outputId="69442478-adf0-49db-ac27-578f7f38f9f2">

``` python
a=4
b=6
if a>b:
  print("a is greater than b")
else:
  print("a is not greater than b")
```

<div class="output stream stdout">

    a is not greater than b

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="MLc64VW4uM1-" outputId="66831c7b-1bb4-492f-d3b6-94c8e26e82f5">

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

<div class="output stream stdout">

    a is less than b

</div>

<div class="output execute_result" execution_count="82">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="7kX3E8dGvQED" outputId="caffc748-413a-4172-cf6d-70ebf17bb749">

``` python
'''
one line if statement
'''
a=4
b=5
print("A") if a > b else print("=") if a == b else print("B")
```

<div class="output stream stdout">

    B

</div>

</div>

<div class="cell markdown" id="Tonh1YnqwXWU">

## 7.2 while loop

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="13n_FMKrwBND" outputId="575d87c1-8b33-4039-8f4d-15132540db53">

``` python
i=1
while i<5:
  print (i)
  i=i+1 #i+=1
```

<div class="output stream stdout">

    1
    2
    3
    4

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="-qnos4OXwmFb" outputId="c6dc28ad-a059-4ddf-c14e-b8a0aa06e90b">

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

<div class="output stream stdout">

    1
    2
    3

</div>

</div>

<div class="cell markdown" id="fEM5XStTxncL">

## 7.3 for loop

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="6ToHUOORxkie" outputId="f915b2d7-b072-4bf9-d223-211bc8fd93f1">

``` python
alpha_b=['Apple','Boy','Cat']
for x in alpha_b: #x is a variable --->For loops iterate over a given sequence
  print(x)
```

<div class="output stream stdout">

    Apple
    Boy
    Cat

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Pl7QKgAmyKlg" outputId="05ac2980-a155-4d7c-cce6-007ba5a7782d">

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

<div class="output stream stdout">

    Apple

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="knH7LwVmzAvp" outputId="c68ce67d-17fa-4cf7-b97e-96993bb88acf">

``` python
'''
the range() Function
'''
for x in range(5):    #which means values from 0 to 4 not 0 to 5
  print(x)
```

<div class="output stream stdout">

    0
    1
    2
    3
    4

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="boL7I2P1zTkw" outputId="f5bf0850-d5ba-4c69-dd51-ef66b17f68c5">

``` python
for x in range(2,5):
  print(x)
```

<div class="output stream stdout">

    2
    3
    4

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="3XDBZAsnzaFs" outputId="5ff46e43-c77a-4fc8-8e00-473fd053158e">

``` python
for x in range(0,40,10):
  print(x)
```

<div class="output stream stdout">

    0
    10
    20
    30

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="xbJI6HdSz1Oy" outputId="9b0e33a4-13f0-4980-9e49-97894f9fe433">

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

<div class="output stream stdout">

    Apple banana
    Apple mango
    Apple cherry
    Boy banana
    Boy mango
    Boy cherry
    Cat banana
    Cat mango
    Cat cherry

</div>

</div>

<div class="cell markdown" id="NlL6jyjh1WVD">

# 8.Functions

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:36}"
id="ux-huCkH0cd9" outputId="85ae29c3-66c8-46c8-c9f9-aed1cfa5f0b2">

``` python
'''
A function is defined using the def keyword in Python
'''
```

<div class="output execute_result" execution_count="92">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" id="JDq-U1zy482U">

``` python
def my_fun():
  print("Hey there!")
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="R3wws0Dzsr7B" outputId="edc50c44-19f6-45a9-e543-beaa345b7f01">

``` python
my_fun()
```

<div class="output stream stdout">

    Hey there!

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="9uHFIrrx63ZG" outputId="8132b859-58e9-43b2-afd8-058b2620a194">

``` python
print(my_fun(1))
print(my_fun(2))
print(my_fun(3))
print(my_fun(4))
print(my_fun(5))
```

<div class="output stream stdout">

    6
    7
    8
    9
    10

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="txCAGD7r6e4Q" outputId="20a3be3a-bab9-46cf-c18f-8a79514500cc">

``` python
i=1
while i<5:
  print(my_fun(i))
  i+=1
```

<div class="output stream stdout">

    6
    7
    8
    9

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="6Owcz5w_DGMq" outputId="4c1340e5-c5fc-4b70-8a76-3fcf6a47ea53">

``` python
'''
Sometimes we have to perform mathematical tasks on numbers i.e. minimum, maximum,
 sqrt, ceil.,floor, pi etc.
'''
```

<div class="output execute_result" execution_count="99">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="MdpI3_MCBLRS" outputId="73f028f5-1f02-41f6-c6d7-a3dd67675233">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="8N6oNN12DEZh" outputId="9a95cea3-8b88-4bb6-d3f1-d8e66fd7da88">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="SQxUI5YAEbIx" outputId="553b14ca-3be8-4cec-d525-f1e68684f0ce">

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

<div class="cell code" id="QknUoMEcEkJ5">

``` python
'''
For some extended mathemaical function, please import math first
'''
import numpy as np
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="MEY5gkEIE2uL" outputId="cb9cb17e-91c9-4beb-b1a5-e78558f77f23">

``` python
x=np.sqrt(64)
x
```

<div class="output execute_result" execution_count="104">

    8.0

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="WhlCoLTvE7EK" outputId="3859c26e-d40e-4d53-a2ed-8fa306ec1023">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="gYDM1i0_E9U9" outputId="8b0bc690-34db-4005-b3b5-23beaf2962ae">

``` python
x=np.pi+6
x
```

<div class="output execute_result" execution_count="106">

    9.141592653589793

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="iCoPPH639Di5" outputId="60be1a1a-1a15-4c12-8edf-1b1736394fbc">

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

<div class="cell code" id="uep8ggcr9J9Z">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt")
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="icEGLrJKqokg" outputId="12846ea2-8022-4901-a0a3-741f7272eff8">

``` python
f
```

<div class="output execute_result" execution_count="120">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="-K9qlqLerNFX" outputId="a90745dc-fe89-496a-b96e-5adb9352ef45">

``` python
f[0]
```

<div class="output execute_result" execution_count="121">

    array([0., 0.])

</div>

</div>

<div class="cell code" id="Q5QXORTyrIA5">

``` python
# read text file using loadtxt
f= np.loadtxt("testt.txt",unpack="True")
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="5PYpY86LrQZQ" outputId="89703b92-54c6-48ec-8978-d011672a7bf1">

``` python
f
```

<div class="output execute_result" execution_count="123">

    array([[0.      , 0.111111, 0.222222, 0.333333, 0.444444, 0.555556,
            0.666667, 0.777778, 0.888889, 1.      ],
           [0.      , 0.110883, 0.220398, 0.327195, 0.429956, 0.527415,
            0.61837 , 0.701698, 0.776372, 0.841471]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="a3g5o-_srSbY" outputId="a60d2045-a756-4232-d49f-688a3467ca81">

``` python
f[0]
```

<div class="output execute_result" execution_count="124">

    array([0.      , 0.111111, 0.222222, 0.333333, 0.444444, 0.555556,
           0.666667, 0.777778, 0.888889, 1.      ])

</div>

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="0JXRjcPpNl_H" outputId="637165da-b042-412f-bb61-80dccaf598bf">

``` python
print(matplotlib.__version__)  ##Check Matplotlib version
```

<div class="output stream stdout">

    3.7.1

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:53}"
id="lIzAELlxNsGm" outputId="241096da-5b58-4375-8b92-bfc57aaef13a">

``` python
'''
Generally we have many submodule of a Python module:
Most of the Matplotlib utilities lies under the pyplot submodule:
and are usually imported under the plt alias:
'''
```

<div class="output execute_result" execution_count="131">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code" id="lrq8JSDwoIfA">

``` python
import matplotlib.pyplot as plt #Now the Pyplot package can be referred to as plt.
import numpy as np
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="KtGZ9Ql5sjV1" outputId="5a78daf7-a1c5-434a-8f03-027fd03ee67b">

``` python
x=np.array([0,10])
y=np.array([0,250])
plt.plot(x,y)
```

<div class="output execute_result" execution_count="133">

    [<matplotlib.lines.Line2D at 0x789f8afb98a0>]

</div>

<div class="output display_data">

![](efdec09461a636380c9bd8d589eac27dc2e05dfb.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="55Zdfyb8uucQ" outputId="5a2add35-fe4a-4772-f05b-42bd42ef47c7">

``` python
'''
Next try to use two submodule of numpy i.e. np.arange and np.linspace along with matplotlib
'''
t=np.arange(-10,10,0.001)
fun=np.sin(t)
plt.plot(t,fun)
```

<div class="output execute_result" execution_count="134">

    [<matplotlib.lines.Line2D at 0x789f898de230>]

</div>

<div class="output display_data">

![](b3fecf4077926b4df8f201e8a635e5835f3800ea.png)

</div>

</div>

<div class="cell markdown" id="sbohRWzx0mJE">

##Set axis Labels

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:466}"
id="0LpwPLhgxmMk" outputId="bdb3c7ba-d630-4d21-87f2-6c770ed7b62b">

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

<div class="output execute_result" execution_count="135">

    [<matplotlib.lines.Line2D at 0x789f8976f1f0>]

</div>

<div class="output display_data">

![](25899ac15dad6f469ff7b87bcdce58a0776cacbb.png)

</div>

</div>

<div class="cell markdown" id="KlL5dkba0rOc">

##Set Title of plot

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="jNIVTgFE3bwR" outputId="b037678d-af47-4633-9130-56add7825571">

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

<div class="output execute_result" execution_count="136">

    [<matplotlib.lines.Line2D at 0x789f8966ecb0>]

</div>

<div class="output display_data">

![](c5feed8cdb7aeb9b6abfbed252d0d9b84d8ee27b.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="qcPSDD6r6nij" outputId="1569fff4-a96b-4445-d44a-7d8f6cf62383">

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

<div class="output execute_result" execution_count="137">

    [<matplotlib.lines.Line2D at 0x789f896e5210>]

</div>

<div class="output display_data">

![](c5feed8cdb7aeb9b6abfbed252d0d9b84d8ee27b.png)

</div>

</div>

<div class="cell markdown" id="x4p9hTHK0y2o">

##Change color of plot curve

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="_Z6sgHnD66Cp" outputId="50af6397-6848-4a3a-e933-fe21962bdc5b">

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

<div class="output execute_result" execution_count="138">

    [<matplotlib.lines.Line2D at 0x789f89633430>]

</div>

<div class="output display_data">

![](69c7a54f6bf455bf88639cd94aa1d59f4fae6a08.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="rsVxmp8U7QCR" outputId="81b2d9ac-5d0c-48a9-8ae1-aaf1f8a06980">

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

<div class="output execute_result" execution_count="139">

    [<matplotlib.lines.Line2D at 0x789f8942b190>]

</div>

<div class="output display_data">

![](ebc96a109c3d62a36c9816b02a6474ac03f0bbd9.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:88}"
id="Pk3VEVdG9440" outputId="7dca46aa-4f07-4e43-d02c-bed0e57d0f82">

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

<div class="output execute_result" execution_count="140">

``` json
{"type":"string"}
```

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="h5v3ACb_AjWH" outputId="284328d3-2a79-43f6-b173-76815de63e42">

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

<div class="output execute_result" execution_count="141">

    [<matplotlib.lines.Line2D at 0x789f894e1bd0>]

</div>

<div class="output display_data">

![](7cb03316adea4318df0f94cc93ce1625281c0f37.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="IVF0-i3UKD0P" outputId="5df44ea3-12e7-47a0-f373-0be747777db8">

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

<div class="output execute_result" execution_count="142">

    [<matplotlib.lines.Line2D at 0x789f893a00d0>]

</div>

<div class="output display_data">

![](611caee9f5d67d03c372cf627eb6de40e9669147.png)

</div>

</div>

<div class="cell markdown" id="TJ9lv75ahdM6">

##MultiPlot in a single plot

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="5vsCTtxpNlv4" outputId="d05b13d1-069f-4cf8-b787-111731e0c926">

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

<div class="output execute_result" execution_count="143">

    [<matplotlib.lines.Line2D at 0x789f892320e0>]

</div>

<div class="output display_data">

![](9e4bce0aa666b983d6ffb428c15ecf7768c5d71a.png)

</div>

</div>

<div class="cell markdown" id="rzzXp1r0kJW4">

## Add Legands

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="q2dZ0erDh1-e" outputId="c7a6e527-b7af-4850-9790-c38b4e68e933">

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

<div class="output execute_result" execution_count="144">

    <matplotlib.legend.Legend at 0x789f892d1480>

</div>

<div class="output display_data">

![](52ebdaf45c4a9cb0e53903d2c2d3fde9c320a1c3.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="CI_SlwjjkX6e" outputId="5f1e53c6-0197-4213-f7d6-1a220743c00e">

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

<div class="output execute_result" execution_count="145">

    <matplotlib.legend.Legend at 0x789f892d2b30>

</div>

<div class="output display_data">

![](37efd18e6422db69fa705a3e1df6a515a93d4204.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:491}"
id="xAAPPrXQm_47" outputId="4b587c24-420f-4307-e823-7e814216cd83">

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

<div class="output execute_result" execution_count="146">

    <matplotlib.legend.Legend at 0x789f8894c850>

</div>

<div class="output display_data">

![](109a24a58add344e21b7cfc58b1d475051454feb.png)

</div>

</div>

<div class="cell markdown" id="IbWFnmIbtMhI">

## Add Grid

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:474}"
id="IYERRUFJn2hT" outputId="30ec4be8-e234-41ce-a8eb-37bf83fc7aaa">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:622}"
id="5cHDdWu9uZ7y" outputId="e8337d97-1fef-4e87-c491-6f6601941ebd">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:622}"
id="XPpZbA-8voWy" outputId="acf3557e-5b73-41cb-d334-90a887ff8c75">

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

<div class="cell code" id="bS31gmnOd4q8">

``` python
```

</div>

<div class="cell markdown" id="9zQJ4R510WXR">

##Errorbar Plots

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:466}"
id="F0lG-aGzzP_Z" outputId="0baa6cc5-7dab-4a90-c148-345a80f4b219">

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

<div class="output execute_result" execution_count="150">

    Text(0, 0.5, 'y')

</div>

<div class="output display_data">

![](c4051b3dfc9b6105f48e90ca93ca890e46a6ab01.png)

</div>

</div>

<div class="cell markdown" id="vTzJBq0L0gou">

##Confidence levels regions

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="MP2JfL8D0jlm" outputId="c472ff66-8c3a-4ec8-e7ae-c7e0ada40892">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
y_err=y*0.1
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.fill_between(x, y+1.*y_err, y-1.*y_err, facecolor='#F08080', alpha=0.99)
plt.fill_between(x, y+2.*y_err, y-2.*y_err, facecolor='#F08080', alpha=0.59)
plt.fill_between(x, y+3.*y_err, y-3.*y_err, facecolor='#F08080', alpha=0.39)
```

<div class="output execute_result" execution_count="151">

    <matplotlib.collections.PolyCollection at 0x789f881b51b0>

</div>

<div class="output display_data">

![](abbcfc82307ac0ca2ea18ff7dbccd9a0ba4dc6ec.png)

</div>

</div>

<div class="cell code" id="iz5063RLemgm">

``` python
```

</div>

<div class="cell markdown" id="KMcpsJvQ0qGN">

##Scatter Plot

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:447}"
id="I3fRMxkR0qf1" outputId="b609cac4-853c-4669-d31a-3866cecd1ee0">

``` python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
plt.scatter(x,y)
```

<div class="output execute_result" execution_count="152">

    <matplotlib.collections.PathCollection at 0x789f880ef670>

</div>

<div class="output display_data">

![](b084fb6ac9ccd77797e2f0e4f3642c03c6c96cc0.png)

</div>

</div>

<div class="cell markdown" id="_dvN4iwh0rQF">

##Histogram Plot

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:482}"
id="bltHawb10tF1" outputId="46fbbae1-2da9-4a73-970b-f3d0febd01c5">

``` python
x=np.array((1,2,1,2,5,3,4,5,7,8,6,7,8,3,2,1))
plt.hist(x)
```

<div class="output execute_result" execution_count="153">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:545}"
id="Gs5HtfKC0wAW" outputId="5e36bf24-3145-4b8a-f00e-3f48992e852a">

``` python
x=(45,23,37,5)
plt.pie(x)
```

<div class="output execute_result" execution_count="154">

    ([<matplotlib.patches.Wedge at 0x789f79cb4e50>,
      <matplotlib.patches.Wedge at 0x789f79cb4d60>,
      <matplotlib.patches.Wedge at 0x789f79cb5720>,
      <matplotlib.patches.Wedge at 0x789f79cb5ba0>],
     [Text(0.30990582150899426, 1.0554422683381766, ''),
      Text(-1.0959649072339253, -0.09413247108056673, ''),
      Text(0.24914641133865234, -1.0714131162707834, ''),
      Text(1.0888035854028022, -0.15654632673430272, '')])

</div>

<div class="output display_data">

![](166917faf2f3d09385975c218609869246fa8360.png)

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:545}"
id="E_NKbh8lV-uW" outputId="6815d67e-5b4a-4874-ab29-12d2ef079cf1">

``` python
#Add Label
x=(45,23,37,5)
plt.pie(x,labels=["Sample(x1)", "Sample(x2)", "Sample(x3)", "Sample(x4)"])
```

<div class="output execute_result" execution_count="155">

    ([<matplotlib.patches.Wedge at 0x789f79cef520>,
      <matplotlib.patches.Wedge at 0x789f79cb6b00>,
      <matplotlib.patches.Wedge at 0x789f79cefe20>,
      <matplotlib.patches.Wedge at 0x789f79d282e0>],
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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:415}"
id="Dlj2mC8TkKOe" outputId="960df702-3691-46d4-ad95-ee33769f6a59">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:143}"
id="LPlk8AkmCJ8l" outputId="4b2265ee-7fe0-4734-ab47-ea503b79647d">

``` python
df
```

<div class="output execute_result" execution_count="159">

        Name  Age  Color
    0    Tom    2  Black
    1  Jerry    5  White
    2    Sam    8  Brown

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="lulcy-dJCT6S" outputId="6eb41fdb-d035-4809-ca27-50622a215eb0">

``` python
df['Age']
```

<div class="output execute_result" execution_count="160">

    0    2
    1    5
    2    8
    Name: Age, dtype: int64

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="8YiBCCB0R6IS" outputId="7211980e-ecb1-46a9-89bd-473b03ee736c">

``` python
df['Color']
```

<div class="output execute_result" execution_count="161">

    0    Black
    1    White
    2    Brown
    Name: Color, dtype: object

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="uUCKXo5IR9w8" outputId="b2738651-1f99-4c7e-b1b7-dc56e471b74b">

``` python
df['Age'].max()
```

<div class="output execute_result" execution_count="162">

    8

</div>

</div>

<div class="cell markdown" id="t6eCk9RFxhkH">

##Print Full Dataframe

</div>

<div class="cell code" id="-KZonCgDgGvv">

``` python
df_covid=pd.read_csv("https://raw.githubusercontent.com/darshanbeniwal/Statistical_Cosmology_using_Python_ICARD_2021/main/Week_9_Feb_01_2022/Covid_19_Jan_16_2022.csv")
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:513}"
id="p9955jIJSlHV" outputId="f6024b3e-b1f1-433f-bbcf-6175f399771a">

``` python
df_covid
```

<div class="output execute_result" execution_count="164">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="DWgwQzq-Styp" outputId="ddead91d-58be-427f-956c-deb32d634868">

``` python
df_covid.dtypes
```

<div class="output execute_result" execution_count="165">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:261}"
id="jHuaBGTGkNAN" outputId="12a4515e-cca3-4279-b3ed-d7a22a81e8a5">

``` python
df_covid.head(5)
```

<div class="output execute_result" execution_count="166">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:295}"
id="ulrTr0HtkZqi" outputId="93f296a9-964f-41d4-997e-71448241b28f">

``` python
df_covid.tail(5)
```

<div class="output execute_result" execution_count="167">

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

<div class="cell code" id="XkUsLqWvy6Xp">

``` python
df=df_covid['Total_Cases']
```

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="A8E4KdJFTPu8" outputId="9a2f581c-6ba2-498f-9b94-9acbff5effe6">

``` python
df
```

<div class="output execute_result" execution_count="169">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:889}"
id="JSvkM9wRTSc2" outputId="4ae2a634-24ba-47d1-8df4-b2725bb91c15">

``` python
df_covid[['Country','Total_Cases']]
```

<div class="output execute_result" execution_count="170">

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

<div class="output display_data">

    <google.colab._quickchart_helpers.SectionTitle at 0x789f799bbdf0>

</div>

<div class="output display_data">

    import numpy as np
    from google.colab import autoviz

    def value_plot(df, y, figscale=1):
      from matplotlib import pyplot as plt
      df[y].plot(kind='line', figsize=(8 * figscale, 4 * figscale), title=y)
      plt.gca().spines[['top', 'right']].set_visible(False)
      plt.tight_layout()
      return autoviz.MplChart.from_current_mpl_state()

    chart = value_plot(_df_0, *['Total_Cases'], **{})
    chart

</div>

<div class="output display_data">

    <google.colab._quickchart_helpers.SectionTitle at 0x789f881c4df0>

</div>

<div class="output display_data">

    import numpy as np
    from google.colab import autoviz

    def histogram(df, colname, num_bins=20, figscale=1):
      from matplotlib import pyplot as plt
      df[colname].plot(kind='hist', bins=num_bins, title=colname, figsize=(8*figscale, 4*figscale))
      plt.gca().spines[['top', 'right',]].set_visible(False)
      plt.tight_layout()
      return autoviz.MplChart.from_current_mpl_state()

    chart = histogram(_df_1, *['Total_Cases'], **{})
    chart

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:206}"
id="QkqXI2riTSZa" outputId="9568e21e-5380-4b3a-8180-81dae78e2c53">

``` python
df_covid[['Country','Total_Cases']].head(5)
```

<div class="output execute_result" execution_count="171">

      Country  Total_Cases
    0   World    326673326
    1     USA     66664283
    2   India     37122164
    3  Brazil     22975723
    4      UK     15146356

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:828}"
id="pKQTOxtCTSVV" outputId="3bfe144b-f952-45f9-d33d-c5dfffe3c5b1">

``` python
df_covid.loc[df_covid['Total_Cases']<1000]
```

<div class="output execute_result" execution_count="172">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="-k2lEojTT4fC" outputId="c6c78773-c0e9-488f-f022-0b88c8a8b311">

``` python
len(df_covid.loc[df_covid['Total_Cases']<1000])
```

<div class="output execute_result" execution_count="173">

    17

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;,&quot;height&quot;:521}"
id="0QL_QCVAT4aS" outputId="ce2048e0-bf88-42dd-f144-e7d226713c36">

``` python
df_covid.corr()
```

<div class="output stream stderr">

    <ipython-input-174-0cef49a8a48f>:1: FutureWarning: The default value of numeric_only in DataFrame.corr is deprecated. In a future version, it will default to False. Select only valid columns or specify the value of numeric_only to silence this warning.
      df_covid.corr()

</div>

<div class="output execute_result" execution_count="174">

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

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="WJ9AD15ZgCbv" outputId="28c17cdc-73e5-4fb7-e169-a475c5587e49">

``` python
print(random.choice(list))
```

<div class="output stream stdout">

    0

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="AWGM8PBOgCY2" outputId="486a100b-b8eb-417f-d4d8-ee7a8e134d4b">

``` python
print(random.choice(string))
```

<div class="output stream stdout">

    s

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="YNgq2bwngCVI" outputId="056d9e04-9c9d-46ed-c70f-69a3cea0f457">

``` python
print(random.choice(tuple))
```

<div class="output stream stdout">

    Dark Energy

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="GuJNXHu9e-56" outputId="09ff2a90-46ac-46f0-b778-018feb420302">

``` python
random.random()
```

<div class="output execute_result" execution_count="182">

    0.19468829303370372

</div>

</div>

<div class="cell markdown" id="JoX5hDsKjCe4">

## Random Shuffle

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="dZ5GNKCRiXlS" outputId="1be478b1-fd2c-4bee-990e-609816d36b6f">

``` python
random.shuffle(list)  #shuffle will only work in list-->It changes the original list
print(list)
```

<div class="output stream stdout">

    [8, 0, 2, 4, 6]

</div>

</div>

<div class="cell markdown" id="rBo4nkqB-x6P">

##Random Sampling

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="Qx0hicv3-vtW" outputId="c261ce2a-92b1-4798-dc71-52e806ad32b2">

``` python
list=[0,2,4,6,8]
random.sample(list,3) #return a particluar list of items without any chnage in origi list
```

<div class="output execute_result" execution_count="184">

    [4, 2, 0]

</div>

</div>

<div class="cell markdown" id="nMwo06xIwyQ3">

## Generate Random Numbers

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="xBu0GoHpuYOG" outputId="33d8f880-3f94-4117-b4b3-87aea556c63b">

``` python
print(random.randint(0,5))  #Generate a Random Number
```

<div class="output stream stdout">

    1

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="PYs7Wd-fwtdJ" outputId="f779dd63-0f06-4344-9e17-cf4ece2b4adb">

``` python
print([random.randint(0,10) for i in range(5)]) #Generate a list of Random Number List
```

<div class="output stream stdout">

    [8, 8, 5, 9, 9]

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="PyZ2pKvxxVHR" outputId="489634b3-b6bb-4c77-86b6-227179d824a4">

``` python
#Alternatively, for Random number list, you can use numpy as
np.random.randint(0,10,5)
```

<div class="output execute_result" execution_count="187">

    array([6, 7, 7, 4, 5])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="lKOw4TsDzz6i" outputId="a00f71d9-6c7a-44b2-97d1-2a86f732c221">

``` python
np.random.randint(0,10,size=5) #Basically the last arguments denotes the size of list
```

<div class="output execute_result" execution_count="188">

    array([5, 8, 3, 7, 8])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="eNMKtneY4Tnr" outputId="4c9520e9-068f-4a33-a8ac-c655b40383e0">

``` python
np.random.randint(0,10,size=(2,5))
```

<div class="output execute_result" execution_count="189">

    array([[2, 9, 1, 6, 1],
           [2, 5, 8, 6, 7]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="nRFje-EE-QLO" outputId="3243575a-b7c1-4c59-899d-5323831e29fc">

``` python
#Suppose you want to generate random floating values using randint
np.random.randint(0,10,size=(2,5)).astype("float")/10
```

<div class="output execute_result" execution_count="190">

    array([[0.8, 0.2, 0.2, 0.9, 0.5],
           [0.1, 0.8, 0. , 0. , 0.8]])

</div>

</div>

<div class="cell code"
colab="{&quot;base_uri&quot;:&quot;https://localhost:8080/&quot;}"
id="y8SMKj3O4smL" outputId="3a69e0cb-883b-4ec6-cf12-892aecafeac6">

``` python
#Alternatively, one can use random_sample
np.random.random_sample(size=(2,5))
```

<div class="output execute_result" execution_count="191">

    array([[0.51246289, 0.91632871, 0.03069853, 0.66503185, 0.0550954 ],
           [0.77538356, 0.24332393, 0.96529977, 0.36469277, 0.88184092]])

</div>

</div>

<div class="cell code" id="Fmj3yyKVi1FD">

``` python
```

</div>
