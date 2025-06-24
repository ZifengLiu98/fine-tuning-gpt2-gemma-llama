# Fine-Tuning LLMs for Online Forum Reply Generation

This repository presents a comparative fine-tuning pipeline for three large language models (LLMs): **GPT-2**, **Gemma 7B**, and **LLaMA 3 8B**, focused on generating meaningful replies to student or teacher posts in online course forums.

## Project Overview

With the rise of AI in education, this project explores how different LLMs can be fine-tuned to generate high-quality forum replies that simulate realistic peer or instructor interaction.

### Objective
Fine-tune and evaluate multiple LLMs on a dataset of forum posts and replies to:
- Improve AI-generated educational discourse.
- Compare performance across model families.
- Provide reproducible training and inference pipelines.

---

## Models Used

| Model        | Description                          | Fine-Tuning Method     |
|--------------|--------------------------------------|------------------------|
| **GPT-2 Small** | Lightweight autoregressive model     | Full fine-tuning       |
| **Gemma 7B IT** | Instruction-tuned Google model       | LoRA + QLoRA (4-bit)   |
| **LLaMA 3 8B**  | Meta's SOTA model for general tasks | LoRA + QLoRA (4-bit)   |

---

##  Project Structure

```text
.
├── notebooks/
│   ├── A1_GPT2_Fine-tuning.ipynb
│   ├── A1_Gemma_Fine-tuning.ipynb
│   ├── A1_LLaMA_Fine-tuning.ipynb
│   └── Combined_Fine_tuning_Models.ipynb
├── data/
│   └── final_cleaned_8330.xlsx         # Forum post-reply dataset (to be updated)
├── models/
│   └── finetuned_gemma-7b-it/          # Saved checkpoints
├── results/
│   ├── gpt2_generated_replies.xlsx
│   ├── gemma_generated_replies.xlsx
│   └── llama_generated_replies.xlsx
└── README.md
