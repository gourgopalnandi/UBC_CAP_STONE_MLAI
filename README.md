
# BH-CAP_STONE-MLAI
This project contains the Capstone project files.

# Disclaimer: Content Warning

This project involves the analysis of content from social media platforms, including tweets that may contain hate speech and offensive language. The primary goal of this project is to explore methods for identifying and understanding such harmful content, and it does not in any way endorse or promote hate speech.
The content within this project may include explicit language, discriminatory remarks, or offensive terminology. This encompasses but is not limited to slurs related to race, ethnicity, religion, gender, sexuality, or other protected characteristics. It is crucial to note that such behavior is strongly condemned. The inclusion of this data in the project is solely for the purpose of creating models that can aid in detecting and mitigating the spread of hate speech and offensive language online.
It is important to exercise caution when proceeding with this project, as the content it contains may not be suitable for all audiences due to its sensitive nature. Viewer discretion is strongly advised.
The overarching aim of this work is to combat hate speech and offensive language and contribute to the creation of online spaces that are more respectful and inclusive. Your understanding and support in this endeavor are greatly appreciated.
Overview
The primary challenge in this project is the automatic detection of hate speech on social media platforms, particularly in distinguishing it from other forms of offensive language. Conventional lexical detection methods often face difficulties in making this distinction, as they tend to label any messages containing specific terms as hate speech. This lack of precision has been a limiting factor in previous studies that employed supervised learning models.

Summary of Findings
The project's findings present the performance of various machine learning models, including Logistic Regression, Decision Tree, Random Forest, SVC, K Neighbors, and XGBoost, in combination with different vectorization techniques such as Count, Tfidf, Hashing, and Binary. The evaluation focuses on two key performance metrics: 'best_score,' expressed as a percentage, and 'fit_time,' measured in minutes.

The 'best_score' metric reflects the models' accuracy in predicting the correct outcomes, with higher percentages indicating superior accuracy. In contrast, the 'fit_time' metric represents the training time of the models, with lower values signifying faster training.

Among the models evaluated, the SVC Tfidf Vectorizer attains the highest 'best_score' at 90.64%. However, it demands a substantial training time of approximately 126.92 minutes. While it achieves the highest accuracy, its extended training duration may limit its suitability for real-time applications.

On the other hand, the Decision Tree Hashing Vectorizer achieves a slightly lower 'best_score' of 89.08% but excels in 'fit_time,' requiring only about 1.53 minutes for training. This model strikes a balance between respectable accuracy and efficient training, making it a more suitable choice for applications demanding rapid computations.

The baseline models, Naive Bayes and Logistic Regression, deliver 'best_score' values of 86.91% and 89.75%, respectively. These models exhibit reasonable accuracy while boasting remarkably short training times of approximately 0.0024 and 0.0127 minutes, respectively. Such models can be advantageous in scenarios where swift training is essential.

In summary, the optimal model selection depends on the trade-off between predictive accuracy and computational efficiency required for the specific task. If maximizing accuracy is the primary goal, the SVC Tfidf Vectorizer may be the preferred option. However, for applications where fast computation is a priority, models like the Decision Tree Hashing Vectorizer or the baseline models may be more suitable.

Additional Results:
The eXtreme Gradient Boosting model achieves an impressive 'best_score' of 91.57% with a training time of 0.915651 minutes. It exhibits high accuracy and strong precision, recall, and F1-score values.
The AdaBoost model accomplishes a 'best_score' of 90.11% with a training time of 0.380739 minutes. It also demonstrates commendable accuracy and robust precision, recall, and F1-score values.
The Random Forest model achieves a 'best_score' of 89.15% but requires a longer training time of 5.282936 minutes. Nevertheless, it delivers good accuracy and satisfactory precision, recall, and F1-score values.
These additional findings offer further insights into the performance of specific models and can aid in making an informed choice regarding model selection.

Recommendations
Based on the project's results and findings from the performance evaluation of various machine learning models and vectorization techniques, several recommendations for future exploration are suggested:

Exploration of Ensemble Methods: The results highlight the promise of ensemble methods such as eXtreme Gradient Boosting (XGBoost) and AdaBoost, which exhibit strong performance with high accuracy, precision, recall, and F1-score values. Further exploration of ensemble methods may enhance the predictive capabilities of models.

Investigation of Alternative Vectorization Techniques: While Tfidf vectorization was predominantly employed in the evaluation, it would be worthwhile to explore alternative vectorization techniques like Word2Vec, GloVe, or Doc2Vec. These techniques may capture more nuanced semantic information and potentially enhance model performance.

Evaluation of Deep Learning Models: The evaluated models primarily fall within the domain of traditional machine learning algorithms. Exploring deep learning models, such as Convolutional Neural Networks (CNNs) or Recurrent Neural Networks (RNNs), could provide deeper insights into the data and potentially unlock higher levels of accuracy in predicting outcomes.

Fine-Tuning of Hyperparameters: The project's models may further benefit from fine-tuning their hyperparameters. A systematic exploration of hyperparameter space using techniques like grid search or random search may help identify optimal parameter combinations for each model

### Directory Structure

- code
    - Exploratory_Data_Analysis.ipynb
    - Basic_Model_Exploration.ipynb
    - Advance_Model_Exploration.ipynb
    - A neural network example.ipynb
    - Selected Model - AdaBoost - Testing.ipynb
    - Selected Model.ipynb
- data
    - original_raw_data.csv
    - processed_tweet.csv
- docs
    - Final Report.pdf - Final project report.
    - CRISP-DM.txt
    - OriginalPaper.pdf - Originala paper.
- plots - This direc tory contain all the plots from the project.
- streamlit - This directory contain a streasmlit project for testing.
- README.md - This file.

### Links
There are few files in this project. Each file has a seperate purpose. 

Final Report [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/docs/Final%20Report.pdf)

Exploratory Data Analysis [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/Exploratory%20Data%20Analysis.ipynb)

Basic Model Exploration [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/Basic%20Model%20Exploration.ipynb)

Advance Model Exploration [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/Advance%20Model%20Exploration.ipynb)

A neural network example [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/A%20neural%20network%20example.ipynb)

Selected Model - AdaBoost - Testing [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/Selected%20Model%20-%20AdaBoost%20-%20Testing.ipynb)

Selected Model.ipynb [here](https://github.com/gourgopalnandi/UBC_CAP_STONE_MLAI/blob/main/code/Selected%20Model.ipynb)
