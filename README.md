<div align="center">   

# SSM-Det: State Space Model-based Object Detector for Intelligent Transportation System
</div>

# Abstract 
The State Space Model (SSM) has been a growth of interest in computer vision due to its long-term dependency modeling with linear complexity. Despite massive endeavor, it has not been extensively explored in intelligent transportation system (ITS) yet. 
In this paper, we propose  State  Space Model-based object Detector (SSM-Det), that is meticulously curated with Direction-aware Visual State Space Encoder (D-VSSE). Specifically, it customizes multi-path pixel exchange and patch re-arrangement via four-direction scanning mechanism,  promoting for information communication. To bridge the information bottleneck across high-low level, we further design Split-Fusion (SF) and Skip-Connection (SC) modules for contextual feature propagation before decoding: SF performs multi-channel semantic separation and re-weighting in global-local scope, while SC is responsible for cross-layer feature interaction in a cascaded manner. 
Empirical studies is conducted on both VisDrone2019-DET and SEU\_PML benchmarks, and our proposed SSM-Det reports the state-of-the-art performance against all counterparts by a substantial margin, while maintaining the real-time inference speed. 
We hope this work contributes to the in-depth investigation of SSM-based detector for intelligent transportation applications.

# Pipeline
![SSM-Det pipeline](figure/pipeline.png)
The overall structure of  State Space Model-based object Detector (SSM-Det), that is mainly composed of Backbone, Direction-aware Visual State-Space Encoder (D-VSSE), Split-Fusion (SF), Skip-Connection (SC), Transformer Decoder and Header. After feature extraction, D-VSSE performs the long-term dependency modeling at the expense of linear complexity, and SF-SC fuses multi-scale representations for cross-layer information interaction. Finally, Transformer Decoder adopts Uncertainty-minimal Query Selection and Detection Header for high-quality box prediction. The $\textit{U}$, $\textit{D}$ and $\textit{Rep}$ mark Up-sampled, Down-sampled convolution and Re-parametrization.

#  Quantitative Results
![performance comparisons on VisDrone2019-DET](figure/table3.png)
Performance comparisons with the state-of-the-arts on the Visdrone 2019-DET.
![performance comparisons on seu\_pml](figure/table4.png)
Performance comparisons with the state-of-the-arts on the SEU_PML dataset.

#  Visualization
![Visualization on VisDrone2019-DET](figure/fig7-vis.jpg)
 The result visualization of SSM-Det on VisDrone2019-DET.
![Visualization on VisDrone2019-DET](figure/fig8-seu.jpg)
 The result visualization of SSM-Det on SEU_PML dataset.

#  Datasets
- [VisDrone](https://github.com/VisDrone/VisDrone-Dataset)
- [SEU_PML](https://github.com/vvgoder/SEU_PML_Dataset)

#  Acknowledgment
This code draws inspiration from their work. We sincerely appreciate their excellent contribution.
- [RT-DETR](https://github.com/lyuwenyu/RT-DETR)
- [Mamba](https://github.com/state-spaces/mamba)
- [VMamba](https://github.com/MzeroMiko/VMamba)
#  Citation
```

```