# Load the required packages 

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

# Load Mock dataset

```python
x_mock=np.array((1.0,2.0,3.0,4.0,5.0))
y_mock=np.array((2.3,4.1,6.2,8.1,10.0))
err_y_mock=np.array((0.08, 0.12, 0.2 , 0.16, 0.28))
```

# Plot datapoint

```python
plt.errorbar(x_mock,y_mock,err_y_mock,fmt='b.')
plt.xlabel('x')
plt.ylabel('y')
plt.show()
```

# Perform Chi-square analysis

```python
a_arr=[]
b_arr=[]
chi_sq_arr=[]
for a in np.arange(0,1,0.001):
    for b in np.arange(0.0,3,0.005):
      chi_sq=0
      for i in range(0,len(x_mock)):
          y_th=a+b*x_mock[i]
          chi_sq1=((y_mock[i]-y_th)/err_y_mock[i])**2
          chi_sq=chi_sq+chi_sq1
      a_arr.append(a)
      b_arr.append(b)
      chi_sq_arr.append(chi_sq)

```

# Save Arrays in a Text file
```python
np.savetxt('store_file.txt',np.transpose([a_arr,b_arr,chi_sq_arr]),fmt='%10.5f',newline='\n',delimiter=' ')

```

# Load text file using Pandas
```python
df = pd.read_csv ('store_file.txt',sep="\s+",names=["a","b","chi2"])

```

# Find minimim   𝜒2   value

```python
df_min=df.loc[df['chi2'].idxmin()]
df_min
```
```python
a_best=0.344
b_best=1.930
x_th=np.arange(0,5,0.01)
y_th=a_best+b_best*x_th

plt.errorbar(x_mock,y_mock,err_y_mock,fmt='b.')
plt.plot(x_th,y_th,'r')
plt.xlabel('x')
plt.ylabel('y')
plt.show()
```
# Estimate Confidence Intervals
## 68.27%  confidence level

```python
df_1_sig = df[(round(df['chi2'], 3) >= round(df_min[2], 3) + 2.2) & (round(df['chi2'], 3) <= round(df_min[2], 3) + 2.4)]
df_1_sig
```

## Plot  68.27%  Confidence Level

```python
plt.plot(df_1_sig['a'],df_1_sig['b'],'b.')
```

## 95.45%  confidence level

```python

```

## Plot  95.45%  Confidence Level

```python

```

## 99.70%  confidence level

```python

```

## Plot  99.70%  Confidence Level

```python

```

# Final Output

```python

```

# Save Final Output

```python

```




