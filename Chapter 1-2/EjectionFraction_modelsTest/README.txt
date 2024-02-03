TASK : Predict heart ejection fraction from NT-pro-bnp, Anion gap, SBP, and sex on 1178 roww

Performance measures :  Root mean square error and Mean absolute error (use only if normaly distributed) will be tested in three different models with cross-validation (cv=10):

Linear regression(  RMSE_crossVal -> 12.14 ± 0.66%);
Decision tree (     RMSE_crossVal -> 17.47 ± 1.07%);
Random forest(      RMSE_crossVal -> 12.73 ± 0.84%).

Random forest was retained for fine-tunning. The best fit model return a RMSE of 12.72 [max_features=2, n_estimators=1000, conf_int [11.29, 14.11 ]] where the best predictor of ejection fraction were NT-proBNP(0.34) and systolic blood pressure (0.34)
