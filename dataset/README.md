# Dataset setup

Download the **EuroSAT RGB** dataset from the [official repository](https://github.com/phelber/EuroSAT) or use [the Kaggle mirror](https://www.kaggle.com/datasets/apollo2506/eurosat-dataset).

This repository does not redistribute image files. The baseline notebook currently expects the Kaggle RGB path:

`/kaggle/input/datasets/apollo2506/eurosat-dataset/EuroSAT`

The RGB directory should contain `AnnualCrop/`, `Forest/`, `Residential/`, and `River/` folders, among others. For local runs, change the notebook's `DATASET_PATH` to your downloaded EuroSAT RGB directory and change the two `/kaggle/working/` save paths to `results/` (create it if necessary). Run from the repository root so the relative output paths work.
