<div align="center">    
 
# Predicting Myocardial Injury from Continuous Single-Lead Electrocardiographic Monitoring in the Emergency Department

</div>

## Description   
This repository contains notebooks used in the pre-processing, model training, and analysis for "Predicting Myocardial Injury from Continuous Single-Lead Electrocardiographic Monitoring in the Emergency Department". This study uses transfer learning from 12-lead ECGs to detect myocardial injury using continuous single-lead monitoring data and patient information available shortly after ED arrival. The primary target of prediction is NSTEMI, i.e., presence of new troponin elevation in patients with chest pain or shortness of breath. 

All protected health information (PHI) has been removed from the notebooks. However, study data contain PHI and are therefore not publicly available. A de-identified dataset sufficient to reproduce the key analyses will be available from the corresponding author upon reasonable request.

### Pre-Trained Model
The Transformer base model ("PRNA") is described in [this paper](https://ieeexplore.ieee.org/document/9344053). The model was modified to use the lead II ECG waveforms from the Philips IntelliVue monitors.

### Emergency Department Data
Refer to [this repository](https://github.com/stanfordmlgroup/ed-monitor-data/) for data structure and the `edm` module which contains shared library code.
