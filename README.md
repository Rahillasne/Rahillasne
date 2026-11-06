# Rahil Lasne

**Robot learning, and the docs that let other people run it.**
CS + Linguistics at San José State University (May 2028) · San Francisco Bay Area

[![LinkedIn](https://img.shields.io/badge/LinkedIn-rahil--lasne-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahil-lasne-01ba92267/)
[![PyPI orbit-eval](https://img.shields.io/pypi/v/orbit-eval?label=PyPI%20orbit-eval&color=3775A9)](https://pypi.org/project/orbit-eval/)
[![CoRL 2026](https://img.shields.io/badge/CoRL%202026-2%20workshop%20papers-B31B1B)](#papers)
[![LeRobot PR merged](https://img.shields.io/badge/huggingface%2Flerobot-PR%20%234628%20merged-FFD21E?logo=huggingface&logoColor=black)](https://github.com/huggingface/lerobot/pull/4628)

I train and evaluate robot policies in simulation and on real arms (Isaac Sim, Isaac Lab, LeRobot, ROS 2 on Jetson). Then I write up what it took so someone else can reproduce it: the commands, the versions, what broke, and what the result does and doesn't show.

## Start here

<a href="https://github.com/Rahillasne/causal-confusion-driving"><img src="https://raw.githubusercontent.com/Rahillasne/causal-confusion-driving/main/results/figures/fig1_dissociation.png" alt="Three bar charts. The confounded policy scores higher validation accuracy than the original, yet gets a lower closed-loop driving score and is stuck at green lights about 22% of the time." width="100%"></a>

**[Causal confusion in imitation learning, reproduced](https://github.com/Rahillasne/causal-confusion-driving).** A NeurIPS 2019 result rebuilt from scratch on a laptop CPU: the policy that predicts the expert better drives worse. The README goes from install to every figure, with run times, 49 tests, a log of what failed along the way, and the limits of the result.

| Project | What it is | Try it |
|---|---|---|
| [orbit-eval](https://github.com/Rahillasne/orbit-eval) | A zero-dependency CLI that tells you whether a robot-policy change survived the noise. 403 tests. | `pip install orbit-eval`, then the [60-second quickstart](https://github.com/Rahillasne/orbit-eval#quickstart-60-seconds) |
| [Tanager Fieldguide](https://github.com/Rahillasne/tan-fieldguide) | Spectral search over Tanager-1's open hyperspectral archive: click a chip, find its lookalikes across 149 scenes. | [Open it in your browser](https://rahillasne.github.io/tan-fieldguide/). Nothing to install. |
| [ORBIT](https://github.com/Rahillasne/Orbit) | Dataset diagnostics for LeRobot: per-task capability scores and what to record next. | [Install from source](https://github.com/Rahillasne/Orbit#installation) |

## Open source

- **[huggingface/lerobot #4628](https://github.com/huggingface/lerobot/pull/4628)**, merged: success counts and 95% confidence intervals at every level of `lerobot-eval`, with docs and tests. Revised after the maintainer's AI-assisted review.
- **[NVIDIA/Isaac-GR00T #773](https://github.com/NVIDIA/Isaac-GR00T/issues/773)**: the RoboCasa README's results table can't come from its documented eval command (the percentages imply 20 or 200 episodes, not 10). Proposed a caption fix.

## Papers

Sole author.

- [Per-Task Regression Under Suite-Average Selection of Retrained Robot Policies](https://openreview.net/forum?id=DGjXgDszHR). CoRL 2026 Workshop (SPAIS).
- [The Noise Floor Beneath the Policy: How Evaluation Defaults Determine What Is Measurable](https://openreview.net/forum?id=tl7yt4nGpw). CoRL 2026 Workshop (WEBP).
- [Per-Task Retraining Noise in Robot Imitation Learning](https://openreview.net/forum?id=QXDem3bdVS). Preprint, 2026.

## Toolbox

Python · C++ · PyTorch · ROS 2 · NVIDIA Isaac Sim · Isaac Lab · LeRobot · Jetson · Docker · Linux · Google Cloud

---

Looking for a Summer 2027 internship in robotics, simulation or developer education.
