# Building-Large-Language-Models-from-Scratch

This will be my walk through of the book "Building Large Language Models from Scratch" by Sebastian Raschka

 <a href="http://mng.bz/orYv"><img src="images/Raschka-HI.png" width="250px"></a> 

 As of Monday, September 23, 2024, this book has not yet been released but will be October 29, 2024 on amazon.ca.

 I am expecting the [current repo](https://github.com/rasbt/LLMs-from-scratch) to be updated up until that publication date.

 mamba activate llmfs


## Monday, September 23, 2024

Setting up of the local mamba environment for this book. 

 1) mamba create -n llmfs
 2) mamba activate llmfs
 3) mamba install conda-forge::python
 4) mamba install conda-forge::jupyterlab
 5) mamba install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
 6) mamba install conda-forge::tiktoken
 7) mamba install conda-forge::matplotlib
 8) mamba install conda-forge::pandas
 9) mamba install conda-forge::tqdm
10) mamba install conda-forge::psutil

## Tuesday, September 24, 2024

Gotta say he really explains things well and so far does not skim over any important details! I really like that!

## Saturday, September 28, 2024

11) mamba install conda-forge::transformers

## Thursday, October 3, 2024

Continue to go through this most excellent resource! It is really well written! And the [original repo](https://github.com/rasbt/LLMs-from-scratch) continues to be updated to this day! 

## Tuesday, October 22, 2024

Starting to go through 'Chapter 5 - Pretraining on unlabeled data'

12) pip install thop

## Wednesday, October 23, 2024

Looks like we need tensorflow for Chapter 5. Rather then just installing it to the environment, I will create a new environment for it by cloning 'llmfs' to 'llmfs-tf' and then installing tensorflow to that environment.

mamba create -n llmfs-tf --clone llmfs
mamba activate llmfs-tf
pip install tensorflow

Nice! This new environment works with the code from chapter 5.

## Thursday, October 24, 2024

mamba activate llmfs

13) mamba install conda-forge::ipywidgets

## Friday, October 25, 2024

Creating an environment.yml file for the llmfs-tf environment. Then I will create a new environment from that file on KAUWITB. 