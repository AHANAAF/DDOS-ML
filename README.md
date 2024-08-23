# DDoS Detection using Machine Learning

Denial of Service (DDoS) attacks poses a significant threat to network security. These attacks often originate from virtual machines in the cloud, rather than the attacker's own machine, to maintain anonymity and utilize higher network bandwidth.

Past research has primarily focused on analyzing traffic at the destination (victim's) side with predefined thresholds. However, these approaches come with notable disadvantages:
- They are solely passive defenses post-attack and cannot utilize outbound statistical attack features.
- Tracing back to the attacker is challenging using these methods.

Numerous DDoS detection techniques exist, but they often fall short in effectively mitigating these attacks. Thus, in this project, we implemented eight distinct Machine Learning (ML) techniques to detect DDoS attacks from the source side within a cloud infrastructure.

## Project Details

- **Data Source**: We trained our models using the NSDL Dataset and implemented eight different ML models for DDoS detection.
- **Data Split**: We partitioned our gathered data into training and testing samples.
- **Tool Usage**: Jupyter Notebook was the primary tool for training and testing our machine learning models.
- **Evaluation**: We assessed both supervised and unsupervised learning algorithms, including:
  - Linear Regression (LR)
  - Support Vector Machine (SVM) with linear, RBF (Radial Basis Function), and polynomial kernels
  - Decision Tree
  - Naive Bayes
  - Random Forest
  - Unsupervised learning algorithm: k-means

## Evaluation Metrics

- **Accuracy**: This metric represents the fraction of correctly classified samples and is a common way to evaluate a model's performance.
  
  `Accuracy = (TP + TN) / (TP + TN + FP + FN)`

- **Recall**: Also known as sensitivity, recall measures the true positive rate (TPR), indicating the proportion of actual positive values correctly identified.
  
  `Recall = TP / (TP + FN)`

- **Precision**: Precision, or positive predictive value, measures the consistency of repeated measurements under unchanged conditions.
  
  `Precision = TP / (TP + FP)`

- **F1 Score**: The F1 score, a harmonic average of recall and precision, is valuable when recall and precision conflict.
  
  `F1 Score = 2 * (Recall * Precision) / (Recall + Precision)`

