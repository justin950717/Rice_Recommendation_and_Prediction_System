# Rice_Recommendation_and_Prediction_System
## Masters in DSBA Capstone Project


This is my Master's capstone project titled: ADOPTING MACHINE LEARNING TECHNIQUES USING IOT-BASED SENSORS TO RECOMMEND AND PREDICT RICE CULTIVATION IN MALAYSIA. This capstone project aims to develop a rice recommendation and prediction system by adopting ML techniques couple with IoT-based sensors to effectively recommend and predict rice cultivation in Malaysia. Furthermore, this project will resolve two key areas: firstly, to determine whether the use of IoT technology can substantially enhance rice yields, and secondly, to educate Malaysian rice farmers on suitable rice cultivation features while simultaneously predicting their potential rice yields using ML. The ML models employed for this project will also be based on supervised classification and regression tree-based models for recommending rice cultivation suitability based on specific land and environmental attributes, as well as to predict its potential yields. Hence, from the findings of this capstone project, the optimal ML models for implementing in Malaysia’s rice domain are the Random Forest classifier and regressor models, which will serve as the engine for the rice recommendation and prediction system that will propel Malaysia’s rice farming practices to new heights.



**Problem Statement**
1. Malaysia rice industry still lacks behind in terms of agricultural technology.
2. Malaysian rice farmers are still unaware of the ideal key features needed for effective rice cultivation.
3. Malaysia's weather patterns can fluctuate drastically between monsoon and off-monsoon seasons, resulting in varying environmental and soil conditions.
   


**Aim**

To develop a rice recommendation and prediction system by adopting ML techniques based on IoT data for effective rice cultivation in Malaysia.



**Objectives**
1.	To investigate the use of IoT technology in the improvement of crop yield. 
2.	To determine the relevant key features for rice cultivation, in terms of ML predictors. 
3.	To examine and compare different ML techniques done by previous research within the same domain. 
4.	To implement supervised ML classification and regression techniques for recommending rice cultivation suitability and predicting rice potential yields.
5.	To evaluate the supervised classification and regression ML models’ performances using appropriate evaluation metrics and select the optimal ML models to be deployed.
6.	To deploy the optimal ML models into the rice recommendation and prediction system.



**Scope**
1. To collect rice cultivation datasets either in the Malaysian context or similar region. 
2. To do extensive literature review on:
   - The use of IoT technology in the improvement of crop yield.
   - Relevant key features for rice cultivation.
   - ML models and results done by previous researchers within the same domain.
3. To build and train ML models for recommending rice cultivation suitability as well as predicting rice potential yield.
4. To evaluate each model’s performances in carrying out its specific task. 
5. To  deploy the identified optimal models as a comprehensive rice recommendation and prediction system.



**Methodology**

The overall project design focuses on conducting quantitative experiments with empirical evaluations, as the data collected primarily consists of quantitative data that will undergo predictive analysis using statistical ML algorithms to model the predictions. This will be done through the following diagrammatic flowchart, outlining the specific objectives achieved at each stage.
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/9cc4a22d-74d3-4688-991e-bd6a11b4374f)



**Model Implementation**

Each of the respective hyperparameter values were set to the default minimum provided by Python's "scikit-learn" module

*Note: the baseline tree-based classifiers turned out to perform exceptionally well with almost 100% accuracies. Hence, no further hyperparameter tuning was conducted on it. Only tree-based regressors were subjected to hyperparameter tuning*

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/ac3f3dec-bc34-4c6b-b43c-1e7962e3a661)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/097b5416-02f3-4a16-876c-7e28a0047aee)



