# DISCO: A Large Scale Human Annotated Corpus for Disfluency Correction in Indo-European Languages

Authors: Vineet Bhat, Preethi Jyothi, Pushpak Bhattacharyya

Accepted at: EMNLP 2023 Findings

Link to paper: https://arxiv.org/abs/2310.16749

Abstract: Disfluency correction (DC) is the process of removing disfluent elements like fillers, repetitions and corrections from spoken utterances to create readable and interpretable text. DC is a vital post-processing step applied to Automatic Speech Recognition (ASR) outputs, before subsequent processing by downstream language understanding tasks. Existing DC research has primarily focused on English due to the unavailability of large-scale open-source datasets. Towards the goal of multilingual disfluency correction, we present a high-quality human-annotated DC corpus covering four important Indo-European languages: English, Hindi, German and French. We provide extensive analysis of results of state-of-the-art DC models across all four languages obtaining F1 scores of 97.55 (English), 94.29 (Hindi), 95.89 (German) and 92.97 (French). To demonstrate the benefits of DC on downstream tasks, we show that DC leads to 5.65 points increase in BLEU scores on average when used in conjunction with a state-of-the-art Machine Translation (MT) system.

Steps to reproduce results - 

1. crf_and_rnn-training.ipynb - To run CRF and RNN models for Sequence tagging based disfluency correction & testing
2. seqganbert-training.ipynb - To run the Seq-GAN-BERT model for DC using labeled and unlabeled data
3. transformer-training.ipynb - Training multilingual transformers like MuRIL & XLMR for sequence tagging based DC

Entire dataset can be found in ./data/labeled-data/

## Citation 
```
@inproceedings{Bhat2023DISCOAL,
  title={DISCO: A Large Scale Human Annotated Corpus for Disfluency Correction in Indo-European Languages},
  author={Vineet Bhat and Preethi Jyothi and Pushpak Bhattacharyya},
  year={2023},
  url={https://api.semanticscholar.org/CorpusID:264451744}
}




