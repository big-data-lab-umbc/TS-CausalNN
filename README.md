# TS-CausalNN: Learning Temporal Causal Relations from Non-linear Non-stationary Time Series Data

## Abstract 

The growing availability and importance of time series data across various domains, including environmental science, epidemiology, and economics, has led to an increasing need for time-series causal discovery methods that can identify the intricate relationships in the non-stationary, non-linear, and often noisy real world data. However, the majority of current time series causal discovery methods assume stationarity and linear relations in data, making them infeasible for the task. Further, the recent deep learning-based methods rely on the traditional causal structure learning approaches making them computationally expensive. In this paper, we propose a Time-Series Causal Neural Network (TS-CausalNN) - a deep learning technique to discover contemporaneous and lagged causal relations simultaneously. Our proposed architecture comprises (i) convolutional blocks comprising parallel custom causal layers, (ii) acyclicity constraint, and (iii) optimization techniques using the augmented Lagrangian approach. The proposed model learns non-stationary features from input data through learning and aggregating nonlinear functions. Finally, using these learned nonlinear features, the parallel custom causal convolution 2D layers learn causal connections between different variables. Through experiments on multiple synthetic and real world datasets, we demonstrate the empirical proficiency of our proposed approach as compared to several state-of-the-art methods. The inferred graphs for the real world dataset are in good agreement with the domain understanding. 

## Code
This repository contains the code implementation of our proposed model and all the baseline models we have compared for performance evaluation. Also, the ablation study codes are available here. A summary of all directories is given below. 

- baselines: This directory contains all the notebooks with baseline models applied to different datasets.  
- datasets: Real wrold and synthetic datasets used for this paper are available in this directory. The synthetic dataset generation codes are also available here.
- proposed_model: The proposed model is available here. The notebooks in this directory contain experimental results for different datasets using the proposed mode.
- ablation_study: For the ablation study, we have created a variant of the proposed model. The implementation of this variant and results for different datasets are available in this directory.

## Citation
If you use this code for your research, please cite our [paper]():

```
@article{tscausalnn2025,
  title={TS-CausalNN: Learning Temporal Causal Relations from Non-linear Non-stationary Time Series Data},
  author={Faruque, Omar and Ali, Sahara and Zheng, Xue and Wang, Jianwu},
  journal={IEEE International Conference on Data Mining (ICDM) Workshop of Artificial Intelligence for Time Series Analysis (AI4TS)},
  year={2025},
  publisher={IEEE}
}
