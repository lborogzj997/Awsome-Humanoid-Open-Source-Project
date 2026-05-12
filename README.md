# Awesome Humanoid Open-Source Projects

A curated collection of tested open-source projects for humanoid and legged robots, covering simulation, reinforcement learning, motion imitation, sim-to-real deployment, control, optimization, and motion retargeting.

We built a custom humanoid/legged robot platform and explored the following frameworks and toolkits for simulation, deployment, and optimization.
The ratings below reflect our hands-on experience with custom robot integration and real-world deployment.

## RL Walking Frameworks
legged/gym, humanod gym, unitree gym, engeai gym etc... (Similar, build on legged gym)--
⭐⭐⭐
https://github.com/unitreerobotics/unitree_rl_gym
https://github.com/roboterax/humanoid-gym
https://github.com/engineai-robotics/engineai_legged_gym

MujocoPlayground (tested, not friendly to a custom robot)
⭐
https://github.com/google-deepmind/mujoco_playground

Holosoma  (Success deploy on a custom robot,can walk)
⭐⭐⭐⭐⭐
https://github.com/amazon-far/holosoma


## AMP / DeepMimic / Motion Imitation

Mimickit (simulation only)
⭐⭐
https://github.com/xbpeng/MimicKit

Legged_Lab extension (sim2sim, sim2real(extendable))
⭐⭐⭐
https://github.com/zitongbai/legged_lab

Beyondmimic(simulation)
⭐⭐
https://github.com/HybridRobotics/whole_body_tracking

EngineAi AMP
⭐⭐
https://github.com/engineai-robotics/engineai_amp


## Robotics Toolkits

Pinocchio(FK,IK)
⭐⭐⭐⭐
https://github.com/stack-of-tasks/pinocchio

Pace-Sim2real，Actuators identification
⭐⭐⭐
https://github.com/leggedrobotics/pace-sim2real

GMR, motion retargeting (support any humanoid, tested on custom robot)
⭐⭐⭐⭐⭐
https://github.com/YanjieZe/GMR

## Notes
Ratings are based on our practical experience with:
Custom humanoid robot integration
Sim-to-sim deployment
Sim-to-real transfer
Motion imitation quality
Ease of modification and extensibility
Most RL locomotion frameworks are derived from or inspired by Legged Gym and Isaac Gym ecosystems.
This repository focuses on practical deployment and engineering experience rather than benchmark-only evaluation.
