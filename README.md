# Quick Start
### 1. Edit Llama3 (8B) model 
 
    python -m experiments.evaluate     --alg_name=MEMIT_seq     --model_name=meta-llama/Meta-Llama-3-8B-Instruct     --hparams_fname=Llama3-8B.json --ds_name=mcf --dataset_size_limit=2000    --num_edits=100  --downstream_eval_steps=5


### 2. Summarize the results  
To summarize the results, you can use [`experiments/summarize.py`](experiments/summarize.py):

    python -m experiments.summarize --dir_name=MEMIT_seq --runs=run_<run1>,run_<run2>
