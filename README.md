### Project Title
Machine Learning Techniques for Distinguishing Between Human and AI-Generated Text

** by Mykhaylo Chuba **

#### Executive summary
This project explores the effectiveness of machine learning techniques in distinguishing between human and AI-generated text, addressing crucial issues of authenticity, misinformation, and trust in digital content. Using a dataset from Kaggle, various classification models such as Logistic Regression, Decision Trees, KNN, and SVM were evaluated. The SVM model achieved the highest accuracy of 98.6 but required significant computational resources. Conversely, the Logistic Regression model, with a slightly lower accuracy of 98.3, was computationally efficient and produced the highest recall score of 98.6. This efficiency makes Logistic Regression the preferred choice for scalable applications, ensuring accurate identification of AI-generated text while conserving computational resources, thus supporting safer and more transparent AI deployments.


#### Rationale
In the era of information proliferation, distinguishing between human and AI-generated content is vital to address issues of authenticity, misinformation, and trust. Understanding the characteristics of AI-generated text can help make AI tools more transparent and accountable. With the increasing use of AI in generating content, it becomes crucial to ensure compliance with copyright laws, academic requirements, and regulations. By identifying AI-generated texts accurately, we can prevent the misuse of AI and contribute to safer AI deployments

#### Research Question
Can machine learning models effectively differentiate between text generated by humans and text produced by artificial intelligence?

#### Data Sources
https://www.kaggle.com/datasets/shanegerami/ai-vs-human-text/data

#### Methodology
For this natural language processing experiment, I’m using a variety of machine learning classification techniques, such as Logistic Regression, Decision trees, KNN and SVM. The analysis involves preprocessing the text, extracting features that could distinguish between human and AI texts, and selecting the best-performing model based on evaluation techniques such as accuracy score, precision, recall, F1-score, time-to-fit, etc.

#### Results
During the project, I evaluated four different natural language processing models, including Logistic Regression, Decision Trees, KNN and SVM. SVM had the highest accuracy score of 0.986 with the best parameters {'svc__C': 10, 'svc__kernel': 'rbf', 'vect__max_features': 5000}; however, it took the longest time to fit of 316 sec. Therefore, I recommend using the Logistic Regression model, which had a slightly lower accuracy score of 0.983 with best parameters {'lgr__C': 0.1, 'vect__max_features': 5000}, but it took only 1 sec to fit. For 0.3% reduction in accuracy compared to SVM, it consumes 316X less computational power. This could be particularly beneficial if we want to scale the model and fit it on a larger data set. It also produces the highest recall score of 0.986. Since maximizing for the True Positives is arguably more important in classifying human vs. AI-generated text, as it reduces the amount of misclassified human as AI, Logistic Logistic is definitely better suited for this task. 

#### Next steps
Building on the successful implementation and evaluation of machine learning models to distinguish between human and AI-generated text, the next steps for this project should focus on further refining and validating the models. Firstly, expanding the dataset to include more diverse and representative samples can help improve the model's robustness and generalizability. Additionally, exploring advanced neural network architectures, such as transformers and recurrent neural networks (RNNs), could potentially enhance model performance and accuracy. Implementing cross-validation and hyperparameter tuning on a larger scale will ensure the models are optimized for various real-world scenarios. Finally, developing an intuitive user interface for the model can facilitate its deployment and accessibility for end-users, making it a practical tool for detecting AI-generated content in various applications, from academia to content creation and beyond.

#### Outline of project

- [Link to Part 1 - Modeling](https://github.com/mishachuba/Capstone_Human_vs_AI/blob/main/Capstone_AI_vs_Human_Modeling_final.ipynb)
- [Link to Part 2 - Best Model Interpretation](https://github.com/mishachuba/Capstone_Human_vs_AI/blob/main/Capsonte_AI_vs_Human_Best_Model_Interpretation_final.ipynb)


##### Contact and Further Information

Mykhaylo Chuba

mishachuba@yahoo.com
