# Awesome-Deep-Learning-Methods-For-Disease-Diagnosis-Based-On-CT-Scans
A Reading List of DL Methods for Disease Diagnosis Based on CT

## 2D Methods
[ImageCLEF 2019: Deep Learning for Tuberculosis CT Image Analysis](https://ceur-ws.org/Vol-2380/paper_54.pdf); CLEF (Working Notes) 2019  
**Tuberculosis:** 使用了两种切片选择方法，基于被选切片，利用2D CNN来提取特征，最后实现预测肺结核严重程度和生成CT报告两个任务。两种切片选择方法：1）医生选择；2）选择中间层的N个切片。  
**Dataset:** ImageCLEF Tuberculosis 2019

[ImageCLEF 2019: Projection-based CT Image Analysis for TB Severity Scoring and CT Report Generation](https://ceur-ws.org/Vol-2380/paper_70.pdf); CLEF (Working Notes) 2019  
**Tuberculosis:** 提出了一种自动分析3D CT的方法，将3D CT表示为沿三个轴的一组2D投影图像，每个轴2张，共6张。这种方法降低了输入数据的维度，因此允许使用不太复杂的模型来执行图像分类任务。  
**Dataset:** ImageCLEF Tuberculosis 2019

[Multi-View CNN with MLP for Diagnosing Tuberculosis  Patients Using CT Scans and Clinically Relevant  Metadata](https://www.researchgate.net/profile/U-Cevik/publication/334654878_Multi-View_CNN_with_MLP_for_Diagnosing_Tuberculosis_Patients_Using_CT_Scans_and_Clinically_Relevant_Metadata/links/5d387e58299bf1995b47dc1a/Multi-View-CNN-with-MLP-for-Diagnosing-Tuberculosis-Patients-Using-CT-Scans-and-Clinically-Relevant-Metadata.pdf); 

[Sample-Efficient Deep Learning for COVID-19 Diagnosis Based on CT Scans](https://www.medrxiv.org/content/10.1101/2020.04.13.20063941v1.full.pdf); MedRxiv 2020  
**COVID-19:** 提出了一种Self-Trans方法，将对比自监督学习与迁移学习集成，当数据量较小的时候也能取得较好的效果。  
**Dataset:** [COVID-CT](https://github.com/UCSD-AI4H/COVID-CT)


## 3D Methods
[Estimating Severity from CT Scans of Tuberculosis Patients using 3D Convolutional Nets and Slice Selection](https://www.researchgate.net/profile/Hasib-Zunair/publication/334680379_Estimating_Severity_from_CT_Scans_of_Tuberculosis_Patients_using_3D_Convolutional_Nets_and_Slice_Selection/links/5e585b99a6fdccbeba079f36/Estimating-Severity-from-CT-Scans-of-Tuberculosis-Patients-using-3D-Convolutional-Nets-and-Slice-Selection.pdf); CLEF (Working Notes) 2019  
**Tuberculosis:** 针对每个3D volume，选择the first 4 slices, the middle 8 silces and the last 4 silces，总共16个切片，并利用3D CNN网络来诊断肺结核。  
**Dataset:** ImageCLEF Tuberculosis 2019

[Improving Tuberculosis (TB) Prediction Using Synthetically Generated Computed Tomography (CT) Images](https://openaccess.thecvf.com/content/ICCV2021W/CVAMD/papers/Lewis_Improving_Tuberculosis_TB_Prediction_Using_Synthetically_Generated_Computed_Tomography_CT_ICCVW_2021_paper.pdf); ICCVW 2021  
**Tuberculosis:** 利用多视角的X-ray生成3D CT，诊断肺结核。  
**Dataset:** PAthology Detection in Chest radiographs

[Lung nodule detection and classification from Thorax CT-scan using RetinaNet with transfer learning](https://www.sciencedirect.com/science/article/pii/S1319157820303335); J KING SAUD UNIV-COM 2022  
**Lung Nodule:** 提出了I3DR-Net用于肺结节检测和分类。  
**Dataset:** LIDC, Moscow Private Dataset

[Reinventing 2D Convolutions for 3D Images](https://ieeexplore.ieee.org/abstract/document/9314699); JBHI 2021  
**Multi-tasks:** 提出了ACS (axial-coronal-sagittal)卷积，可以应用在各种3D医学图像处理任务上，来减少计算资源的消耗。  
**Dataset:** LIDC-IDRI, LiTS, DeepLesion

[Uniformizing Techniques to Process CT Scans with 3D CNNs for Tuberculosis Prediction](https://link.springer.com/chapter/10.1007/978-3-030-59354-4_15); PRIME 2020  
**Tuberculosis:** 为了节省计算资源，评估了3种统一化3D CT volume的方法，即SSS、ESS和SIZ。SSS是选择前4个、中8个和后4个切片；ESS是从3D CT中均匀地选择切片；SIZ是通过沿z轴插值来利用3D体积的完整几何形状。此外，还设计了一种3D CNN来诊断肺结核。  
**Dataset:** ImageCLEF Tuberculosis Severity Assessment 2019