# Bachelor_Thesis_RAFT
This repository contains the code and data used in my Bachelor thesis on "Disinformation detection using Large Language Models (LLMs)"
## Data
This folder contains all five test sets used to evaluate the performance of the models.

## Code
Contains five jupyter notebooks.
extend_data_with_gpt: Contains the code used to augment the ISOT dataset with rationales. GPT-3.5 is used via API requests. 
Mistral_finetuning_RAFT: This notebook was used to fine-tune Mistral-7B on the ratinoale-augmented datase. 
Mistral_ollama_inference: This code was used for the baseline evaluation of the SLM before fine-tuning.
RAFT_model_inference: This notebook was used to create the predictions for the test sets by the RAFT model (after fine-tuning)
evaluation_final: With this notebook the results were evaluated and the results plotted.
