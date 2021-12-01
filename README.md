# text-style-transfer
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/></a>&nbsp
  <img src="https://img.shields.io/badge/GoogleColab-F9AB00?style=flat-square&logo=GoogleColab&logoColor=white"/></a>&nbsp 
</p>
<b><i>Text style transfer</i></b> is to convert a formal piece of text into an informal piece of text, vice cersa. We've encountered the problem of lack of parallel corpora to train these models that could lead to good task performance. In this project, we aim to increase performance of formality style transfer model using in-domain data augmentation methods including synonym replacement and round trip translation. Both of these methods focuses on in-domain training that avoids losing generality and assures the quality of data. Augmentation that replies on synonym replacement replaces certain words of the sentence and round trip translation translate the sentence from one language to another and back. For our baseline model, we incorporate <a href=https://github.com/raosudha89/GYAFC-corpus><b>GYFAC</b></a>(Grammarly's Yahoo Answers Formality Corpus) corpus.<br>
Machine transformers of our model are modeled through sequence to sequence(Seq2Seq) neural architecture along with the attention mechanism. The language model leverages the likelihood of belonging to the target domain and predicts the next word. Furthermore, we explore three different scoring functions that are dot, general and concatenate and evaluate our augmented model compared to the baseline model using BLEU score as our metric.


<h2> major Contributions </h2>

- Improve model performance with **data augmentation** methods
- Explore formality style transfer datasets and models
- Compare results of different scoring variants
- Application of **Attention** mechanism to solve the bottleneck problem of seq2seq
- Wrote short full-paper on our findings and experiments
- Conducted baseline, augmented, ablation study experiments

<h2> Directory </h2>

### _algorithms_
- **tknizer**: tokenizer_formal, informal / augmented_formal, informal
- **model**: Data preprocessing, encoder/decoder with attention, train

### _ppt_
- proposal
- final_report

###### <i>GYFAC corpus is not shown due to confidential issues.</i>
