# MLDL2021

BERT is one of the most efficient language representation models introduced in last years. Its transformer-based architecture permits to create state-of-art models for a wide range of tasks by easily fine-tuning the pre-trained BERT.
Conceptually simple and powerful, BERT is the strong basis for solving many tasks, especially the question answering one included in the functioning of search engines. Furthermore, proving it as a Markov Random Field Language Model is useful to consider BERT as a high-quality, fluent text generator too. In this work, first its structure is analyzed and its results as a text generator are compared to other existing models. Finally the power of BERT is extended in the specific field of question answering task.

# Basic Usage

The [main script](https://github.com/annalisad98/MLDL2021/blob/main/MLDLproject.ipynb) is a workable replica from [BERT has a Mouth, and It Must Speak](https://github.com/nyu-dl/bert-gen), where BERT as a text generator is compared with [OpeanAi GPT](https://github.com/huggingface/pytorch-openai-transformer-lm/tree/d848a49f718b75287e1bd0364803c41c6b1deef5), [Transfomer-XL](https://github.com/huggingface/transformers/tree/master/src/transformers/models/transfo_xl) and [XL-Net](https://github.com/huggingface/transformers/tree/master/src/transformers/models/xlnet). The evaluation is made using both the metrics from [BERT has a Mouth, and It Must Speak](https://github.com/nyu-dl/bert-gen) and the metrics from the [Texygen platform](https://github.com/geek-ai/Texygen).
In order to run the code, it is necessary to upload some files from [data](https://github.com/annalisad98/MLDL2021/tree/main/data):         
* datawiki103.5k.txt: it is a sample of 5000 sentences from WikiText-103 test set
* tbc.5k.txt: it is a sample of 5000 sentences from Toronto Book Corpus (TBC)
* wiki_train_1000_samples.txt: it is a sample of 1000 sentences from WikiText-103 train set. Here is the [code](https://github.com/annalisad98/MLDL2021/blob/main/file_gen/wiki1000sample.ipynb) to generate it.
* wt40.txt: it contains 40 prompts (sentences truncated at the sixth token), sampled from WikiText-103 train set. Here is the [code](https://github.com/annalisad98/MLDL2021/blob/main/file_gen/wiki40prompts.ipynb)



Wiki1000sample:
It is a script used to randomly select 1000 phrases from the WikiText-103 dataset. 
At first the titles conteinded in the dataset are discarded, leaving only the phrases. Then the 1000 

# Implemented Models and Original Papers
