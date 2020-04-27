# 優惠券使用預測
* 目的：預測用戶是否會在規定時間內使用相應優惠券
* 應用背景：避免濫發優惠券、安擾使用者體驗而降低商譽
* 資料集：[Midterm exam for ML 100 marathon by Cupoy](https://www.kaggle.com/c/ml100marathon-02-01/data)
* Metric：AUC
* 分析步驟
  * Feature generation  
  * Outlier detection & replacement (>1.5 IR) 
  * Fill NA  
  * Feature scaling   (Min_Max)
  * Balance the data  (SMOTE)
  * Feature Selection (XGBOOST)
    * Evaluate with roc_auc_score, try to reduce influence of inbalance
    * important features：
      1. 'discount_convRate'(折扣率),
      2. 'Distance'(與店家距離), 
      3. 'received_size'(當天收到的優惠券數量),
      4. 'discount_conditionP'(需要花費多少金額才能使用優惠券),
      5. 'week_3'(當月第三週),
      6. 'discount_Price'(折扣金額),
      7. 'week_4'(當月第四週)
  * Model (Logistic regression 
   * Tune Parameters (grid search)
* 分析結果  
![avatar](https://github.com/SFYeh/2nd-ML100Days/blob/master/Projects/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%AC/%E5%84%AA%E6%83%A0%E5%88%B8%E9%A0%90%E6%B8%AC.PNG)
* 預測未來可嘗試的改善  
  * better way to fill value may be prediction
  * model choosing (why this model)
  
 ------------------------
 額外統計分析
 
