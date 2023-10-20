# To set range of parameters in contour plots
```python
param_limits = [(71, 73), (0.5, 0.9)]
fig = corner.corner(samples_MH,bins=40,color="b",labels=['$H_0$','$z_{t}$'],truths=[h0_best,zt_best],fill_contours=True,
                    levels=(0.68,0.95,0.99,),
                    smooth=True,
                    range=param_limits,
                    quantiles=[0.16, 0.5, 0.84],title_fmt='.3f',plot_datapoints=False,show_titles=True)

```
