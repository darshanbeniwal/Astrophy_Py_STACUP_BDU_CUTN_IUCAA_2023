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
x,f_x,f_x_err = np.loadtxt('https://raw.githubusercontent.com/darshanbeniwal/Astrophy_Py_STACUP_BDU_CUTN_IUCAA_2023/main/Text_files_Datasets/mock_data_2.txt', unpack=True)
```


# 4. Solve Integration

```python
from scipy.integrate import quad

def g_t(t, a, b):
    return (a + b * t)

def integrand(t, a, b):
    return (1 / g_t(t, a, b))

def f_x_th(x, a, b):
    integrals = []
    for xi in x:
        result, error = quad(integrand, 0, xi, args=(a, b))
        integrals.append(result)
    return np.array(integrals)
```

# 5. Define Likelihood Function

```python
def likelihood(theta, x, f_x, f_x_err):
    a, b= theta
    model = f_x_th(x, a, b)
    return (np.sum(-0.5*((f_x-model)/f_x_err)**2-0.5*np.log(2*np.pi*f_x_err**2)))
```
# 6. Define Prior Function

```python
def prior(theta):
    a, b= theta
    if 0.0< a < 1 and 5.0 < b < 10.0:
        return np.log10(1.0 / ((1 +1.0) * (10.0 - 5.0)))
    return -np.inf
```
# 7. Define Posterior Function

```python
def posterior(theta, x, f_x, f_x_err):
    lp = prior(theta)
    if not np.isfinite(lp):
        return -np.inf
    return (lp + likelihood(theta, x, f_x, f_x_err))
```
# 8. Define Metropolis-Hastings Algorithm Function

```python
def Metropolis_Hastings(parameter_init, nsteps):
    result = []  # List to store the sampled parameter values
    result.append(parameter_init)  # Add the initial parameter values to the result list
    for t in range(nsteps):  # Iterate over the specified number of steps
        step_var = [0.1, 1]  # Variance of the proposal distribution for each parameter
        proposal = norm.rvs(loc=result[-1], scale=step_var)  # Generate a proposal parameter value from a normal distribution
        probability = np.exp(posterior(proposal,x, f_x, f_x_err) - posterior(result[-1],x, f_x, f_x_err))  # Calculate the acceptance probability
        if (uniform.rvs() < probability):  # Accept the proposal with the acceptance probability
            result.append(proposal)  # Add the proposal to the result list
        else:
            result.append(result[-1])  # Reject the proposal and add the previous parameter value to the result list
    return(result)  # Return the sampled parameter values
```
# 9. Define Initial Seeds, Number of Steps

```python
a_ini,b_ini=0.5,6.1
initials=a_ini,b_ini
ndim=2
nsteps=30000
```
# 10. Run Metropolis-Hastings Algorithm

```python
result = Metropolis_Hastings(initials, nsteps)
samples_MH=np.array(result)
```
# 11. Plot the chains

```python
fig, axes = plt.subplots(2, 1, figsize=(8, 8))
samples = samples_MH.T

# Plot the traceplot of H0
axes[0].plot(samples[0], "g")
axes[0].set_ylabel("$a$")

# Plot the traceplot of Om
axes[1].plot(samples[1], "r")
axes[1].set_ylabel("$b$")
```
# 12. Remove Burn-in Phase

```python
nburn_in=200
result_b = result[nburn_in:]
samples_MH_b=np.array(result_b)
```
# 13. Replot the Chains

```python
fig, axes = plt.subplots(2, 1, figsize=(8, 8))
samples_b = samples_MH_b.T

# Plot the traceplot of H0
axes[0].plot(samples_b[0], "g")
axes[0].set_ylabel("$a$")

# Plot the traceplot of Om
axes[1].plot(samples_b[1], "r")
axes[1].set_ylabel("$b$")
```
# 14. Find Best Fit value of parameters

```python
a_chain=samples_MH_b[:,0]
b_chain=samples_MH_b[:,1]
#Estimate the mean of a and b chains
a_best = np.mean(a_chain)
b_best = np.mean(b_chain)

#Estimate the Std. Deviation of a and b chains

sig_a = np.std(a_chain)
sig_b = np.std(b_chain)

print("Best fit values:")
print("a:",a_best, "Sig_a:", sig_a)
print("b:",b_best, "Sig_b:", sig_b)

```
# 15. Show Parameter Histograms

```python
plt.figure(figsize=(8, 3)) #Plot Size

# Plot the histogram of a
plt.subplot(1, 2, 1)
plt.hist(a_chain, bins=100, color='blue')
plt.xlabel('a')
plt.ylabel('Count')

# Plot the histogram of b
plt.subplot(1, 2, 2)
plt.hist(b_chain, bins=100, color='blue')
plt.xlabel('b')
plt.ylabel('Count')
```
# 16. Plot Contour

```python
fig = corner.corner(samples_MH,bins=50,color="b",labels=['a','b'],truths=[a_best,b_best],fill_contours=True,
                    levels=(0.68,0.95,0.99,),smooth=True,
                    quantiles=[0.16, 0.5, 0.84],title_fmt='.3f',plot_datapoints=False,show_titles=True)

```
