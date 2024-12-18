# Permanent-Dropout: Simultaneous Modification of Policy Architecture and Parameters

## Installation
We recommend using Miniconda to create your virtual env.
```
conda create -n dropout_env python=3.11
conda activate dropout_env
git clone https://github.com/hail-mary/permanent-dropout.git
cd permanent-dropout
pip install gymnasium[mujoco] stable-baselines3 pyyaml
```

## Training
```
cd permanent-dropout
python main.py
```

