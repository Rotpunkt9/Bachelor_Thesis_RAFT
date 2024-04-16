# Bachelor_Thesis_RAFT
This repository contains the code and data used in my Bachelor thesis on "Disinformation detection using Large Language Models (LLMs)"

## Abstract:
Disinformation is a pervasive, multifaceted problem in our digital age, which poses significant threats to our society, including political processes. Conventional fact-checking methods cannot keep up with the flood of information spread online. Therefore automatic disinformation detection methods are needed. The advent of Large Language Models (LLMs) has opened new avenues to address this problem. LLMs, with their advanced language understanding capabilities, can be utilized to detect disinformation, making them a valuable tool for this task.

This thesis presents a novel method, Rationale-Augmented Fine-Tuning (RAFT), for enhancing the disinformation detection capabilities of Small Language Models (SLMs). By leveraging the analytical reasoning capabilities of LLMs, RAFT aims to improve the performance of SLMs in identifying fake news. The research conducted in this thesis involved the creation of a rationale-augmented dataset using GPT-3.5 and fine-tuning the SLM Mistral-7B using this dataset.

The results demonstrate the effectiveness of the RAFT model in disinformation detection across multiple benchmark datasets, often outperforming both the base SLM before fine-tuning and the LLM teacher model. The thesis concludes that RAFT significantly enhances the disinformation detection capabilities of SLMs, offering a promising direction for future research in combating fake news.
## Data
This folder contains all five test sets used to evaluate the performance of the models.

## Code
Contains five jupyter notebooks.
extend_data_with_gpt: Contains the code used to augment the ISOT dataset with rationales. GPT-3.5 is used via API requests. 


Mistral_finetuning_RAFT: This notebook was used to fine-tune Mistral-7B on the ratinoale-augmented dataset. 


Mistral_ollama_inference: This code was used for the baseline evaluation of the SLM before fine-tuning.


RAFT_model_inference: This notebook was used to create the predictions for the test sets by the RAFT model (after fine-tuning)


evaluation_final: With this notebook the results were evaluated and the results plotted.
