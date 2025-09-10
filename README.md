# IsaacLab Experiments

This project is based on Isaac Lab with Isaac Sim 4.5 on Windows.  
We modify the source codes of Isaac Lab, skrl, and rsl_rl for our experiments.

## Installation

1. Install Isaac Lab following the official installation guide:  
   https://isaac-sim.github.io/IsaacLab/v2.1.0/source/setup/installation/isaaclab_pip_installation.html

2. Replace source codes:  
   - Unzip `isaaclab.zip`, `skrl.zip`, and `rsl_rl.zip`.  
   - Replace the corresponding folders inside:
     ```
     your_directory/env_isaaclab/Lib/site-packages
     ```

3. Add training scripts:  
   - Unzip `scripts.zip` into:
     ```
     your_directory/
     ```

## Training

### PPO

```
python scripts\reinforcement_learning\rsl_rl\train.py --task Isaac-LiftMultiple-Cube-Shadow-v0 --headless
```
### RPO

```
python scripts\reinforcement_learning\skrl\train.py --task Isaac-LiftMultiple-Cube-Shadow-v0 --headless
```

### Available tasks
To try different environments, replace `--task` with one of the following:

- Isaac-LiftMultiple-Cube-Franka-v0  
- Isaac-LiftMultiple-Cube-Shadow-v0  
- Isaac-Lift-Cube-Shadow-v0  
- Isaac-Lift-Cube-Franka-v0  
- Isaac-LiftRotate-Cube-Shadow-v0  
- Isaac-LiftRotate-Cube-Franka-v0  
- Isaac-Rotate-Cube-Shadow-v0  
- Isaac-Rotate-Cube-Franka-v0  
- Isaac-Repose-Cube-Shadow-Direct-v0

