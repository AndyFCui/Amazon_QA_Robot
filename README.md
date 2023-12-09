# Amazon_QA_Robot
This is QA Robot use NLP to training a smart robot agent

## Project Member:
- Andy(Xiangyu) Cui, cui.xiangyu@northeastern.edu
- Zichong Meng, meng.zic@northeastern.edu
- Xichen Liu, liu.xic@northeastern.edu
- Xueyan Feng, feng.xuey@northeastern.edu

## Basic Idea
- In traditional settings, manual customer service takes time and experience to answer customer questions. Our group sees this challenge in our daily life and would like to propose a solution to   this problem. We would like to implement a customer service chatbot to assist users to gain knowledge of amazon products. We would like to use amazon customer questions and answers and           build/use our artificial intelligence agent to conduct in-speed and accurate response while optimizing operational costs.

## Approach to Solution
- We will use the following datasets:
- https://www.kaggle.com/datasets/PromptCloudHQ/toy-products-on-amazon

- The dataset contains numerous lines of customer questions and answers to each question from amazon about toys. The questions and answers are splitted using  The questions and answers are in a csv file, but a question and answer pair shares the same QuestionID. We will use those questions as our training input and those answers as our targets. 

- We planned to train two different kinds of neural network models, thus to see how two different QA models perform. We would like to train a Bert based model (encoder only, bidirectional), RoBERTa, and an original transformer model (encoder-decoder structure).
Also we plan to perform visualizations on the model embeddings using T-SNE, and we would also like to create several answer maps for test cases to show each of the model performances.
Related work
Question Answering Systems: Survey and Trends
https://doi.org/10.1016/j.procs.2015.12.005
Question and Answer Test-Train Overlap in Open-Domain Question Answering Datasets
https://doi.org/10.48550/arXiv.2008.02637
Learning to Answer by Learning to Ask: Getting the Best of GPT-2 and BERT Worlds
https://doi.org/10.48550/arXiv.1911.02365
Assessment methodology
We will adopt the following methodology to assess our models within this project:

## Evaluation Metric:
We'll track the percentage of questions our models answer correctly, and we will also employ F1 metric and BLEU score to assess the details of each model's performance, especially in our setting where our datasets are imbalanced.

## Discussion:

## GPT2 finetuned model weights
```bash
pip install gdown
```
For 25 epoch
```bash
gdown 1TPkEpr-Z4PxN4lW5m_X-Epge1QT3bfOr
```
For 50 epoch
```bash
gdown 1YM976lPRR30ccaNkSL1zhpuhmSZeQ_-v
```
