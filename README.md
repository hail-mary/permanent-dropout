# Neuron Pruning as a Tool for Accelerating Deep Reinforcement Learning

## Installation
We recommend using Miniconda to create your virtual env.
```
conda create -n pruning_env python=3.11
conda activate pruning_env
git clone https://github.com/hail-mary/neuron-pruning.git
cd neuron-pruning
pip install gymnasium[mujoco] stable-baselines3 pyyaml
```

## Training
```
python main.py

# option: specify the log directory by adding `--logdir` flag.
python main.py --logdir logs
```

## Evaluation
```
python main.py --eval [PATH_TO_CHECKPOINTS]

# option: recording requires ->> pip install "gymnasium[other]"
python main.py --eval [PATH_TO_CHECKPOINTS] --record
```

## Plot results
`--plot` can also accept multiple json files for comparison.
```
python main.py --plot .\logs\history.json
```

