# 優惠券使用預測
* 應用背景：
O2O（Online to Offline）是一種利用線上活動 (網路商店、促銷通知等) 帶動實體商店消費的行銷手法。  
除了實際消費收入之外，線上所收集的用戶資訊也可被用來優化客戶體驗、個性化投放廣告等等，具有極大商機。  
然而，隨機投放的優惠券將對用戶造成無意義的干擾而影響體驗，導致品牌商譽下降。  
因此，若能透過數據分析進行個性化投放，僅發放優惠券給真正會使用的客戶將能提升用戶對商家的整體良好印象。
* 預測目標：預測用戶是否會在15天內使用相應優惠券  
* 評估指標：AUC  
* 資料集：[Midterm exam for ML 100 marathon by Cupoy](https://www.kaggle.com/c/ml100marathon-02-01/data)
* 欄位說明
![avatar](https://github.com/SFYeh/2nd-ML100Days/blob/master/Projects/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%AC/%E8%B3%87%E6%96%99%E6%AC%84%E4%BD%8D%E8%AA%AA%E6%98%8E.PNG)

* [程式碼連結](https://github.com/SFYeh/2nd-ML100Days/blob/master/Projects/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%AC/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%ACver6.ipynb)

* 分析步驟

![avatar](https://github.com/SFYeh/2nd-ML100Days/blob/master/Projects/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%AC/%E5%88%86%E6%9E%90%E6%B5%81%E7%A8%8B.PNG)

* 重要特徵
 -- 活動地點與商家距離  
 - 折扣率   
 - 當天收到的折扣券數目  
 - 折扣條件價格 (例如：滿100)  
 - 每月的第三週  
 - 滿額折扣金額 (例如：折50元)  
 - 每月的第四週  

* 分析結果 

![avatar](https://github.com/SFYeh/2nd-ML100Days/blob/master/Projects/%E5%84%AA%E6%83%A0%E5%88%B8%E4%BD%BF%E7%94%A8%E9%A0%90%E6%B8%AC/%E5%84%AA%E6%83%A0%E5%88%B8%E9%A0%90%E6%B8%AC%E7%B5%90%E6%9E%9C.PNG)


* 未來可嘗試的改善  
  * better way to fill value may be prediction
  * model choosing (why this model)
  * 雖然參數調整已經用cv了，但validation set評估的時候也可以再用一次cv看看結果
  * 額外統計分析
 
