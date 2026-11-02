# WaveUNet
WaveUNet is a novel deep learning framework for InSAR phase unwrapping, combining Discrete Wavelet Transform (DWT) with Attention Mechanisms to achieve state-of-the-art performance. This repository contains the official implementation of our paper.
For local mining-area funnel phase unwrapping using WaveUNet, please use the following repository: https://github.com/xiangHQ/WaveUNet-for-local-mining-area-funnel-phase-unwrapping.git
Flowchart of this study
<img width="4663" height="2921" alt="image" src="https://github.com/user-attachments/assets/e8760644-0cab-47d6-9691-6d9083661d76" />
*Figure 1: Overall architecture of the proposed WaveUNet framework*

✨ Key Features

Wavelet-based Multi-scale Analysis: Leverages DWT to capture both global and local phase patterns
Attention Mechanism: Enhances feature representation in challenging regions (steep slopes, discontinuities)
End-to-End Learning: Direct mapping from wrapped to unwrapped phase
Efficient Architecture: Balanced trade-off between accuracy and computational cost

🏗️ Model Architecture

The WaveUNet consists of three main components:
Encoder: Hierarchical feature extraction with DWT-based downsampling
Bottleneck: Attention-augmented feature transformation
Decoder: Progressive upsampling with skip connections

📊 Dataset
InSAR-DLPU dataset: https://github.com/zhoulifan/InSAR-DLPU.git

📋 Requirements
Python >= 3.8
PyTorch >= 1.11.0
CUDA >= 11.0 (optional, for GPU acceleration)

** The original link is follows:
https://github.com/xiangHQ/WaveUNet.git
# Please reference the paper: WaveUNet
An efficient deep network based on discrete wavelet transform and attention mechanism for InSAR phase unwrapping
(https://www.sciencedirect.com/science/article/abs/pii/S092427162600331X)
