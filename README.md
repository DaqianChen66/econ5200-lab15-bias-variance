# econ5200-lab15-bias-variance
# Bias, Variance and an Unbiased Cross-Validation Score

## Objective

I studied how model selection affects prediction error and how nested cross-validation provides a more reliable evaluation.

## Methodology

- Compared polynomial models of degrees 1 to 12 using 5-fold cross-validation on 80 simulated observations.
- Evaluated the selected model on 20,000 new observations.
- Used nested cross-validation to assess model selection.
- Examined the bias-variance tradeoff through simulation.
- Built and tested a reusable k-fold cross-validation function.

## Key Findings

- Degree 5 had the lowest CV error of 0.1853.
- Its true prediction error was 0.2330, showing that the selected CV score was optimistic.
- Nested CV estimated an error of 0.1910.
- The irreducible noise level was 0.2025.
- My function produced a 10-fold CV error of 0.1921 for degree 5.

These results show why model selection and model evaluation should be separated.
