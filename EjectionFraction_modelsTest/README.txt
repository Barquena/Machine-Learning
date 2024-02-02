TASK : Predict heart ejection fraction from NT-pro-bnp, Anion gap, SBP and sex

Performance measures :  Root mean square error and Mean absolute error (use only if normaly distributed) will be tested in Tree different models with cross-validation (cv=10):

linear regression(RMSE_crossVal -> 12.14±0.66%);
Decision tree (RMSE_crossVal -> 17.47±1.07%);
Random forest(RMSE_crossVal  -> 12.73±1.84%).

Random forest was retained for fine-tuning. The best fit model return a RMSE of 12.72 [max_features=2, n_estimators=1000, conf_int [11.28916955, 14.1075363 ]] where the best best predictor of ejection fraction were NT-proBNP(0.34) and systolic blood pressure (0.34)