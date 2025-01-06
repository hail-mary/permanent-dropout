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
# optional: recording
python main.py --logdir logs --record_video
```

## Evaluation
```
python main.py --eval [PATH_TO_MODEL]
```

## References
* Averaging Weights Leads to Wider Optima and Better Generalization
* Improving Stability in Deep Reinforcement Learning with Weight Averaging
