# SkimLit (Skim Literature)

For this project I have taken inspiration from the paper [*PubMed 200k RCT: a Dataset for Sequenctial Sentence Classification in Medical Abstracts*](https://arxiv.org/abs/1710.06071).

The goal of the paper was to explore the ability for NLP models to classify sentences which appear in sequential order.

I have trained various models which are able to classify each sentence of the abstract of a RCT research paper, to one of the particular classes **BACKGROUND, CONCLUSIONS, METHODS, OBJECTIVE, RESULTS**.

![Skimlit example inputs and outputs](https://raw.githubusercontent.com/mrdbourke/tensorflow-deep-learning/main/images/09-skimlit-overview-input-and-output.png)
[*image source*](https://raw.githubusercontent.com/mrdbourke/tensorflow-deep-learning/main/images/09-skimlit-overview-input-and-output.png)

<div align="center">

| Models | Accuracy | Precision | Recall | F1 |
| ---- | ---- | ---- | ---- | ----|
| Baseline | 72.183 | 0.718 | 0.721 | 0.698 |
| (character + word + positional) embedding | 86.478 | 0.868 | 0.864 | 0.861 |
| (character + pretrained_word + positional) embedding | 86.253 | 0.862 | 0.862 | 0.860 |
| word embedding | 82.516 | 0.824 | 0.825 | 0.823 |
| (character + pretrained_word) embedding | 80.031 | 0.800 | 0.800 | 0.796 |

<i>Table comparing accuracy, precision, recall and f1-score of different models</i></div>

You can view the training results of the models on [Tensorboard](https://tensorboard.dev/experiment/SEn1rZGlSvKtVwjlZIexlQ/#scalars).

You can access all the trained models [here](https://drive.google.com/drive/folders/11sl9w5jjg2pgrSyiuK6HdWnn9UXqVbcV?usp=share_link).
