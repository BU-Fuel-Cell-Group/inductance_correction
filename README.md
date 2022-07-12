# Inductance Correction

This repository accompanies our JOM article, submitted for publication in August 2022. Please see our original paper for details of this inductance correction procedure. The following functions are included in the Impedance_correction_functions.ipynb file:<br />

1. correct_known_inductance(f,Z,L): takes impedance data (f and complex Z arrays) and returns impedance data that has been corrected for a known L.
2. correct_inductance(f,Z,f_min, f_max): corrects impedance data for inductance, which is automatically calculated by fitting Z" vs. f at high frequencies.
3. remove_ohmic(f,Z): removes the ohmic resistance from impedance data
4. remove_ohmic_manual(f,Z,R): removes a known ohmic resistance from impedance data
5. clean_linkk(f,Z,p): removes data points from EIS spectra with linKK residuals greater than p%

## Required Packages

**impedance.py**<br />
Murbach, M. D., Gerwe, B., Dawson-Elli, N., and Tsui, L. impedance.py: A Python package for electrochemical impedance analysis, Journal of Open Source Software, 5(52), 2349 (2020).

**csv<br />
pandas<br />
cmath<br />
numpy<br />
matplotlib<br />
mpl_toolkits**

<br />We recommend you install the above packages to a new environment before running the included Jupyter notebooks.

