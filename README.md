# fine-tuning-gpt2-gemma-llama
### this project explores how different LLMs can be fine-tuned to generate high-quality forum replies that simulate realistic peer or instructor interaction.

### Model used
| Model           | Description                         | Fine-Tuning Method   |
| --------------- | ----------------------------------- | -------------------- |
| **GPT-2 Small** | Lightweight autoregressive model    | Full fine-tuning     |
| **Gemma 7B IT** | Instruction-tuned Google model      | LoRA + QLoRA (4-bit) |
| **LLaMA 3 8B**  | Meta's SOTA model for general tasks | LoRA + QLoRA (4-bit) |
