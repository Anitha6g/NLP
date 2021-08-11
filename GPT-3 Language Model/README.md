# GPT-3 Language Model
Language model with transformer architecture for generating Neural Fake News
Reference:
Code for Defending Against Neural Fake News
Project page at rowanzellers.com/grover, the AI2 online demo, or read the full paper at arxiv.org/abs/1905.12616.

## What's in this repo?

* Code for the Language model(in lm/). This involves training the model as a language model across fields.
* Code for generating neural fake news from a language model, in sample/.
* Code for making your own RealNews dataset in realnews/.
Model checkpoints freely available online for all of the Grover models. For using the RealNews dataset for research, please submit this form.

Scroll down 👇 for some easy-to-use instructions for setting up Grover to generate news articles.
NOTE: If you just care about making your own RealNews dataset, you will need to set up your environment separately just for that, using an AWS machine (see realnews/.)

Quickstart: setting up Grover for generation!

Set up your environment. Here's the easy way, assuming anaconda is installed: conda create -y -n grover python=3.6 && source activate grover && pip install -r requirements-gpu.txt

Download the model using python download_model.py base

Now generate: python sample/contextual_generate.py -model_config_fn lm/configs/base.json -model_ckpt models/base/model.ckpt -metadata_fn sample/april2019_set_mini.jsonl -out_fn april2019_set_mini_out.jsonl
