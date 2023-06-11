## 1. _[ASMS_MAY2020_Poster_Bifarin_final]_ 
## Machine Learning Predicts Renal Cell Carcinoma Status from Urine Using Multiplatform Metabolomics.
My poster presentation at the American Society for Mass Spectrometry (ASMS) Conference 2020 on detecting kidney cancer with machine learning and urine-based metabolomics

### Introduction
Due to the characteristic asymptomatic progression of Renal Cell Carcinoma (RCC), an early diagnosis of RCC greatly improves survival. Currently, RCC is detected through cross-sectional imaging, followed by renal mass biopsy, which is invasive and riddled with sampling errors. Hence, there is a critical need for a non-invasive diagnostic assay. RCC is a disease of altered cellular metabolism with the tumor(s) in close proximity to the urine in the kidney suggesting metabolomic profiling would an excellent choice for assay development.

### Methods
We applied machine learning (ML) techniques to predict RCC status from an integrated liquid chromatography/mass spectrometry (LC/MS) and nuclear magnetic resonance (NMR) metabolic profile. NMR spectroscopy and LC/MS experiments were collected for urine from 82 RCC patients and 174 healthy controls. The cohort was divided into two sub-cohorts for training and validation purposes. Discriminatory 1H NMR and MS features were selected using an embedded based feature selection pipeline applied to the training cohort. Three ML techniques with different induction biases were used for training and hyperparameter tuning. Final assessment of RCC status prediction was made using the selected features and the tuned ML algorithms on the test cohort.

### Preliminary Results
The model cohort consists of a pair of 31 healthy controls and RCC samples selected using a propensity score matching algorithm (PSM). After PSM, the cohort were gender matched (17 males, 14 females), and had statistically insignificant difference in age (Student t-test p-value=0.64) and BMI (Student t-test p-value=0.06). Smoking history and race’s statistics also improved considerably when compared to the pre-matched cohort. In addition, all RCC stages were represented – early stage RCC (I/II) represents 55% while the late stage RCC (III/IV) represents 45% of the model cohort. Using this model cohort, 49 NMR features and >6000 LC-MS features were filtered to 132 features using the following methods: >2-fold difference between groups, q <0.05 (Student t-test, FDR Benjamin-Hochberg), and removal of highly correlated features (Pearson's correlation coefficient, r >0.8). Next, we used a random forest recursive - feature elimination (RF-RFE) technique and partial least square regression discriminant analysis (PLS-DA) to select the top 20 discriminatory features, using Gini index and VIP scores respectively. The ten metabolic features that overlapped between the two sets was selected as the metabolic panel. The panel were used to train and tune selected hyperparameters in Random Forest (RF), K-nearest neighbor (k-NN), and support vector machine (SVM-Lin and SVM-RBF) classifiers in the model cohort. In the test cohort (healthy controls=143, RCC=51), the best ML model using Random Forest classifiers, discriminated RCC and healthy controls with an accuracy, sensitivity, and specificity of 98% under cross-validation conditions. 2-aminoacetophenone was one of the tentative metabolic biomarkers discovered among the selected features. The identification of metabolic panel is underway.  

### Novel Aspect
Our results provide evidence that RCC diagnosis may be possible via a routine urine test. 

## 2. _[ASMS_JUNE2022_Poster_Bifarin_final]_ 
## Ovarian Cancer Lipidome Dynamics in a _Dicer-Pten_ Double-Knockout Mouse Model.
My poster presentation at the American Society for Mass Spectrometry (ASMS) Conference 2022

### Introduction
Ovarian cancer (OC) is responsible for more deaths than any other cancer associated with the female reproductive system. In addition, it is the fifth leading cause of cancer-related death in women. This is particularly the case because of the low survival rate associated with late diagnosis coupled with nonspecific symptoms at early stages. Particularly deadly is high-grade serous carcinoma (HGSC), the most frequent type of OC. 

### Methods
An HGSC Dicer-Pten Double-Knockout (DKO) mouse model was used to study the dynamics of lipidome changes in this OC subtype. DKO mice mimic many features of the human disease. For example, it originates in the fallopian tube before spreading to the ovary and the abdominal cavity. After two months of breeding, serum samples of DKO (n = 15) and DKO control (n = 15) mice were collected every two weeks for six months. Ultra-high performance liquid chromatography−mass spectrometry (UHPLC−MS) was used for serum lipidomic profiling.  The dynamics of lipidomic changes were studied using univariate statistical methods, hierarchical clustering analysis, machine learning, and survival analysis. 

### Preliminary Results
Eighty-seven significant lipidomic features (Student’s T-test p-value < 0.05) were identified when DKO was compared with DKO control for all time points combined. Given the different death rate profile of control and DKO mice, each time point collection was converted to a percentage of the total lifetime of the individual mice, making the group comparison more robust. Percentage lifetimes were then binned into five different stages (0-30%, 30-45%, 45-60%, 60-75%, and 75-100% lifetime). Hierarchical clustering analysis revealed the clustering of longitudinal lipid abundance trajectories into four selected clusters, associated with distinct lipid phenotypes.  Machine learning was used for DKO classification for the five different stages of OC progression, with the highest classification performance at 46-60% lifetime (Test set ROC AUC = 0.85). Altered lipid levels were observed for fatty acids (FA) and their derivatives, phospholipids, and sphingolipids. Early progression of OC is marked by increased levels of phosphatidylcholines and phosphatidylethanolamines. In contrast, later stages were marked by more diverse lipids alterations, including FA and FA derivatives, triglycerides, ceramides, hexosylceramides, sphingomyelins, lysophosphatidylcholines, and phosphatidylinositols. These alterations provided evidence of perturbations in cell membrane stability, cellular proliferation, and survival. 

### Novel Aspect
Our study provides the first in-depth, longitudinal lipidome dynamics study of ovarian cancer in the DKO mouse model.


