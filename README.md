# SkimLit (Skim Literature)

For this project I have taken inspiration from the paper [*PubMed 200k RCT: a Dataset for Sequenctial Sentence Classification in Medical Abstracts*](https://arxiv.org/abs/1710.06071).

The goal of the paper was to explore the ability for NLP models to classify sentences which appear in sequential order.

I have trained various models which are able to classify each sentence of the abstract of a RCT research paper, to one of the particular classes **BACKGROUND, CONCLUSIONS, METHODS, OBJECTIVE, RESULTS**.

![Skimlit example inputs and outputs](https://raw.githubusercontent.com/mrdbourke/tensorflow-deep-learning/main/images/09-skimlit-overview-input-and-output.png)
[<div align="center">*image source*</div>](https://raw.githubusercontent.com/mrdbourke/tensorflow-deep-learning/main/images/09-skimlit-overview-input-and-output.png)

<div align="center">

| Models | Accuracy | Precision | Recall | F1 |
| ---- | ---- | ---- | ---- | ----|
| Baseline | 0.772 | 0.841 |  |  |
| char_word_positional_embedding | 0.863 | 0.825 |  |  |
| char_pretrained_word_positional_embedding | 1.031 | 0.799 |  |  |
| Conv1D_token_embed | 1.091 | 0.706 |  |  |
| char_pretrained_word_embedding | 1.196 | 0.681 |  |  |

<i>Table comparing accuracy and loss of different models on the test dataset</i></div>
