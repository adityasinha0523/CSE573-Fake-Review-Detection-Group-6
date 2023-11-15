# CSE573-Fake Review Detection Group 6
CSE573 Fake Review Detection

# Contributors
<ol>
<li>Aditya Sinha</li>
<li>Praveenaa Kulandhaivel</li>
<li>Arjun Ramesh</li>
<li>Haritha Athinaryanan</li>
<li>Lakshmi Narayana Rao Boyapati</li>
<li>Junaita Davakumar</li>
</ol>


# Dataset

The generated fake reviews dataset, containing 20k fake reviews and 20k real product reviews. OR = Original reviews (presumably human created and authentic); CG = Computer-generated fake reviews.
More about the dataset:
https://osf.io/tyue9/

# Folder Structure
In this specific folder structure, each of the three folders - 'code', 'data', and 'evaluations' - has a distinct and crucial role in organizing the components of the project. The 'code' folder is designated for all Python files, encompassing the entire programming aspect of the project. This include Python scripts for data processing, analysis, model training, and any other computational tasks. 

The 'data' folder is exclusively used for storing the Amazon dataset. This dedicated space for the dataset ensures easy accessibility and management, particularly important for large datasets or when multiple datasets are involved.

Lastly, the 'evaluation' folder is critical for housing the evaluations of the results. This could include performance metrics, comparative analyses, visualizations, or detailed reports that assess the effectiveness, accuracy, and other aspects of the outputs generated by the Python scripts. By storing these evaluations separately, the structure allows for a clear distinction between the raw data, the processing code, and the analysis of the outcomes, thereby maintaining a high degree of organization and clarity in the project. 
# Ensemble Learning
## Bagging with Random Forest
| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |

## Boosting with ADA Boost
| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |

## Boosting with XGBoost
| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |

# Classification Algorithms

Utilized different classification Algorithms


## SVM
Support Vector Machine (SVM) is a powerful and versatile supervised machine learning model, particularly renowned for its effectiveness in classification tasks. At its core, SVM seeks to find the optimal hyperplane that best separates different classes in the feature space. The beauty of SVM lies in its ability to handle both linear and non-linear data. In linear classification, it focuses on maximizing the margin between data points of different classes, with the points closest to the hyperplane (support vectors) being crucial in defining the separation. For non-linear classification, SVM employs a technique called the kernel trick, which transforms the data into a higher-dimensional space where a linear separator is possible. This makes SVM highly adaptable to various datasets. SVM models are known for their robustness, especially in cases where the number of features exceeds the number of samples. They are widely used in applications ranging from image classification to bioinformatics, due to their ability to handle complex and high-dimensional data efficiently.

### TF-IDF

| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |




## Multinominal Naive Bayes
The Multinomial Naive Bayes model is a popular variant of the Naive Bayes algorithm, tailored specifically for text classification tasks, particularly in scenarios where the features (typically words) are represented as frequency counts. This model operates under the core principle of Naive Bayes, which is the assumption of independence among features. In the context of text, it means that the presence or frequency of certain words in a document is independent of the presence of other words. This simplifying assumption, while often unrealistic in real-world language, enables the model to perform surprisingly well in practice, particularly in tasks like spam detection, sentiment analysis, and topic categorization. The "multinomial" aspect refers to the statistical distribution that the model assumes for the data - it treats features as arising from a multinomial distribution, which is suitable for data that can be turned into counts, such as word counts in text. Despite its simplicity and the strong independence assumption, Multinomial Naive Bayes is known for its efficiency, ease of implementation, and particularly good performance with high-dimensional data, such as large text corpora.

### TF-IDF

| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |



## Logistic Regression
Logistic Regression is a widely used statistical method for binary classification problems, where the goal is to predict a binary outcome (such as yes/no, win/lose, 0/1). Despite its name, it's a linear model for classification rather than regression. At its core, Logistic Regression models the probability that a given input belongs to a particular category. It uses the logistic function (or sigmoid function) to transform its output to a probability value which can then be mapped to two or more discrete classes. This function outputs a value between 0 and 1, which is interpreted as the probability of the dependent variable being a '1' (or true, success, etc.). The model coefficients (or weights) are typically learned using methods like maximum likelihood estimation. Logistic Regression is highly interpretable, computationally inexpensive, and provides probabilities for predictions, making it a fundamental tool for binary classification problems. It's particularly useful in fields such as medical diagnosis, credit scoring, and any domain where probabilistic outcomes are of interest. Despite its simplicity, it can serve as a strong baseline for binary classification problems.

