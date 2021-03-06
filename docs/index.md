# PyCO2SYS

[![PyPI version](https://badge.fury.io/py/PyCO2SYS.svg)](https://badge.fury.io/py/PyCO2SYS) [![DOI](https://zenodo.org/badge/237243120.svg)](https://zenodo.org/badge/latestdoi/237243120)

PyCO2SYS is a Python implementation of CO<sub>2</sub>SYS [[LW98](refs/#LW98), [HPR11](refs/#HPR11), [OEDG18](refs/#OEDG18)], the MATLAB toolbox for marine carbonate system calculations.

## Installation and use

Install from the Python Package Index:

    pip install PyCO2SYS

Update an existing installation:

    pip install PyCO2SYS --upgrade --no-cache-dir

Import and use very much like in MATLAB with:

```python
from PyCO2SYS import CO2SYS
CO2dict = CO2SYS(PAR1, PAR2, PAR1TYPE, PAR2TYPE, SAL, TEMPIN, TEMPOUT, PRESIN, PRESOUT,
    SI, PO4, pHSCALEIN, K1K2CONSTANTS, KSO4CONSTANTS, NH3=0.0, H2S=0.0, KFCONSTANT=1)
```

See the [Github repo README](https://github.com/mvdh7/pyco2sys#pyco2sys) for more details on the inputs and outputs.

## Citation

See [the original MATLAB repo](https://github.com/jamesorr/CO2SYS-MATLAB) for more detailed information on versions and citation.

  * If you use any CO<sub>2</sub>SYS-related software, please cite the original work by Lewis and Wallace (1998) [[LW98](refs/#LW98)].
  * If you use CO2SYS.m, please cite van Heuven et al. (2011) [[HPR11](refs/#HPR11)].
  * If you use errors.m or derivnum.m, please cite Orr et al. (2018) [[OEDG18](refs/#OEDG18)].
  * If you use PyCO2SYS, please mention it somewhere along with the DOI: [![DOI](https://zenodo.org/badge/237243120.svg)](https://zenodo.org/badge/latestdoi/237243120)

Please mention which version of PyCO2SYS you used. **Note that each version has a different DOI - please use the correct one!**

You can find the current version that you are using in Python with:

```python
from PyCO2SYS.meta import version
print('This is PyCO2SYS v{}'.format(version))
```

The DOIs for each version (starting at v1.2.0) are listed in the [documentation of the version history](versions).

## About

PyCO2SYS is maintained by [Dr Matthew P. Humphreys](https://mvdh.xyz) at NIOZ Royal Netherlands Institute for Sea Research, Department of Ocean Systems (OCS), and Utrecht University, Texel, the Netherlands.
