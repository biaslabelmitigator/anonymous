**Replicate Package** - https://drive.google.com/drive/folders/1yEyeyngSLRMc_MOjVPdAKJ08d72icADM 

It includes the code of proposed approach and synthetic datasets used to evaluate FairSMOTE and FairGenerate, enabling replication of the results.

********************************************************************************************************
<h2> Datasets</h2>

In this study, we utilized nine publicly available datasets. All datasets are provided in the Dataset folder, except Meps15 and Meps16, which are excluded due to size limitations. These two datasets can be accessed through the provided URL.

1. Adult Income dataset - http://archive.ics.uci.edu/ml/datasets/Adult
2. COMPAS - https://github.com/propublica/compas-analysis
3. German Credit - https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29
4. Bank Marketing - https://archive.ics.uci.edu/ml/datasets/bank+marketing
5. Default Credit - https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients
6. Heart - https://archive.ics.uci.edu/ml/datasets/Heart+Disease
7. MEPS15 - https://meps.ahrq.gov/mepsweb/
8. MEPS16 - https://meps.ahrq.gov/mepsweb/
9. Student - https://archive.ics.uci.edu/ml/datasets/Student+Performance

**MEPS15** - https://gitlab.liris.cnrs.fr/otouat/MEPS-HC/-/blob/main/h181.csv <br />
**MEPS16** - https://gitlab.liris.cnrs.fr/otouat/MEPS-HC/-/blob/main/h192.csv
********************************************************************************************************

<h2> Baselines </h2>

**FairGenerate: Enhancing Fairness Through Synthetic Data Generation and Two-Fold Biased Labels Removal**
FairGenerate is a pre-processing method that uses a differential evolution-based approach to generate synthetic data samples, aiming to balance the distribution of sensitive attributes and class labels in the dataset. It identifies and removes biased labels both before and after the synthetic data generation process to ensure consistency and fairness.
We use the code they provided in the code repository:  https://github.com/xyz745/FairGenerate

**Fair-Smote: Proposed in the paper: Bias in Machine Learning Software: Why? How? What to Do?**
Fair-SMOTE is a pre-processing method that uses the modified SMOTE method to balance the distribution of sensitive features and class labels in the dataset consistently. Then, biased data labels are removed through situation testing tactics.
We use the code they provided in the code repository: https://github.com/joymallyac/Fair-SMOTE

**FairMask: Proposed in the paper: FairMask: Better Fairness via Model-Based Rebalancing of Protected Attributes**
Fairway is a hybrid algorithm that combines pre-processing and post-processing methods. 
We use the code they provided in the code repository: https://github.com/anonymous12138/biasmitigation 

**LTDD: Linear Regression Based Training Data Debugging**
LTDD is a preprocessing algorithm that finds and removes the biased portion present in the features of the training data.
We use the code they provided in the code repository: https://github.com/fairnesstest/LTDD

**MirrorFair**
MirrorFair is a preprocessing method that employs an ensemble approach to address fairness issues, grounded in the principles of counterfactual inference. It creates a counterfactual dataset from the original dataset and trains two separate models, one on the original dataset and the other on the counterfactual dataset. Finally, it adaptively combines the predictions from both models to produce fairer final decisions. We use the code they provided in the code repository: https://github.com/XY-Showing/FSE2024-MirrorFair
 
