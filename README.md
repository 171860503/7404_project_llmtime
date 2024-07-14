# Large Language Models Are Zero Shot Time Series Forecasters

## Announcement

This repository contains the code for the paper
[_Large Language Models Are Zero Shot Time Series Forecasters_](https://arxiv.org/abs/2310.07820)
by Nate Gruver, Marc Finzi, Shikai Qiu and Andrew Gordon Wilson (NeurIPS 2023).

## Installation
Run the following command to install all dependencies in a conda environment named `llmtime`. Change the cuda version for torch if you don't have cuda 11.8. 
```
source install.sh
```
After installation, activate the environment with
```
conda activate llmtime
```
If you prefer not using conda, you can also install the dependencies listed in `install.sh` manually. 

If you want to run OpenAI models through their API (doesn't require access to a GPU), add your openai api key to `~/.bashrc` with
```
echo "export OPENAI_API_KEY=<your key>" >> ~/.bashrc
```

Finally, if you have a diffferent OpenAI API base, change it in your `~/.bashrc` with
```
echo "export OPENAI_API_BASE=<your base url>" >> ~/.bashrc
```

(Or you can just use our group's api key directly, see the comment line in the demo.ipynb - line 8 & 10)

## demo.ipynb

Hi, this is Group 1 of the course COMP7404 in HKU.

Our members include: 
Chen Hongyi 3036122505
Jiang Shuhui 3036213251
TSANG Kwok Keung 3036122361
Jiang Zhuocheng 3036197641
Hu Shurui 3036215742

Our main working is in demo.ipynb and visualize.ipynb(experiments_visualize.html).

Before you get started, please make sure you have completed setting up the environment as instructed in the previous section.

You can change the hyperparameters as you wish to see the performance of each model. Besides you can import new model by presetting its hyperparameters and declare its api in the second code cell.

It should be noted that we remove the 'precomputed_outputs' folder(which mainly include the precomputed outputs of all the models on all the datasets from the git repository of the origin paper) due to the size limit of the submitted files. If you want to take a look at them, please refer to the git repository of our project: https://github.com/171860503/7404_project_llmtime.git