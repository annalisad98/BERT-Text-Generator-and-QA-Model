# MLDL2021

BERT is one of the most efficient language representation models introduced in last years. Its transformer-based architecture permits to create state-of-art models for a wide range of tasks by easily fine-tuning the pre-trained BERT.
Conceptually simple and powerful, BERT is the strong basis for solving many tasks, especially the question answering one included in the functioning of search engines.
Furthermore, proving it as a Markov Random Field Language Model is useful to consider BERT as a high-quality, fluent text generator too. In this work, first its structure is analyzed and its results as a text generator are compared to other existing models. Finally the power of BERT is extended in the specific field of question answering task.

## Basic Usage

The [main script](https://github.com/annalisad98/MLDL2021/blob/main/MLDLproject.ipynb) is a workable replica from [BERT has a Mouth, and It Must Speak](https://github.com/nyu-dl/bert-gen), where BERT as a text generator is compared with [OpeanAi GPT](https://github.com/huggingface/pytorch-openai-transformer-lm/tree/d848a49f718b75287e1bd0364803c41c6b1deef5), [Transfomer-XL](https://github.com/huggingface/transformers/tree/master/src/transformers/models/transfo_xl) and [XL-Net](https://github.com/huggingface/transformers/tree/master/src/transformers/models/xlnet). The evaluation is made using both the metrics from [BERT has a Mouth, and It Must Speak](https://github.com/nyu-dl/bert-gen) and the metrics from the [Texygen platform](https://github.com/geek-ai/Texygen).
In order to run the code, it is necessary to upload some files from [data](https://github.com/annalisad98/MLDL2021/tree/main/data):         
* datawiki103.5k.txt: it is a sample of 5000 sentences from WikiText-103 test set
* tbc.5k.txt: it is a sample of 5000 sentences from Toronto Book Corpus (TBC)
* wiki_train_1000_samples.txt: it is a sample of 1000 sentences from WikiText-103 train set. Consider this link [code](https://github.com/annalisad98/MLDL2021/blob/main/file_gen/wiki1000sample.ipynb) to generate it.
* wt40.txt: it contains 40 prompts (sentences truncated at the sixth token), sampled from WikiText-103 train set. For the code refer to this link [code].(https://github.com/annalisad98/MLDL2021/blob/main/file_gen/wiki40prompts.ipynb)


## Bert for Question Answering
[MLDL2](https://github.com/annalisad98/MLDL2021/blob/main/MLDL2.ipynb) implements the [web app for Question Answering](https://d4ephv6bpz2b2gkf.anvil.app/6L3Z3ZV54XCQ2BF4DY7FJQBD) using the multi-language model [XLM-RoBERTa](https://github.com/huggingface/transformers/tree/master/src/transformers/models/xlm_roberta). The available languages are English, Italian and French. In this script we consider three short texts on different topics and the questions have to relate to these texts, but possible applications could rely on bigger datasets, allowing more general questions.

## Implemented Models and Original Papers
* BERT-gen: [BERT has a Mouth, and It Must Speak: BERT as a Markov Random Field Language Model](https://arxiv.org/abs/1902.04094)
* OpenAi GPT: [Improving Language Understanding by Generative Pre-Training](https://openai.com/blog/language-unsupervised/)
* Texygen: [Texygen: A Benchmarking Platform for Text Generation Models](https://arxiv.org/abs/1802.01886)
* Transformer-XL: [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860)
* XLNet [XLNet: Generalized Autoregressive Pretraining for Language Understanding](https://arxiv.org/abs/1906.08237)
* XLM-RoBERTa [Unsupervised Cross-lingual Representation Learning at Scale](https://arxiv.org/abs/1911.02116)
