# CSE573-Fake Review Detection Group 6
 CSE573 Fake Review Detection


# Dataset

[Amazon Data Set](https://github.com/adityasinha0523/CSE573-Fake-Review-Detection-Group-6/blob/main/DATA)



# Classification Algorithms

Utilized different classification Algorithms


## SVM

### TF-IDF

| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |




## Multinominal Naive Bayes

### TF-IDF

| Accuracy | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| 85.65%   |   85.66%  | 98.12% |  92.25%  |



## Logistic Regression

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