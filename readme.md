Observational learning
======================

## Installation

Based on instruction from spinningup. 

Create conda environment 
   ```
   conda create -n ol python=3.6
   source activate ol
   ```
   
Install the right version of CUDA for your GPU. In my case:
   ```
   conda install cudatoolkit=9.0
   conda install cudnn
   git clone git@github.com:benlansdell/obs-rl-sac.git
   cd obs-rl-sac
   pip install -e .
   ```
   
Install gym-minigrid (https://github.com/benlansdell/gym-minigrid)

Test:
```python -m spinup.run sacd --hid "[32,32]" --env MiniGrid-Blocks-6x6-v0 --exp_name test_sacd --gamma 0.999```
