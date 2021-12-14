<div align="center">    
 
# Predicting Myocardial Injury Using ED Monitoring Data

</div>

## Description   
This repository contains notebooks used in the pre-processing, model training, and analysis of the Myocardial Injury study. This study aimed to use transfer-learning on single-lead ECGs to help predict the presence of myocardial injury based based on continuous monitoring data and patient cohort information available in the emergency department (ED). This study specifically looks at NSTEMI patients who were admitted based on a complaint of chest pain or shortness of breath. 

Note that all PHI data has been removed from the notebooks. However, the data used in this study contain protected health information and are therefore not publicly available. A de-identified dataset sufficient to reproduce the key analyses will be available from the corresponding author upon reasonable request.

### Pre-Trained Model
The Transformer base model ("PRNA") is described in [this paper](https://ieeexplore.ieee.org/document/9344053). The model has currently been modified to use only Lead-II ECGs, matching the monitoring data available from the Philips IntelliVue monitors.

### Emergency Department Data
Refer to [this repository](https://github.com/stanfordmlgroup/ed-monitor-data/) for data structure and the `edm` module which contains shared library code.
