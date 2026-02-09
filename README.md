# Amiya26
This repository is shared under <a  href="LICENSE">Academic Free License (AFL) v. 3.0</a>
and lists the resources compiled by us for the VarDial/AMIYA 2026 Shared task in EACL26.


Please check <a href="https://sites.google.com/view/vardial-2026/shared-tasks">here</a> for more information on the competition!

<a href="https://huggingface.co/meta-llama/Llama-3.1-8B-Instruct">Llama</a> and 
<a href="https://huggingface.co/Qwen/Qwen2.5-7B-Instruct">Qwen </a> models 
fine-tuned using LoRA implementations in LllamaFactory 
using the data shared in the competition (processing described in <i>Dataset description(Sheet1).csv</i> and <i>notes_translation_data.pdf</i>)
are available at <br>
https://huggingface.co/mood157/dialect_translator_clean_qwen2.5_7B_instruct <br>
and 
https://huggingface.co/mood157/dialect_translator_clean_llama_3.1_8B_instruct


Our "primary" model that does best on dialectness scores (after RL training on preference data compiled by us)
is available at 
https://huggingface.co/gsdas/amiya_llama3.1_dpo

The "tentative_gold" data we used in evaluation for the systems paper (Table 2).
About 50 prompts (from AL-QASIDA) per dialect were selected to prompt the GPT-4o model. The output is considered "gold" if our classifier
detects it is in the correct dialect, if not, we apply translation to convert the output to the required dialect and once again test it using our classifier.

Our dialect classifier (adapter for Llama) is available at https://huggingface.co/gsdas/amiya_dialect_predictor

We also shared the preference data used for training our RL models (rl_pairs.json) and a sample subset of data from the competition that can be used to test our dialect prediction model.
