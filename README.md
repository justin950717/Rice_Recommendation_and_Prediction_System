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
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/4894aa1e-989e-4827-b761-fb8ac7a8c5bb)


**Model Implementation**

Each of the respective hyperparameter values were set to the default minimum provided by Python's "scikit-learn" module

*Note: the baseline tree-based classifiers turned out to perform exceptionally well with almost 100% accuracies. Hence, no further hyperparameter tuning was conducted on it. Only tree-based regressors were subjected to hyperparameter tuning*

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/ac3f3dec-bc34-4c6b-b43c-1e7962e3a661)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/097b5416-02f3-4a16-876c-7e28a0047aee)


**Model Performances**
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/344c885f-5826-4734-9097-9b729b39d0a3)


![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/09a7bd0a-c1ad-4c91-9c84-517749e63a8c)
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/e69b69b3-ea51-4991-8433-7c558d6f950b)

**GUI system Results**
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/e716b171-d042-44f9-9464-89a0970e535e)
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/1d876bdd-b162-4047-b3bd-e379b0ffaec6)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/bbc7bdc4-b39a-4039-aaa4-112c38461710)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/e3e41a76-c65c-44f5-af07-526dc652cc9c)
![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/37673b3d-1a65-4d60-96bf-89ba7a799cd6)

![image](https://github.com/justin950717/Rice_Recommendation_and_Prediction_System/assets/95216403/0ecfdad2-7e35-4e6e-958d-4559f2943f8a)


**Conclusion**

*Summary of findings*

-Optimal ML models to be adopted in Malaysia’s rice farming sector = RF classifier and regressor models. Both models will be deployed in a GUI application that served as the engine for the rice recommendation and prediction system. 

-The variable importance of the RF classifier reveals that the most crucial feature (variable) for successful rice cultivation is the volume of rainfall, followed by the Nitrogen nutrient content and humidity, as rice crops thrive in ample amounts of irrigation with high concentrations of Nitrogen nutrient contents. 

-The variable importance of the GBT regressor reveals that the most influential feature for predicting rice yield is the area of the planted rice fields, since a larger planted land area ultimately leads to a greater yield production.

-The tree-based classifier models performed exceptionally well due to the ease of modelling its training data. The accuracies of the tree-based classifiers even outperformed other classifier models used by previous research cited in the literature review. 


*Significance & Contribution*

-The development of the rice recommendation and prediction system will revolutionize Malaysia's rice farming practices, by equipping Malaysian rice farmers with the ability to accurately predict whether rice can be cultivated in their fields and forecast its potential yields. 

-This project aligns with the Malaysia’s government plan to upscale its rice cultivation domain, as current challenges caused by climate change, population growth and insufficient rice productions, have given rise to the need to innovate Malaysia’s agricultural technologies with the aid of IoT and ML.

-The contributions of this project will not only ease and educate rice cultivation among local farmers but will also potentially lead to increased yields and profits. With such benefits, the hope is to encourage more Malaysians to uptake rice farming and reduce the nation's reliance on rice imports for the sake of food security.


***Note: Below is repository legend for easier naviagation***

Repository Legend:
1.  Datasets -> folder consisting of all datsets utilized in this project (including a dataset readme file)
2.  Project -> Capstone project python codes




