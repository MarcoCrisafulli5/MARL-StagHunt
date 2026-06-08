# MARL-StagHunt

The StagHunt environment available [here](https://github.com/giorgiofranceschelli/Gymnasium-Stag-Hunt/tree/master) contains 3 multi-agent grid-based stochastic games, the aim of this project is to explore prosocial behavior in multi-agent
reinforcement learning. 

Indipendent Deep Q-Learning implemented with a shared experience buffer.
Config is centralized into Configuration section of the notebook.

## Requirements
- Python **3.11 exactly** (higher versions may cause compatibility issues)

## Features 

- Visualize training progress at training time
- TensorBoard optional
- Section for a simple evaluation included
- Save and Load weights of the trained networks

## Installation

Clone this repo first, then clone the Gymnasium-Stag-Hunt repo, *Install the packages insisde a new virtaul environment .venv*.
VSCode users in order to prevent bugs with kernel not found, your folder structure should like this:
```
  MARL-StagHunt/
  |-.venv/
  |-Gymnasium-Stag-Hunt/
  |-notebook.py
  |... rest of the stuff
```

If you create .venv in a parent folder to MARL-StagHunt or inside Gymnasium-Stag-Hunt, it may not be recognised and available in the kernel list when you try to execute the notebook!!

Instructions below show correct installation process:

```bash
git clone https://github.com/MarcoCrisafulli5/MARL-StagHunt.git
cd MARL-StagHunt
python -m venv .venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows
git clone https://github.com/giorgiofranceschelli/Gymnasium-Stag-Hunt/tree/master
cd Gymnasium-Stag-Hunt
pip install -e .
cd ..
pip install -r requirements.txt
