# Code_for_cal_gBOLD_CSF
Minimal MATLAB example for computing gBOLD–CSF coupling
# gBOLD–CSF Coupling Demo

This repository provides a minimal MATLAB implementation of the gBOLD–CSF coupling analysis, based on the method described by Fultz et al. (Science, 2019), and utilized in our ongoing study submitted to Brain Communications (Zhang et al., 2025).

---

## 📂 Files

- `demo_main.m` – main script for group-level gBOLD–CSF coupling computation  
- `compute_gBOLD_CSF_coupling.m` – computes cross-correlation between gBOLD and CSF time series  
- `compute_gBOLD_derivative_correlation.m` – computes correlation between CSF and the negative first derivative of gBOLD  
- `permutation_test_coupling.m` – performs a permutation-based significance test (10,000 iterations)  

---

## 🚀 Usage

Open MATLAB and run:

```matlab
load('example_gbold.mat');  % [T x N] matrix of gBOLD signals
load('example_csf.mat');    % [T x N] matrix of CSF signals
demo_main
