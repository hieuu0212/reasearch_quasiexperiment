# Scientific Research: The Trade Consequences of Sanctions  

This repository contains the code used to replicate the quantitative analysis of an international economics research project on economic sanctions and international trade.

---

## Overview

The project consists of one main empirical section:

### Section 1: TRADE UNDER PRESSURE: A QUASI-EXPERIMENTAL DESIGN ON SANCTIONS
A quasi-experimental study on the causal effects of sanctions on trade flows, implemented within a staggered Difference-in-Differences framework. The analysis employs:
- Two-Way Fixed Effects  
- Extended Two-Way Fixed Effects  
- Callaway & Sant'Anna (2021) estimator  

---

## Requirements

- Stata 17 or above  
- Required user-written packages:
  - `jwdid` (latest version)

Please ensure that the latest versions of `jwdid.ado` and `jwdid_estat.ado` are installed by overwriting existing versions:  
https://github.com/friosavila/stpackages/tree/main/jwdid

---

## Data

The datasets are not included in this repository.

### Data sources
- Global Sanctions Database (GSDB)  
- Research and Expertise on the World Economy (CEPII)  

### Access
The data can be downloaded from:  
https://drive.google.com/drive/folders/13DpGKoT70Z6LVx6NmO6TrKQrLojECB6O?usp=sharing

---

## How to Run the Replication

1. **Set the working directory in Stata**  
- Open each code file and modify the global paths to match your local directory structure.

2. **Run the data processing pipeline**  
- Open `01_data_processing.do`  
- This script will:
  - Process raw GSDB and CEPII data  
  - Merge datasets  
  - Construct datasets for the empirical analysis  
  - Generate the main dataset:
    - `data_sdid.dta`: dataset used for the quasi-experimental analysis  

3. **Run the empirical analysis**  
- `03_regression_chapter3.do`

4. **Generate figures**  
- Figures are generated using `02_data_graph.do`

---

## Notes

- Replication results may vary depending on system settings and package versions.

---

## Contributors

- M.A. Trinh Minh Quy  
- Dang Minh Nhat  
- Nguyen Trung Hieu  
- Nguyen Minh Khang  
- Ho Trong An  
- Hoang Khac Hung  
- Pham Thieu Ly Na  

---

## Affiliation

University of Economics and Law, Vietnam National University, Ho Chi Minh City  

---

## Contact

For questions or replication issues, please contact:  
- nhatdang0164@gmail.com  
- minhquy0710@gmail.com  
- hieunt23408a@st.uel.edu.vn  
