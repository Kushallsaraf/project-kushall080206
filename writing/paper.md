
## Name

Kushall Saraf

---


### Introduction


In the realm of cutting-edge technology, machine learning (ML) has emerged as a transformative force, revolutionizing various fields with its predictive capabilities and data-driven insights. From healthcare to finance, ML has made significant contributions, enabling more informed decision-making and unlocking new possibilities. One domain where ML's potential has garnered immense interest is sports outcome prediction. By leveraging vast amounts of historical data, sophisticated algorithms, and pattern recognition, ML offers the promise of enhancing our understanding of sports events and ultimately predicting their outcomes with unprecedented accuracy.

Sports, as a multi-billion-dollar industry, has not remained immune to the transformative potential of ML. The vast and ever-growing amount of data generated from sporting events, including player statistics, match results, weather conditions, and more, has become a goldmine for data scientists and sports enthusiasts alike. The application of ML in sports has not only opened new avenues for fan engagement but has also presented opportunities to gain a competitive edge for athletes, coaches, and sports organizations. These teams spend millions of dollars on algorithms used for match outcome prediction, tactical decision-making, player investments, fantasy sports, and injury prediction.[1] The picture below shows the many applications of AI and ML in sports. 

<img width="795" alt="Screenshot 2023-07-30 at 7 03 51 PM" src="https://github.com/LS102-summer2023/project-kushall080206/assets/137182677/28d8a8d0-6ebb-4dcb-9b91-c982de30a476"> [2]

At the forefront of ML applications in sports lies the captivating field of sports outcome prediction. The ability to accurately forecast the results of sporting events has fascinated researchers, data scientists, and sports analysts alike. The implications of successful outcome predictions are multifaceted – from optimizing betting strategies to providing valuable insights for fantasy sports players, and even aiding coaches in devising winning tactics based on an opponent's weaknesses. The below graph shows the trend of ML in sports betting.

