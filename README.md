# Awesome Humanoid & Legged Robotics 🤖

A curated collection of tested open-source projects for humanoid and legged robots. This repository focuses on **practical deployment** and **engineering experience**, covering simulation, reinforcement learning, motion imitation, sim-to-real, and control optimization.

---

## 📑 Table of Contents
- [RL Locomotion Frameworks](#rl-locomotion-frameworks)
- [Motion Imitation (AMP/DeepMimic)](#motion-imitation-ampdeepmimic)
- [Robotics Toolkits & Optimization](#robotics-toolkits--optimization)
- [Evaluation Criteria](#evaluation-criteria)

---

## 🏃 RL Locomotion Frameworks
*Most frameworks in this category are derived from or inspired by the Legged Gym and Isaac Gym ecosystems.*

### Legged Gym Derivatives
| Project | Description | Rating | Link |
| :--- | :--- | :--- | :--- |
| **Unitree RL Gym** | Standard RL for Unitree robots. | ⭐⭐⭐ | [GitHub](https://github.com/unitreerobotics/unitree_rl_gym) |
| **Humanoid-Gym** | Optimized for humanoid structures. | ⭐⭐⭐ | [GitHub](https://github.com/roboterax/humanoid-gym) |
| **EngineAI Legged Gym** | Modified for specific engineai hardware. | ⭐⭐⭐ | [GitHub](https://github.com/engineai-robotics/engineai_legged_gym) |

### Alternative Engines
* **[Holosoma](https://github.com/amazon-far/holosoma)** ⭐⭐⭐⭐⭐
  * **Status:** Successfully deployed on custom hardware.
  * **Pros:** Excellent sim-to-real performance; robot can walk stably.
* **[MujocoPlayground](https://github.com/google-deepmind/mujoco_playground)** ⭐⭐
  * **Status:** Tested.
  * **Cons:** Not friendly for custom robot, bad trainning performance.

---

## 💃 Motion Imitation (AMP / DeepMimic)

* **[Legged_Lab Extension](https://github.com/zitongbai/legged_lab)** ⭐⭐⭐⭐
  * **Features:** Supports Sim2Sim and Sim2Real (highly extendable).
  * **Verdict:** Good balance between simulation and real-world potential.
* **[MimicKit](https://github.com/xbpeng/MimicKit)** ⭐⭐⭐
  * **Verdict:** Simulation only; lacks direct deployment pipelines.
* **[BeyondMimic](https://github.com/HybridRobotics/whole_body_tracking)** (under test)
  * **Features:** Whole-body tracking in simulation.
* **[EngineAi AMP](https://github.com/engineai-robotics/engineai_amp)** (under test)
  * **Features:** Adversarial Motion Priors implementation.

---

## 🛠️ Robotics Toolkits

* **[GMR (General Motion Retargeting)](https://github.com/YanjieZe/GMR)** ⭐⭐⭐⭐⭐
  * **Features:** Supports any humanoid; successfully tested on custom robot platforms.
  * **Verdict:** Highly recommended for motion retargeting.
* **[Pinocchio](https://github.com/stack-of-tasks/pinocchio)** ⭐⭐⭐⭐
  * **Purpose:** High-performance Rigid Body Dynamics (FK, IK, etc.).
  * **Verdict:** Industry standard for analytical control.
* **[Pace-Sim2real](https://github.com/leggedrobotics/pace-sim2real)** ⭐⭐⭐⭐
  * **Purpose:** Actuator identification and system ID.
  * **Verdict:** Essential for closing the gap between sim and real actuators.

---

## 📝 Evaluation Criteria

The ratings are purely based on our **hands-on experience** with a custom humanoid platform. We focused on:

1.  **Ease of Integration:** How difficult is it to swap a custom URDF?
2.  **Sim-to-Real Transfer:** Do the policies work on physical hardware without heavy tuning?
3.  **Extensibility:** Can we easily modify the reward functions or observation space?
4.  **Motion Quality:** Is the gait natural or "jittery"?

---

*“Engineering is about making things work in the real world, not just in a paper.”*
