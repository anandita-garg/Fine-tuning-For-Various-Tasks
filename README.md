# Sentiment-Analysis-Finetuning

The goal of this project was to finetune models for sentiment analysis tasks.
Part of a broader study: https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=11391221

## Datasets And Models
Sentiment Analysis was done for 2 types of data:
1. Binary Classification (dataset: https://www.kaggle.com/datasets/irustandi/yelp-review-polarity)
2. 5-Class Classification (dataset: https://huggingface.co/datasets/Yelp/yelp_review_full)

Models used: DistilBERT (66 Mil), DistilroBERTa-base (82 Mil), ELECTRA (14 Mil)
Finetuning was carried out on Kaggle GPU t4 x2

## Results And Conclusions

### 1. Binary Classification

| Model             | Max Accuracy (%) |
|-------------------|------------------|
| DistilBERT         | 95.98            |
| DistilroBERTa-base | 96.86            |
| ELECTRA            | 95.77            |

### 2. 5-Class Classification

| Model             | Max Accuracy (%) |
|-------------------|------------------|
| DistilBERT         | 66.04            |
| DistilroBERTa-base | 67.64            |
| ELECTRA            | 65.04            |

DistilroBERTa-base outperformed DistilBERT and ELECTRA in both kinds of sentiment analysis.

## Other tasks are available on Kaggle

Natural Language Inference:

https://www.kaggle.com/datasets/ananditaaaaa/deberta-nli

https://www.kaggle.com/datasets/ananditaa/flan-t5-snli-task

https://www.kaggle.com/datasets/ananditaa/electra-snli

CoT Reasoning:

https://www.kaggle.com/datasets/ananditaagarg/0-acuracy-model

https://www.kaggle.com/datasets/ananditaaaaa/flan-t5-base-cot

https://www.kaggle.com/datasets/ananditaaaaa/t5-reasoning-cot
