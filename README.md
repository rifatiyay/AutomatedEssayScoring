# Comparative Analysis of the Performance of BERT and SBERT Models in Predicting Essay Scores in Automated Essay Scoring

**Abstract**

Automated Essay Scoring (AES) offers a solution to the time-consuming and subjective nature of manual essay evaluation. This study explores the effectiveness of Bidirectional Encoder Representations from Transformers (BERT) and Sentence-BERT (SBERT) in AES tasks. SBERT, designed for sentence-level semantics, addresses limitations of BERT in understanding overall sentence meaning. The study proposes SBERT with modified pooling techniques combining mean, max, and CLS pooling for enhanced performance.

**Data and Preprocessing**

The study utilizes the Automated Student Assessment Prize (ASAP) 2012 dataset, comprising English essays. Data preprocessing involved cleaning, score normalization, and splitting into training and testing sets based on essay sets.

**Embedding**

SBERT embeddings were generated using pretrained models and tokenizer from the Sentence-Transformers library. Modifications included mean, max, and CLS pooling to capture rich contextual information from essay embeddings.

**Regression with Fully Connected Neural Network (FCNN)**

A FCNN model was initialized and trained using PyTorch, optimizing Mean Squared Error (MSE) as the loss function. Training involved iterating over epochs with Adam optimizer.

**Evaluation and Results**

Model evaluation was based on training time and accuracy measured by Quadratic Weighted Kappa (QWK) score. SBERT with modified pooling achieved a higher QWK score of 0.7336 compared to BERT’s 0.7333, indicating 1.51% higher accuracy. SBERT showed better performance on shorter essays, while BERT performed better on longer essays.

**Conclusion**

The study concludes that SBERT with modified pooling improves AES accuracy marginally. Findings are applicable to AES application development and provide insights for future research in NLP-based scoring systems.
