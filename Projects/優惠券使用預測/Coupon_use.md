# 優惠券使用預測
* 目的：預測用戶是否會在規定時間內使用相應優惠券
* 資料集：[Midterm exam for ML 100 marathon by Cupoy](https://www.kaggle.com/c/ml100marathon-02-01/data)
* 分析步驟
  * Feature generation  
  * Outlier detection & replacement (>1.5 IR) 
  * Fill NA  
  * Feature scaling   (Min_Max)
  * Balance the data  (SMOTE)
  * Feature Selection (XGBOOST)
    * Evaluate with roc_auc_score, try to reduce influence of inbalance
    * four important features：discount_convRate,Distance, received_size,discount_conditionP
  * Model (Logistic regression 
   * Tune Parameters (grid search)
* 分析結果  

* 未來可嘗試的改善  
  * avoid using label to fill value in trainingset, since we do not have the label in testset
  * better way to fill value may be prediction
  * model choosing (why this model)
