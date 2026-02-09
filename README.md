# Amiya26
This repository lists few of our resources compiled for the VarDial/AMIYA 2026 Shared task in EACL26.

Please check <a href="https://sites.google.com/view/vardial-2026/shared-tasks">here</a> for more information.

<a href="https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct">Llama</a> and <br>
<a href="https://huggingface.co/Qwen/Qwen2.5-7B-Instruct">Qwen </a> models 
fine-tuned using LoRA implementations in LllamaFactory 
using the data shared in the competition (processing described <a href="">here</a> are available at 

https://huggingface.co/mood157/dialect_translator_clean_qwen2.5_7B_instruct
and 
https://huggingface.co/mood157/dialect_translator_clean_llama_3.1_8B_instruct


Our "primary" model that does best on dialectness scores (after RL training on preference data compiled by us)
is available at 
https://huggingface.co/gsdas/amiya_llama3.1_dpo

For further details, please refer to the systems paper.
