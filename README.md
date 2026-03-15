# O'Reilly Live Course: Finetuning Open Source Large Language Models

Repository for the course with all material. 

## Presentation
The [slides](<2026-03-17 Finetuning.pdf>) contain additional
background and theroretical information.

## Python setup 

### uv
If possible, work with [uv](https://astral.sh/uv/). Clone the repository and run `uv sync`.

### anaconda

Create an venv or conda environment and install the following packages:
*    ipykernel
*    ipython
*    ipywidgets
*    jupyter
*    tqdm
*    transformers
*    sentence-transformers
*    bitsandbytes
*    datasets
*    kernels
*    liger-kernel
*    peft
*    trl
*    unsloth

Of course, you can also Use the supplied `requirements.txt`, but some dependencies might be outdated.

## runpod

You can also use runpod. `uv` is already preinstalled there.

## Notebooks

You can either try to run the notebooks directly
or try to follow how I run them and use it as a 
documentation (or run it later).


### Classification
* [10-prepare-dataset-finetune.ipynb: Prepares the dataset for finetuning the classification model (uses data from Amazon reviews)](10-prepare-dataset-finetune.ipynb)
* [11-bert-finetune-classification.ipynb: Finetune a BERT-like model for classificaition](11-bert-finetune-classification.ipynb)
* [12-alternative-zeroshot.ipynb: Alternative approach using a zerosho (NLI) classification model](12-alternative-zeroshot.ipynb)

### Similarity (embedding) finetuning
* [21-sbert-finetune.ipynb: Finetune a sentence BERT (similiarity) model](21-sbert-finetune.ipynb)
* [22a-create-sbert-data-zeroentropy-reranker.ipynb: Optimize the dataset used for finetuning by using a reranker](22a-create-sbert-data-zeroentropy-reranker.ipynb)
* [23-sbert-finetune-qwen-reranker.ipynb: Finetune the similarity model again using the optimized dataset](23-sbert-finetune-qwen-reranker.ipynb)

### Generative model finetuning
#### Full finetune of a Qwen SLM with 700 million parameters
* [31a-qwen3-07-full-finetune.ipynb: Training notebook](31a-qwen3-07-full-finetune.ipynb)
* [31b-qwen3-07.ipynb: Companion notebook for evaluation](31b-qwen3-07.ipynb)
#### LoRA finetune of a Llama model with 1.7 billion parameters
* [32a-llama32-1-huggingface.ipynb: Training notebook](32a-llama32-1-huggingface.ipynb)
* [32b-llama32-1.ipynb: Companion notebook for evaluation](32b-llama32-1.ipynb)
#### LoRA finetune of a SmoLm model from Hugging Face
* [33a-smolm-1-huggingface.ipynb: Training notebook](33a-smolm-1-huggingface.ipynb)
* [33b-smolm-1.ipynb: Companion notebook for evaluation](33b-smolm-1.ipynb)
#### LoRA finetune of a Phi 3.5 model with ~ 4 billion parameters
* [34a-phi3-unsloth.ipynb: Training notebook](34a-phi3-unsloth.ipynb)
* [34b-phi3.ipynb: Companion notebook for evaluation](34b-phi3.ipynb)
