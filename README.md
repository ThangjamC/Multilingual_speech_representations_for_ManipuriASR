# Multilingual_speech_representations_for_ManipuriASR

Lately, there has been a significant trend of moving from deep neural network based hybrid approach to end-to-end (E2E) approach for automatic speech recognition (ASR). While E2E models achieve the state-of-the-art results in most benchmarks for high resource languages, it is always difficult to train descent E2E models with low-resource languages. Given the recent success of Self-supervised learning (SSL) which does not need any labeled data to pretrain a representation for downstream tasks, we present an ASR system for the Manipuri language in News domain using multilingual speech representations in this paper. We follow the state-of-the-art wav2vec2 XLSR approach that uses multilingual speech representations learnt by pretrained model to train a finetuned model. The pre-trained model were finetuned with different configurations and amounts of data with their effects on inference been provided. Further, a language model is used to improve the performance of the system with the limited size of the dataset. Also, recognition error analysis have been discussed. We observe the best Word Error Rate (WER) and character error rate (CER) on test sets obtained by decoding with a language model as 8.25% and 2.43% respectively.

The dataset used in this work are ULCA (open source) and LDCIL (available on request from their website) given in the following links:

https://github.com/Open-Speech-EkStep/ULCA-asr-dataset-corpus
https://data.ldcil.org/manipuri-raw-speech-corpus


Speaker information was annotated manually for ULCA dataset and can be found in the uploaded files train, valid and test.

Also, the trained models can be found at huggingface: https://huggingface.co/thdevi28/Multilingual_based_Manipuri_ASR/tree/main