![68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3530366139356262633461613034393161393531633134312f742f3531613535643937653462303066343432383936376536342f313336393739313839363532362f73706f7274732d363230783334392e6a7067](https://github.com/LS102-summer2023/project-kushall080206/assets/137182677/4f869c35-714f-4166-a61d-4c18d392d71c) [8]


In conclusion, the integration of machine learning in sports outcome prediction is a fascinating and dynamic field, holding immense promise for sports enthusiasts, industry stakeholders, and the wider public alike. By harnessing the power of data and advanced algorithms, we endeavour to shed light on the exciting possibilities and potential pitfalls of using ML to predict the unpredictable –outcome of sports events.


#### Research Question

How does the accuracy of Logistic Regression compare to Support Vector Machine (SVM) when used for sports outcome prediction?

#### Motivation

The significance of data-driven decision-making in the field of sports analytics is what inspired this inquiry. Football, being one of the most popular and passionately followed sports worldwide, presents a compelling arena for predictive modelling. The outcomes of football matches are influenced by a myriad of factors, ranging from team composition and player performance to weather conditions and tactical strategies. By comparing the predictive accuracy of Logistic Regression and SVM in this context, valuable insights can be gained to optimize sports outcome prediction models. Understanding which algorithm performs better in forecasting football match results can not only help sports managers and enthusiasts in making informed betting decisions but also provide teams and coaches with valuable pre-match insights to devise winning strategies. 


#### Current State of the Art

The current state of the art in sports outcome prediction using machine learning techniques in football has witnessed significant advancements. Algorithms like ANN, Nearest Neighbors Regression, XGBoost, Random Forest Regression and the ones targeted in this study are majorly used in sports outcome prediction. Algorithms have been widely employed in sports analytics, leveraging historical match data, player statistics, and contextual information to forecast game results. Logistic Regression, a linear classification method, excels in situations where the decision boundary is relatively simple and easy to interpret. On the other hand, SVM, a powerful and versatile algorithm, is adept at handling complex, high-dimensional datasets, enabling it to capture intricate patterns in football data. Many Studies have explored the impact of feature selection techniques and data preprocessing methods on the predictive performance of ML models. However, challenges remain, such as dealing with imbalanced classes and selecting an appropriate kernel for SVM to optimize performance. As the field continues to evolve, researchers aim to fine-tune these algorithms, incorporating advancements in deep learning and ensemble techniques, to achieve more accurate and reliable football outcome predictions. The ultimate goal is to develop models that can enhance decision-making for sports enthusiasts, analysts, and football teams, paving the way for more data-informed strategies and informed sports predictions.


#### Goals of the Project

In this literature review, I delve into the intriguing world of using machine learning for sports outcome prediction. The aim is to explore the various methodologies and algorithms that have been employed to predict the results of sporting events. By analyzing historical data, team compositions, player performance metrics, and various contextual factors, ML models have sought to decode the intricate patterns that influence the outcome of games.

Through this research, I seek to gain a comprehensive understanding of the strengths and limitations of existing ML approaches in sports outcome prediction. Additionally, I aim to identify potential areas of improvement that could further enhance the accuracy of predictions. Furthermore, I will examine how ML-powered predictions are being utilized in real-world scenarios, such as sports betting markets and sports analytics firms, and the impact these predictions have on decision-making processes.



### Related work

[3], developed a logistic regression model to predict match results of Barclay’s premier league. What stands out is that they gathered the significant variables from various research papers rather than just making their own assumptions. They also gathered data from video games like FIFA which they said improved the quality of the data. They used variables like Home Offense,  Home Defence,  Away Offense, and Away Defence. They got a prediction accuracy of 69.5% from their model. They determined that the most significant variables were home Defence and away Defence. 

[4], used the XGBoost algorithm to predict the results using limited data. They proposed a system which uses XGBoost as their primary algorithm for sports outcome prediction. It is compared with other algorithms using a filtered dataset to find the most influential data. Optimization or normalization has been applied, and the predicted outputs will represent win, draw, or loss in human-readable form. They came to the conclusion that XGBoost could outperform many other algorithms.  

[5], set out to predict the results of the Greek league, considered the most predictable league, using 5 machine learning models. These models were as follows: k-Nearest Neighbour (k-NN), LogitBoost (LB), Support Vector Machine (SVM), Random Forest (RF) and CatBoost (CB). They engineered new features from the already existing ones. The following were created: Home Team form (the Home Team’s form according to the last five matches performance of the team), Away Team form, Home Team league points (the points the Home Team has gained in the league for the corresponding season before the match is played), Away Team league points, Home Team previous match goals (the goals scored by the Home Team in the previous match played), Away Team previous match goals, Home Team previous half time match goals (the goals scored by the Home Team in the previous match until half time) and Away Team previous half time match goals. As far as SVM is concerned they concluded they used a few parameters which resulted in an accuracy of 54.07% and the metric results were 0.4258, 0.4414 and 0.3876 for recall, precision and F1-score respectively. According to Table 3 in their paper, SVM had the least accuracy and F1-score. They also used LogitBoost which performs an additive logistic regression. It had an accuracy of 55.65% and an F1-score of 0.4962 ranking 3rd among the five models. The best-performing model was CatBoost with an accuracy of 67.73% which they applied to two more datasets. They concluded that the two most important features were Home Team Form and Away Team Form. Applying the best model to other datasets, they reached the conclusion that each league has its own properties and particularities that need to be considered separately for an accurate prediction. 

[6], modelled an algorithm using Logistic Regression, SVM and XGBoost to compare their accuracy. He used a dataset from the English Premier League. The web scraping was done and datasets from 2000 to 2015 were used. The data was split into training and testing which was then applied to 3 different classifiers and 12 features were considered. After refining the data, the model was run and the F1-score was calculated on the test data. Logistic Regression had a score of 0.6957, SVM had a score of 0.6818 and XGBoost had the highest accuracy with an F1-score of 0.7451. He further ran some tuning parameters which inflated the score to 0.7826. He concluded that adding sentiment from Twitter, and some news articles can improve the accuracy. Also including more features from various data sources could enhance the accuracy of the predictions.

[7], set out to predict the outcome of the NFL (an American football league). He used Logistic Regression and SVM models to execute the project. Scores and statistics from 2003, 2004 and 2005 were used as datasets for the models. For the first algorithm, he used his own implementation of logistic regression in Matlab, which used the Newton-Raphson method. For the second one, he used SVM-light with linear, polynomial and tangent kernels. As for the conclusion the best results were achieved by the Logistic Regression model. The results were as follows – 2005: 65.83% - 2004: 61.37% - 2003: 67.08%. They determined that using the best features with different algorithms can improve the accuracy of the predictions. 


### Prototype

TODO: This section describes the implemented prototype - how did you implement your prototype, including the overall design of your prototype, details of the algorithms and tools if any used, etc. Use technical diagrams, equations, algorithms, and paragraphs of text to describe the research that you have completed. Be sure to number all figures and tables and to explicitly refer to them in your text.

### Experiments

TODO: This section describes your experimental set up and evaluation. It should also produce and describe the results of your study. The subsection titles below offer a typical structure used for this section.

#### Experimental Design

TODO: Especially as it pertains to responsible computing, if conducting experiments or evaluations that involve particular ethical considerations, detail those issues here.

#### Evaluation

TODO

#### Threats to Validity

TODO: What are some considerations and choices you have made during your project that might compromise some of your presented results (for example, if you are using data could there be sources of data inaccuracy, or if you are relying on an existing tool or library, a potential inaccuracy in their work might result to inaccuracy in yours).

### Conclusion

TODO: Traditionally, this section addresses the areas proposed below as subsections, although not necessarily in this order or organized as offered.

#### Summary of Results

| Ref | Research Title | Dataset | Techniques Applied | Prediction Accuracy |
| --- | -------------- | ------- | ------------------ | ------------------- |
| [3] | Predicting Football Match Results with Logistic Regression | Barclay’s Premier League | Logistic Regression | 69.5% |
| [4] | Football Prediction using XGBoost Algorithm: A Literature Review | NA | XGBoost | NA |
| [5] | Predicting Soccer Outcomes in the Greek League Using Machine Learning | Greek League | k-Nearest Neighbour (k-NN), LogitBoost (LB), Support Vector Machine (SVM), Random Forest (RF) and CatBoost (CB) | SVM – 54.07%, CB – 56.59%, LB – 55.65%, RF – 56.38%, k-NN 50.13% |
| [6] | Predicting Winning Teams | English Premier League | Logistic Regression, SVM, XGBoost | LR – 0.6957, SVM – 0.6818, XG – 0.7451 |
| [7] | Predicting the outcome of NFL games using machine learning | Logistic Regression and SVM | NFL (2003 - 2005) | 2005: 65.83% - 2004: 61.37% - 2003: 67.08% |





#### Future Work

TODO

#### Ethical Implications and Recommendations

1. **Transparency and Explainability:** Models developed using machine learning can be very complicated and challenging to understand. Certain models' lack of transparency and may give rise to questions regarding responsibility and the capacity to comprehend the elements influencing forecasts. In order to ensure impartial decision-making, stakeholders, athletes, coaches, and fans, may have a right to know how forecasts are generated.
   
2. **Privacy and Data Protection:** Collecting and analyzing large datasets for sports prediction can involve personal and sensitive information about athletes, team members, or fans. Ensuring proper consent is crucial to protect individuals' privacy and compliance with data protection laws.
   
3. **Fairness and Bias:** Machine learning models trained on historical data can inherit biases present in the data, leading to biased predictions. This may perpetuate existing inequalities in sports, such as favouring well-established teams or players. Ensuring fairness in predictions requires careful consideration of data representation and addressing bias issues.

4. **Integrity of the Sport:** Predicting sports outcomes might lead to potential manipulation attempts by malicious actors seeking to exploit the predictions for personal gain. Maintaining the integrity of the sport is paramount, and measures must be in place to prevent any misuse of models.

5. **Emotional Impact on Fans and Players:** Accurate predictions may heighten the emotional impact on fans and players, potentially leading to increased pressure and stress. Negative effects on mental health and well-being should be taken into account.

6. **Effects on Competitive Balance:** Wide adoption of predictive models in sports decision-making might impact competitive balance. Smaller or less wealthy teams may struggle to compete with larger, more resourceful teams that have better access to sophisticated predictive technologies.

7. **Regulatory Compliance:** Researchers and organizations must adhere to relevant regulations and guidelines regarding the use of ML models in sports prediction, including data protection laws, anti-match-fixing regulations, and responsible gambling practices.

Addressing these ethical implications requires a collaborative effort involving researchers, sports organizations, policymakers, and other stakeholders to develop guidelines, best practices, and policies that ensure the responsible and ethical use of ML in sports outcome prediction.




#### Conclusions

TODO

#### References


[1]  R. Beal, T. J. Norman and S. D. Ramchurn, "Artificial intelligence for team sports: a survey," The Knowledge Engineering Review, vol. 34, 2019. Available: https://www.proquest.com/scholarly-journals/artificial-intelligence-team-sports-survey/docview/2328571462/se-2. DOI: https://doi.org/10.1017/S0269888919000225.

[2]  A. D. Stefano, “Ai in sports: Trends, applications and future challenges,” AI in Sports: Trends, Applications and Future Challenges, https://www.itransition.com/blog/ai-in-sports (accessed Jul. 30, 2023). 

[3]  D. Prasetio and D. Harlili, ‘Predicting football match results with logistic regression’, in 2016 International Conference On Advanced Informatics: Concepts, Theory And Application (ICAICTA), 2016, pp. 1–5.

[4]  W. Gourh, K. N. Poojary, M. Vengarai, and N. Parkar, ‘Football Prediction using XGBoost Algorithm: A Literature Review’, 2020.

[5]  Marios-Christos Malamatinos, E. Vrochidou and G. A. Papakostas, "On Predicting Soccer Outcomes in the Greek League Using Machine Learning," Computers, vol. 11, (9), pp. 133, 2022. Available: https://www.proquest.com/scholarly-journals/on-predicting-soccer-outcomes-greek-league-using/docview/2716507650/se-2. DOI: https://doi.org/10.3390/computers11090133.

[6]  R. Tuwani, “Predicting_Winning_Teams,” GitHub, https://github.com/llSourcell/Predicting_Winning_Teams/blob/master/Prediction.ipynb (accessed Aug. 1, 2023). 

[7]  B. Hamadani , “1. Introduction - Stanford University,” Predicting the outcome of NFL games using machine learning, http://cs229.stanford.edu/proj2006/BabakHamadani-PredictingNFLGames.pdf (accessed Aug. 1, 2023). 

[8]  B. M. LYNCH, Sports Betting to Grow at Double-Digit Rates over the next Five Years. AUSTRALIAN RACING FACTBOOK. 
