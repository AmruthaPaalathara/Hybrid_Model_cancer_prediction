# Hybrid_Model_cancer_prediction

This project looks at detecting cancer by using a mix of two models: Decision Tree (DT) and Reinforcement Learning (RL). It focuses on testing how well these models work on their own and together as a hybrid to predict cancer using the dataset.

### Repository Structure
*cancerAllv3/: Contains the dataset used for training and testing the models.
*cac3/: Python scripts for training the Decision Tree, creating the RL environment, building and training the RL model, and implementing the hybrid model.
*Reinforcement_Learning_CAC3: Detailed documentation of the project, including methodology, evaluation metrics, and insights.
*cac3.html: A simple web page summarizing the project's results.
*Methodolgt_RL_CAC3.drawio: Includes visual representations of methodology (Fig. 1)

##Methodology
*Dataset Input: The dataset was divided into 70% for training and 30% for testing.
*Decision Tree Training: A DT model was trained to classify the data and predict cancer.
*Environment Creation for RL: Each row in the dataset was treated as a state, resulting in 569 states (rows).
*Reinforcement Learning: An RL model was built and trained to predict outcomes based on state transitions.
*Hybrid Model: Combined DT and RL, where RL overwrites the DT prediction if they differ.
*Evaluation: Accuracy, precision, recall, and F1-score were calculated for each model.

##Results
*Decision Tree (DT):
Accuracy: 93%
Precision: 89%
*Reinforcement Learning (RL):
Accuracy: 13%
Precision: 6%
*Hybrid Model:
Accuracy: 56%
Precision: 30%
The evaluation shows that the Decision Tree model outperforms the RL and hybrid models, making it more suitable for cancer detection.

##Key Insights:
*The RL model struggled with classification due to its inability to adapt properly to the dataset.
*The hybrid model improved over RL but fell short of the DT model's performance.
*Using the Decision Tree model alone provides the best accuracy and precision for cancer prediction in this context.
