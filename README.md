# FIGO (focus in and generalize out)
Accurate segmentation of brain stroke using magnetic resonance imaging (MRI) is associated with difficulties due to the complicated anatomy of the brain and the different properties of the stroke. A well-known challenge associated with this problem is the variability in the size and shape of the stroke, which makes it difficult to employ standard segmentation strategies. This study introduces a contextual transformer framework, which synergies spatial feature extraction with global anatomical processing ability, further enhanced by advanced feature fusion and segmentation synthesis techniques. The main idea is based on focus in and generalize out (FIGO), which uses a special pipeline that focus in stroke features with generalization out external anatomical structures. Experimental studies using the ATLAS v2.0 dataset demonstrate a remarkable improvement in segmentation accuracy using FIGO. Ablation studies confirm the significant impact of the proposed framework in comparison with conventional methods.

<img width="1800" height="1970" alt="fig04" src="https://github.com/user-attachments/assets/e2381847-22cf-4700-a6f9-1a2a4aea1991" />
Detailed overview of the FIGO framework. (a) Semantic visualization emphasizes the synergistic combination of the spatial and contextual information processing components. (b) The detailed workflow diagram shows the model’s pivotal components in depth, starting from preprocessing. It also illustrates the flow from U-NetSED for the initial feature extraction, followed by global feature enhancement using Swin-GCE. In this way, the feature fusion, followed by the segmentation synthesis, helps balance the consideration of both local and global features. The process ends with the fusion and final processing, which integrates the outcomes of each segmentation stage and gives us the segmentation result.

# Dataset
The ATLAS v2.0 dataset used in this study is publicly available at https://github.com/npnl/atlas

# Reference
M. Nouman, M. Mabrok, M. al-Shatouri, E. A. Rashed, "Contextual transformer for brain stroke segmentation in MRI," Computers and Electrical Engineering​, 2025 (to appear)
