# WaveUNet
WaveUNet is a novel deep learning framework for InSAR phase unwrapping, combining Discrete Wavelet Transform (DWT) with Attention Mechanisms to achieve state-of-the-art performance. This repository contains the official implementation of our paper.

For local mining-area funnel phase unwrapping using WaveUNet, please use the following repository: https://github.com/xiangHQ/WaveUNet-for-local-mining-area-funnel-phase-unwrapping.git

Flowchart of this study

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
📝 Correction to Eq. (3)
Please note that Eq. (3) in the published paper contains a typographical error in the spatial attention formulation. The equation

A
=
Softmax
(
Q
T
K
)

should be corrected to

A
=
Softmax
(
Q
K
T
)
.
