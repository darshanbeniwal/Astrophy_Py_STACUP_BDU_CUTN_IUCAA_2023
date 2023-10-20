# Code
```python
r,rerr,theta_deg,thetaerr_deg=np.loadtxt("https://raw.githubusercontent.com/darshanbeniwal/Astrophy_Py_STACUP_BDU_CUTN_IUCAA_2023/main/Text_files_Datasets/mars_orbit_data.txt",unpack=True)
the=theta_deg*np.pi/180
theerr=thetaerr_deg*np.pi/180


def likelihood(theta, the, r, rerr):
    a,e,w= theta
    model = a/(1+e*np.cos(the-w))
    # err_T=np.sqrt(rerr**2+(((e*a*np.sin(the-w))/(e*np.cos(the-w)+1)**2)*theerr)**2)
    return (np.sum(-0.5*((r-model)/(rerr))**2-0.5*np.log(2*np.pi*(rerr)**2)))

def prior(theta):
    a, e, w= theta
    if 0< a < 2 and -0.1 < e < 0.5 and -0.5 < w < 0.6:
        return np.log10(1.0 / ((2 - 0.0) * (0.5 + 0.5)* (0.5 + 0.5)))
    return -np.inf
```