### TF-IDF

| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |



# Deep learning



* ## BERT

BERT base model

The BERT (Bidirectional Encoder Representations from Transformers) base model represents a significant breakthrough in the field of natural language processing (NLP). Developed by Google, it stands out for its ability to understand the context of a word in a sentence by analyzing the words that come before and after it, a method known as bidirectional training. This is a departure from previous models that typically processed text in one direction, either left-to-right or right-to-left. BERT base consists of 12 layers (transformer blocks), 768 hidden units, and 12 attention heads, totaling 110 million parameters. This structure enables it to handle a wide range of NLP tasks, such as question answering, language inference, and sentiment analysis, with remarkable effectiveness. Its pre-training on a large corpus of text, followed by fine-tuning for specific tasks, allows it to achieve state-of-the-art results across various benchmarks.





| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 86.87%   | 87.76%    | 98.62% | 92.87%   |



<br />

​                   


* ## RoBERTa

 RoBERTa base model

RoBERTa (Robustly Optimized BERT Approach) is an enhanced version of the original BERT model, optimized for improved performance in natural language understanding tasks. Developed by Facebook AI, RoBERTa modifies key hyperparameters in BERT, such as training the model with larger mini-batches and learning rates, and training on more data for a longer period. Unlike BERT, RoBERTa removes the next sentence prediction objective and instead focuses solely on more extensive masked language modeling. This approach allows for deeper bidirectional context understanding. The base version of RoBERTa is similar in size to BERT base, with 12 layers, 768 hidden units, and 12 attention heads. However, it distinguishes itself by demonstrating superior performance on a range of benchmark NLP tasks. Its success can be attributed to these subtle yet impactful changes in training methodology and model architecture, which enable it to better capture nuances in language.



| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 86.99%   |  87.78%   | 98.74% |  92.94%  |

<br />

* ## Feed Forward

 Feed Forward base model

A feedforward neural network is a foundational model in the field of machine learning and artificial intelligence, characterized by its simplicity and versatility. In a feedforward model, information moves in only one direction – from input nodes, through hidden layers (if any), and finally to output nodes. There are no cycles or loops in the network, distinguishing it from more complex architectures like recurrent neural networks. The "base" version of a feedforward network typically refers to a basic configuration with a single hidden layer, although the complexity can vary. Each node in the hidden layer transforms the input via a set of learned weights and a non-linear activation function, enabling the network to capture complex relationships in the data. Feedforward networks are widely used in tasks like classification and regression, serving as a fundamental building block for more advanced neural network architectures. Their straightforward structure makes them an excellent starting point for understanding neural network operations.



| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 86.99%   |  87.78%   | 98.74% |  92.94%  |

<br />

* ## XLMBERT

XLMBERT  model

XLMBERT (Cross-Lingual Masked Language Model using BERT) is an advanced variant of the original BERT model, designed to excel in cross-lingual understanding and tasks. It extends the capabilities of BERT to multiple languages, enabling the model to understand and process text across different linguistic contexts. This is achieved by pre-training the model on a large, diverse corpus of text spanning multiple languages. Unlike BERT, which focuses on understanding language in a largely monolingual context, XLMBERT leverages a cross-lingual masked language model training, which allows it to predict missing words in a sentence not only in one language but across different languages. This enhances its ability to understand the nuances and contexts of words in multiple languages simultaneously. XLMBERT's architecture typically follows the transformer-based design of BERT, but it is fine-tuned to handle the complexities and subtleties of multilingual processing. As a result, XLMBERT is particularly effective in tasks that require understanding and processing information across different languages, such as machine translation, multilingual classification, and cross-lingual information retrieval.





| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 86.99%   |  87.78%   | 98.74% |  92.94%  |

<br />
