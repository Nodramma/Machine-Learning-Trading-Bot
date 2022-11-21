# Machine-Learning-Trading-Bot
Machine learning algorithms that can adapt to new data

# Tuning the Baseline Trading Algorithm

* The cumulative products of the initial strategy returns could be presented by the following chart:
![Short Window = 4, Long Window = 100, Period of Traning Data = 3 months ] (4-100_3-mont.png)

* We can observe that by the end of the period  strategy returns are ahead of actual returns by 0.1 with overall accuracy of the model 55 %.


* In the next step I adjast the size of the training dataset to 1 month. The comparison of returns is in the following chart:
 ![Short Window = 4, Long Window = 100, Period of Traning Data = 1 months ] (./1_month.png)

 * Strategy returns are ahead of actual returns on the whole stretch of the observed period with overall accuracy 55%. Although precision and recall of the sell signals dropped to 37% and 3% accordingly.   


* In the following attampet I adjast the size of the training dataset to 6 month. The comparison of returns is in the following chart:
 ![Short Window = 4, Long Window = 100, Period of Traning Data = 6 months ] (./6_months.png)

 * Strategy returns coinside with the  actual returns during first half of the period, perform worse than actual returns in the third quarter and better then actual returns in the fourth quarter of the observed period. The final cumulative result of the strategy are ahead of actual by approximatly 0.2.Overall accuracy 56%. Although the recall rate of the sell signals dropped to 2%.


* Next I adjasted the SMA input feateres to sort_window = 4, long_wondow = 200.
![Short Window = 4, Long Window = 200, Period of Traning Data = 3 months ] (./4_200.png)

* The strategy returns line on the whole stretch of the observed period shows the behaviour oposite to the one of the actual returns, dropping below the cumulative results by the end of the period by aproximately 0.6. Overall accuracy 47%,  recall improves significantly for sell signals to 85 % and drops for buy signals to 16%. Precision rate improved slightly.


* Next I adjasted the SMA input feateres to sort_window = 40, long_wondow = 200.
![Short Window = 40, Long Window = 200, Period of Traning Data = 3 months ] (./40_200.png)

* Most of the observed period strategy returns underperform actual returns. Overall accuracy 54, precision for sell and buy are 45% and 57, recall 22% and 79% accordingly.


* Next I adjasted both the SMA input feateres to sort_window = 40, long_wondow = 200 and the size of the training dataset to 6 month.
![Short Window = 40, Long Window = 200, Period of Traning Data = 6 months ] (./40-200_6-months.png)

* Strategy performs better that actual returns only on the last quarter of the period. Overall accuracy 53, precision for sell and buy are 45% and 57, recall 35% and 67% accordingly.


* As a conclusion to my limited tuning attempts of the model I could admit that the model could benefit from the extencion of the data for the training and testing as well as balancing of that data as  accuracy of the mopdel never exceeded 56 %. The best result over whole period for the strategy returns I received using size of the training data set 1 month and sort and long windows 4 and 100 accordingly. The best final result for the strategy I received using size of the training data set 6 month and sort and long windows 4 and 100 accordingly. 


# Evaluate AdaBoost Machine Learning Classifier

The cumulative products of the strategy returns while using AdaBoost Classifier could be presented by the following chart:
![Short Window = 4, Long Window = 100, Period of Traning Data = 3 months ] (./AdaBust_4-100_3-months.png)

* The AdaBoost strategy returns could be comparable with the results of the initial strategy returns. They perform very similar on the last quarter of the observed period, on the first three quarters the initial strategy behaves better. Although the final return of the Adabust model showes a grater amount. 
