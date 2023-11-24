# Awesome-Deep-Learning-Methods-For-Disease-Diagnosis-Based-On-CT-Scans
A Reading List of DL Methods for Disease Diagnosis Based on CT

## 2D
[Sample-Efficient Deep Learning for COVID-19 Diagnosis Based on CT Scans](https://www.medrxiv.org/content/10.1101/2020.04.13.20063941v1.full.pdf); MedRxiv 2020  
**COVID-19:** 提出了一种Self-Trans方法，将对比自监督学习与迁移学习集成，当数据量较小的时候也能取得较好的效果。  
**Dataset:** [COVID-CT](https://github.com/UCSD-AI4H/COVID-CT)


## 3D
[Uniformizing Techniques to Process CT Scans with 3D CNNs for Tuberculosis Prediction](https://link.springer.com/chapter/10.1007/978-3-030-59354-4_15); PRIME 2020  
**Tuberculosis:** 为了节省计算资源，评估了3种统一化3D CT volume的方法，即SSS、ESS和SIZ。第1、2种方法是从3D CT中均匀地选择切片。第3种方法是通过沿z轴插值来利用3D体积的完整几何形状。此外，还设计了一种3D CNN来诊断肺结核。  
**Dataset:** ImageCLEF Tuberculosis Severity Assessment 2019