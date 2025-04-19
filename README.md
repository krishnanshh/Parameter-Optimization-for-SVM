# Parameter Optimization for SVM

---

## Methodology

We selected a multi-class dataset from the UCI repository with a size of approximately 13,000 rows. The dataset was split using a stratified 70-30 train-test ratio across 10 different random samples to ensure consistent class distribution.

For each sample, we ran 100 iterations of hyperparameter search to optimize the Support Vector Machine (SVM) classifier. The parameters tuned included:

- **Kernel**: linear, poly, rbf, sigmoid
- **C**: Regularization parameter
- **Gamma**: Kernel coefficient
- **Degree**: Only used in the 'poly' kernel

The optimization loop retained the best accuracy along with the corresponding hyperparameters. We also logged the accuracy for each iteration to visualize convergence.

## Results Table

Below is the comparative performance of Optimized-SVM for 10 samples.


## Convergence Graph for Best Sample

The following graph shows how the accuracy evolved over the iterations for the best performing sample (Sample 6).

![](convergence_graph.png)