**Model Performances**
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/344c885f-5826-4734-9097-9b729b39d0a3)
- All the classifier models performed exceptionally well, with accuracy and AUC scores of more than 99% and 0.995 respectively -> indidicating excellent discriminatory power in distinguishing rice and non-rice instances.
- The DT classifier model however, was observed to slightly underperformed in comparison with its peers. As for the RF and GBT classifier models, both were found to have identical performance rates in terms of their accuracy, precision, recall and AUC scores. This suggest that both models were equally effective in classifying between the positive (rice) and negative (non-rice) instances.
- That being said, based on the variable importance results generated, the RF classifier model's variable importance score align more closely with the actual rice cultivation scenario, as it demonstrated a more well-represented variable importance amongst all input variables
- As such, it will be selected as the optimal model candidate to be deployed for recommending rice cultivation suitability in the system.
- Another thing to note is that for all 3 models, the Rainfall variable is seen to have the highest influence on the prediction, followed by Nitrogen nutrient content and humidity. This pattern made sense in the expect of cultivating rice, as rice is very heavily dependent on high amounts of rainfall and humidity for a successful growth.
- Moreover, previous research has indicated that Nitrogen is the primary nutrient content for rice cultivation among NPK, and its ratio is typically used at least two times more than that of Phosphorus and Potassium.



![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/736a7390-8f0d-4cc3-8c7e-bd53b2de6525)
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/4a3fbfc3-7bbd-4222-a6f5-a61cdbf83129)
- The best performing regression model = GBT.
- However, as it was found to be underfitted it will not be selected as the optimal model candidate.
- Instead, the RF regressor will be selected as the optimal model candidate to be deployed for predicting rice yields in the system, as it performed the 2nd best with the least model fitness.
- The tuned GBT regressor model managed to achieve a RMSE, MAPE, and R2 value of 2998.27, 5.91% and 0.885 respectively. 
- In other words, the model was predicting the rice yield with a ±2998.27 hg/ha deviation, resulting in an average error rate of 5.91%. 
- At the same time, the model’s input variables explained nearly 90% of the variance in rice yield prediction.



**GUI system Results**

Rice Recommendation Section of System
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/e716b171-d042-44f9-9464-89a0970e535e)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/1d876bdd-b162-4047-b3bd-e379b0ffaec6)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/bbc7bdc4-b39a-4039-aaa4-112c38461710)


Rice Prediction Section of System
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/62f71c70-172f-4ce5-8b90-e15a69bbc35f)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/49c76814-4c1a-4eaf-83ab-2597a2c1f252)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/c930e43a-d2eb-400d-b815-849d9828699e)



**Conclusion**

*Summary of findings:*

- Optimal ML models to be adopted in Malaysia’s rice farming sector = RF classifier and regressor models. Both models will be deployed in a GUI application that served as the engine for the rice recommendation and prediction system. 

- The variable importance of the RF classifier reveals that the most crucial feature (variable) for successful rice cultivation is the volume of rainfall, followed by the Nitrogen nutrient content and humidity, as rice crops thrive in ample amounts of irrigation with high concentrations of Nitrogen nutrient contents. 

- The variable importance of the GBT regressor reveals that the most influential feature for predicting rice yield is the area of the planted rice fields, since a larger planted land area ultimately leads to a greater yield production.

- The tree-based classifier models performed exceptionally well due to the ease of modelling its training data. The accuracies of the tree-based classifiers even outperformed other classifier models used by previous research cited in the literature review. 



*Significance & Contribution:*

- The development of the rice recommendation and prediction system will revolutionize Malaysia's rice farming practices, by equipping Malaysian rice farmers with the ability to accurately predict whether rice can be cultivated in their fields and forecast its potential yields. 

- This project aligns with the Malaysia’s government plan to upscale its rice cultivation domain, as current challenges caused by climate change, population growth and insufficient rice productions, have given rise to the need to innovate Malaysia’s agricultural technologies with the aid of IoT and ML.

- The contributions of this project will not only ease and educate rice cultivation among local farmers but will also potentially lead to increased yields and profits. With such benefits, the hope is to encourage more Malaysians to uptake rice farming and reduce the nation's reliance on rice imports for the sake of food security.



***Note: Below is repository legend for easier naviagation***

Repository Legend:
1.  Datasets -> folder consisting of all datsets utilized in this project (including a dataset readme file)
2.  Project -> Capstone project python codes




