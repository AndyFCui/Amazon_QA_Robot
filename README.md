# Amazon_QA_Robot
This is QA Robot use NLP to training a smart robot agent

## Project Member:
- Andy(Xiangyu) Cui, cui.xiangyu@northeastern.edu
- Zichong Meng, meng.zic@northeastern.edu
- Xichen Liu, liu.xic@northeastern.edu
- Xueyan Feng, feng.xuey@northeastern.edu

## Tech (Bert & GPT-2)
![tech](https://github.com/AndyFCui/Amazon_QA_Robot/assets/10085168/190a8abf-8fe1-4ce2-9e31-a80a547a3d43)

### Bert
![bert](https://github.com/AndyFCui/Amazon_QA_Robot/assets/10085168/2ce99c67-d661-4fb1-b4bb-14117bb438a8)
![bert_kford](https://github.com/AndyFCui/Amazon_QA_Robot/assets/10085168/de34018b-1f89-4778-9850-4c3a1d863e98)

### GPT-2
![gpt2](https://github.com/AndyFCui/Amazon_QA_Robot/assets/10085168/9a7ceb9f-e991-45f8-943c-c440253fe830)
![gpt2_kford](https://github.com/AndyFCui/Amazon_QA_Robot/assets/10085168/d3fb4469-7ff1-43a6-9801-21a72d37ce9f)






 


## Basic Idea
- In traditional settings, manual customer service takes time and experience to answer customer questions. Our group sees this challenge in our daily life and would like to propose a solution to   this problem. We would like to implement a customer service chatbot to assist users to gain knowledge of amazon products. We would like to use amazon customer questions and answers and           build/use our artificial intelligence agent to conduct in-speed and accurate response while optimizing operational costs.

## Approach to Solution
- We will use the following datasets:
- https://www.kaggle.com/datasets/PromptCloudHQ/toy-products-on-amazon

- The dataset contains numerous lines of customer questions and answers to each question from amazon about toys. The questions and answers are splitted using  The questions and answers are in a csv file, but a question and answer pair shares the same QuestionID. We will use those questions as our training input and those answers as our targets. 

- We planned to train two different kinds of neural network models, thus to see how two different QA models perform. We would like to train a Bert based model (encoder only, bidirectional), Bert-base, and an GPT2-small model (decoder only structure).
Also we plan to perform visualizations training process and accuracy to show each of the model performances.
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

## K-Fold Cross-Validation
We will perform K-Fold Cross-Validation studies on both models see how model performs on different fold of data.

## Ablation Studies
We will fine-tune both models with two different configurations of hyperparameters to see which is the best choice for both models.
