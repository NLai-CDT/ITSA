# Individual Tangent Space Alignment (ITSA)
This is repository for "Cross-Subject and Cross-Montage EEG Transfer Learning for Robust Gait Adaptation Detection" (pre-print can be found: https://doi.org/10.48550/arXiv.2508.08216)

# Notebooks
The repository contains the following notebooks:
1. ITSA_Transformation.ipynb - Implements ITSA pipeline to recentre, rescale and rotate EEG training and testing trials to improve transfer learning. 
2. HybridRCSPRie_Classification.ipynb - Implements hybrid feature extraction including "Seq. RCSP - Rie" and "Par. RCSP-Rie". ITSA transformed training and testing features are extracted using Regularised Common Spatial Patterns (RCSP) and Riemannian geometry-based methods. The extracted features are subsequently classified using a LOSO-CV. 

# Requirements 
- numpy
- pandas==2.0.3
- scipy==1.10.1
- scikit-learn
- jupyter
- pyriemann==0.5
  
# How to Run
1. Segment EEG signal into windows and include corresponding labels
2. Clone or download this repository.
3. Install the required dependences.
4. Launch Jupyter Notebook or JupyterLab.
5. Open either .ipynb file.
6. Run the cells in order.
   
# Data
Dataset used for results reported in "Cross-Subject and Cross-Montage EEG Transfer Learning for Robust Gait Adaptation Detection" are from a publicly available dataset (J. Wagner et al., ‘High-density EEG mobile brain/body imaging data recorded during a challenging auditory gait pacing task’, Sci Data, vol. 6, p. 211, Oct. 2019, doi: 10.1038/s41597-019-0223-2 https://www.nature.com/articles/s41597-019-0223-2).The dataset is available at OpenNeuro.org with accession number ds00197144.

