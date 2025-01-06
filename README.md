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
python main.py --logdir logs
```

## Evaluation
```
python main.py --eval [PATH_TO_MODEL]
# optional: recording, requires pip install "gymnasium[other]"
python main.py --eval [PATH_TO_MODEL] --record_video
```

## Plot results
```
python main.py --plot .\logs\history.json
```

## References
* Averaging Weights Leads to Wider Optima and Better Generalization
* Improving Stability in Deep Reinforcement Learning with Weight Averaging
