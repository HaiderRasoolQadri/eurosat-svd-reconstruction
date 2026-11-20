# Feasibility Checkpoint

**Title:** Rank-Based Reconstruction Analysis of EuroSAT Satellite Images Using SVD  
**Team:** Haider Rasool Qadri (24I-8023), Section MS(DS)  
**Code link:** **https://github.com/HaiderRasoolQadri/eurosat-svd-reconstruction**

**Initial results:** Using EuroSAT RGB, we selected 800 images (200 each from AnnualCrop, Forest, Residential and River) and used an 80/20 stratified train/test split (640/160). PCA with randomized SVD at rank k=20 gave an MSE of **0.003889**, mean relative reconstruction error of **0.132051**, and cumulative training explained variance of **84.95%**. The recorded baseline run took **1.54 seconds**.

**Resources and obstacles:** The implementation used Python, NumPy and scikit-learn on CPU. The subset ran successfully; the notebook's paths were originally configured for Kaggle. The memory/runtime of the planned 9,000-image experiment has not yet been measured. On a laptop, the dataset and output paths must be changed.

**Next step:** Increase the sample toward 9,000 images, compare ranks k = 5, 10, 20, 40, 80 and 120, and evaluate reconstruction error across the four categories. Repeat with fixed seeds if feasible, reducing sample size or maximum rank if CPU/memory requirements are too high.
