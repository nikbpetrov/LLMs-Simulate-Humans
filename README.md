# Python code - main

This is the main code of the paper - `codebook.ipynb`. The R code, in the `R_codebook.Rmd` is used for factor analysis and plotting - this is clearly signposted in the `codebook.ipynb`.

## Set up environment

If you are using Anaconda:
`conda env create -f environment.yml`

If you are using pip:
Recommended Python version: 3.10.13
`pip install -r requirements.txt`

## Rerunning

All code should be run fine. Note that there are two main parts that will not be directly rerunnable:
+ code related to the BBC data processing - the raw data is not shared but all code that was used to process the data is present
+ code related to the Chat-GPT requests - this is disabled/commented out to prevent accidents, but can be used; will need to create an `.env` file - see the `codebook.ipynb` for more information

# R code

The code requires a few packages to be installed. The markdown installs those packages for you, if they are not present.

# GPT-3.5 and GPT-4 requests (raw_data)

The original files for silicon personas' requests in data/raw_data, namely `silicon_gpt35_requests.jsonl`, `silicon_gpt35_requests_results`, `silicon_gpt4_requests.jsonl`, and `silicon_gpt4_requests_results` are >100MB, so these are split into 3 files. These split files are then merged back in the `codebook.ipynb`. The code splitting and merging processes is in the `codebook.ipynb`.