# LAURAE
This repository includes the code and datasets required to reproduce experiments and the proposed LAURAE model for automatic readability assessment. The corresponding paper "Zero-shot Large Language Models for Automatic Readability Assessment" is published in ACL 2026.  


## Files
- The datasets with texts, ground truth readability labels, and all collected readability scores can be found in the "datasets" subfolder.
- The Python files used to collect the LLM readability scores (including prompts) for each dataset are stored in the "collection" subfolder. All LLMs are open-source models available through Huggingface, and can be implemented with the Transformers library.
- The RSRS readability scores can be collected using the "calc_RSRS.ipynb" file. The code was developed based on the RSRS implementation at: https://github.com/kinimod23/GRANT.
- The code to produce LAURAE scores by ensembling the readability formula and LLM scores with weights derived from LLM's verbal confidence score can be found in "getting_readability_corrs_LAURAE.ipynb". The main results of the paper can be replicated using this file. 
