Task: Calculate PPL
==============
Description: Computes PPL of given sentences in a given model

The motivation behind this experiment is the discussion below:
https://github.com/facebookresearch/ParlAI/discussions/4916

On how to compute probability of a sentence in a given language model

### Example:
By runing this command, the sentences in sentences.txt are fed to the
blender_90M model, and PPL is calculated (alongside other metrics) and
stored in the log/logs.jsonl file
 ```shell 
python parlai/scripts/eval_model.py -t calculate_ppl --model 'transformer/generator' --model-file zoo:blender/blender_90M/model --world-logs parlai/tasks/calculate_ppl/log/logs
 ```
