TASK : Predict heart ejection fraction this time with a clean data set containing mostly blood markers (38 columns/ 428 rows)
Performance measures :  Root mean square error and Mean absolute error (use only if normaly distributed) will be tested in three different models with cross-validation (cv=10):

linear regression(  RMSE_crossVal -> 12.78 ± 1.52%);
Decision tree (     RMSE_crossVal -> 16.47 ± 1.57%);
Random forest(      RMSE_crossVal -> 12.32 ± 1.29%).

Random forest was retained for fine-tunning. The best fit model return a RMSE of 12.72 [max_features=21, n_estimators=500, conf_int [10.40, 14.08]] where the best predictor of ejection fraction were :
 (0.0773) 'Diastolic blood pressure',
 (0.0659) 'Creatine kinase',
 (0.0542) 'Creatinine',
 (0.0494) 'PCO2',
 (0.0462) 'Respiratory rate',
 (0.0453) 'Blood calcium',
 (0.0311) 'SPO2),
 (0.0292) 'Urine output',
 (0.0286) 'Anion gap',
 (0.0284) 'MCV',
 (0.0282) 'temperature',
 (0.0257) 'Leucocyte',
 (0.0244) 'BMI',
 (0.0242) 'EF',
 (0.0242) 'Chloride',
 (0.0228) 'Magnesium ion',
 (0.0224) 'Blood potassium',
 (0.0220) 'MCHC',
 (0.0216) 'MCH',
 (0.0215) 'Platelets',
 (0.0214) 'NT-proBNP'.
