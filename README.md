# BlockedVesselMeshing

All dependencies listed in requirements.txt, though not all are needed for the core functionality..

Project structure:

* `data/`
    - `input/`: Currently contains 5 datasets from different sources, with each having the original data in the `raw/` subfolder, and the (standardized) data in the `skeleton/`.
* `python/`: Source code. Most of the main functionality lies in the root, with `clusters.py` implementing the cluster splitting and `blocked.py` implementing the blocked approach.
    - `preprocessing/`: Code to convert input mesh formats into our standardized skeletons as well as the preprocessing pass which improves skeleton niceness.
    - `rainbow/`: A math library used as utility.
    - `tools/`: Various custom utilities and data formats.


## References
Data sourced from;

#### Kidney
```
XU P., HOLSTEIN-RATHLOU N.-H., SØGAARD S. B., GUNDLACH C., SØRENSEN C. M., ERLEBEN K., SOSNOVTSEVA O., DARKNER S.:
A hybrid approach to full-scale reconstruction of renal arterial network.
Scientific Reports 13, 1 (2023), 7569.
```

#### Lung
```
STØVERUD K.-H., BOUGET D., PEDERSEN A., LEIRA H. O., LANGØ T., HOFSTAD E. F.:
AeroPath: An airway segmentation benchmark dataset with challenging pathology, 2023.
arXiv: 2311.01138. 
```

#### Liver
```
JESSEN E., STEINBACH M. C., DEBBAUT C., DOMINIK S.:
Rigorous mathematical optimization of synthetic hepatic vascular trees.
Journal of the Royal Society Interface (2022)
```

#### Brain
```
SHEN J., FARUQI A. H., JIANG Y., MAFTOON N.:
Mathematical reconstruction of patient-specific vascular networks based on clinical images and global optimization.
IEEE Access 9 (2021), 20648–20661. doi:10.1109/ACCESS.2021.3052501.
```

#### Tree
```
DU S., LINDENBERGH R., LEDOUX H., STOTER J., NAN L.:
Adtree: Accurate, detailed, and automatic modelling of laser-scanned trees.
Remote Sensing 11, 18 (2019), 2074.
```
