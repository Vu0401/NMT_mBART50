# NMT_mBART50-Machine-Translation

This repository focuses on Neural Machine Translation (NMT) using the `facebook/mbart-large-50-many-to-many-mmt` model. It utilizes the `mt_eng_vietnamese` dataset from `iwslt2015-en-vi`.

## Introduction

This project leverages the `facebook/mbart-large-50-many-to-many-mmt` model to perform machine translation between English and Vietnamese. The `iwslt2015-en-vi` dataset is used for training and evaluation purposes.

## Performance

The model's performance is evaluated using the BLEU (Bilingual Evaluation Understudy) score, which is a metric for comparing a candidate translation of text to one or more reference translations. The BLEU score for this project is 34.871400.

### Significance of the BLEU Score

The BLEU score is a widely used metric for evaluating the quality of machine-translated text. It ranges from 0 to 100, where a higher score indicates a closer match to the reference translations. A BLEU score of 34.871400 suggests that the model performs quite well in translating between English and Vietnamese, achieving a substantial level of accuracy and fluency. While not perfect, this score indicates that the translations are generally of good quality and useful for practical applications.

## Inference

To perform inference using the model, you can use the following example:

```python
prompt = 'i go to school'
translation = inference(prompt, cfg.tokenizer, model)

print(translation)
# Output: ['tôi đi học.']
