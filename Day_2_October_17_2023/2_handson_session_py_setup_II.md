# 1.File handling

## Create/write a file


```python
import numpy as np
```


```python
# Add footer to Text File

x=np.linspace(0,1,10)
y=np.sin(x)
np.savetxt("test_oct_17.txt", np.transpose([x,y]), fmt="%f",delimiter=" ", newline="\n",header='hhh', footer='ff')

```

##  Read a File


```python
# read text file using loadtxt
f= np.loadtxt("test_oct_17.txt")
```


```python
f
```


```python
f[0]
```


```python
# read text file using loadtxt
f= np.loadtxt("test_oct_17.txt",unpack="True")
```


```python
f
```


```python
f[0]
```


```python
f= np.loadtxt("https://raw.githubusercontent.com/darshanbeniwal/Astrophy_Py_STACUP_BDU_CUTN_IUCAA_2023/main/Text_files_Datasets/Hubble_30.txt",unpack="True")
```


```python
f
```

## Delete a File


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

# 2.Plot data using Matplotlib


```python
import matplotlib.pyplot as plt #Now the Pyplot package can be referred to as plt.
import numpy as np
```

##Errorbar Plots


```python
x=np.arange(0,10,1)
y=np.array((1,3,2,6,5,3,4,5,9,3))
y_err=y*0.3
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.xlabel('x')
plt.ylabel('y')
```

##Save Plot


```python
x=np.arange(0,10,1)
y=np.array((1,3,2,6,5,3,4,5,9,3))
y_err=y*0.3
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.xlabel('x')
plt.ylabel('y')
```

##Confidence levels regions


```python
x=np.arange(0,10,1)
y=np.array((1,2,3,2.8,2.4,2,2.3,2.7,2.3,2))
y_err=y*0.1
plt.errorbar(x,y,y_err,fmt='b.',capsize=3,ecolor='r',elinewidth=1)
plt.fill_between(x, y+1.*y_err, y-1.*y_err, facecolor='#F08080', alpha=0.99)
plt.fill_between(x, y+2.*y_err, y-2.*y_err, facecolor='#F08080', alpha=0.59)
plt.fill_between(x, y+3.*y_err, y-3.*y_err, facecolor='#F08080', alpha=0.39)

```

# 3.Dataframe using Pandas

## Import Packages


```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```


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

# 4.Random Number Operations


```python
import random
```

## Random Items from list, tuple \& string

## Generate Random Numbers


```python
np.random.randint(0,10,1)

```


```python
n_rndm=np.random.randint(0,10,15)
n_rndm
```


```python
plt.hist(n_rndm,bins=15)
plt.show()
```

## Uniform Random Number


```python
import numpy as np

random_numbers = np.random.uniform(-1, 1, 10)

random_numbers
```


```python
plt.hist(random_numbers, bins=20,  color='blue', edgecolor='black')
# plt.hist(random_numbers, bins=20, density=True, color='blue', edgecolor='black')

```

##Gaussian Random Number


```python
n_Gauss = np.random.normal(0, 1, 100)
plt.hist(n_Gauss, bins=20, density=True, color='blue', edgecolor='black')

```


```python
mean=0
std_dev=1
n_Gauss = np.random.normal(mean, std_dev, 100)

x=np.arange(-5,5,0.1)

pdf = (1 / (std_dev * np.sqrt(2 * np.pi))) * np.exp(-0.5 * ((x - mean) / std_dev) ** 2)

plt.plot(x, pdf, color='red', label='Theoretical Gaussian')
plt.hist(n_Gauss, bins=20,  density=True, color='blue', edgecolor='black',label='Gaussian-Random Data')

plt.xlabel('Value')
plt.ylabel('Probability Density')
plt.legend()

```


```python

```
