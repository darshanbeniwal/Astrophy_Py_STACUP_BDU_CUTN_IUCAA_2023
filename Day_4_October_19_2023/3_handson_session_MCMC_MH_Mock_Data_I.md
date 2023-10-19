# 1. Install the required packages

```python
!pip install corner
```
# 2. Import required packages

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.stats import norm,uniform
import corner
```
# 3. Load Mock data from GitHub

```python
x,y,yerr=np.loadtxt("https://raw.githubusercontent.com/darshanbeniwal/Astrophy_Py_STACUP_BDU_CUTN_IUCAA_2023/main/Text_files_Datasets/mock_data_1.txt",unpack=True)
```
# 4. Define Likelihood Function

```python
def likelihood(theta, x, y, yerr):
    a, b= theta
    model = a+b*x
    return (np.sum(-0.5*((y-model)/yerr)**2-0.5*np.log(2*np.pi*yerr**2)))
```
# 5. Define Prior Function

```python

```
# 6. Define Posterior Function

```python

```
# 7. Define Metropolis-Hastings Algorithm Function

```python

```
# 8. Define Initial Seeds, Number of Steps

```python

```
# 9. Run Metropolis-Hastings Algorithm

```python

```
# 10. Plot the chains

```python

```
# 11. Remove Burn-in Phase

```python

```
# 12. Replot the Chains

```python

```
# 13. Find Best Fit value of parameters

```python

```
# 14. Show Parameter Histograms

```python

```
# 15. Plot Contour

```python

```
