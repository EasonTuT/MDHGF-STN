# MDHGF-STN: Multiscale Dual Hypergraph Fusion Spatiotemporal Network for Traffic Flow Prediction
**Abstract**

Traffic flow prediction is a fundamental challenge in the development of intelligent transportation systems. However, existing spatiotemporal prediction frameworks typically rely on either predefined low-order graphs or single-scale hypergraphs to model urban spatial relationships, which often fail to effectively capture the ubiquitous multiscale high-order spatial characteristics of traffic networks, thereby limiting the model's prediction accuracy and generalization capability. To address this, we propose a high-order spatial-aware traffic flow prediction framework—the Multiscale Dual Hypergraph Fusion Spatiotemporal Network (MDHGF-STN). Specifically, we first introduce a multiscale dual hypergraph construction method, which systematically models high-order spatial features of traffic across three scales: microscopic individual travel intent, mesoscopic community commuting patterns, and macroscopic regional flow propagation. Building upon this foundation, we design a comprehensive prediction framework integrating both spatial-aware and temporal-aware blocks. The spatial-aware block employs hypergraph convolution and dynamic graph convolution to extract dual hypergraph features progressively, incorporates a gating mechanism to fuse high-order local spatial information from multiscale dual hypergraphs, and further utilizes spatial multi-head attention to capture global spatial dependencies. The temporal-aware block effectively extracts both short-term fluctuations and long-term trends in traffic flows through dynamic temporal dilated causal convolution and temporal multi-head attention. Finally, the output layer aggregates spatiotemporal features from stacked spatiotemporal-aware blocks to generate accurate future traffic flow predictions. Extensive comparative experiments on four publicly available real-world traffic flow datasets demonstrate that the proposed model significantly outperforms 16 state-of-the-art baseline models across multiple evaluation metrics.
# Requirements
- python 3.7
- pytorch
- numpy
- pandas

# Data Preparation
MDHGF-STN is implemented on those several public traffic datasets.

PEMS03, PEMS04, PEMS07 and PEMS08 from [BasicTS](https://github.com/GestaltCogTeam/BasicTS).
