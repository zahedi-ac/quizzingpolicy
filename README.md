# Personalized Question Selection Using Reinforcement Learning

This repository contains the research implementation accompanying the paper:

**"Towards Intelligent Assessment: Using Reinforcement Learning Algorithms to Improve Accuracy and Efficiency in Online Educational Systems"**

The project investigates the use of **Reinforcement Learning (RL)** algorithms for personalized question selection in online educational assessment systems.

The main objective is to investigate whether an RL-based policy can select questions adaptively according to the needs and abilities of individual students, improving the accuracy and efficiency of knowledge assessment.

---

## Research Context

Traditional online assessments often rely on fixed question sequences or predefined testing strategies. Such approaches may not adequately account for differences in students' knowledge and abilities.

This research formulates personalized question selection as a **Reinforcement Learning problem**, where an agent selects questions based on the current assessment state and receives feedback from student responses.

The general interaction can be represented as:

```text
Student Knowledge State
          │
          ▼
     RL Agent
          │
          ▼
   Select Next Question
          │
          ▼
    Student Response
          │
          ▼
       Reward
          │
          ▼
 Update Assessment State
          │
          └──────────────► Select Next Question
```

---

## Research Objective

The study investigates the applicability of reinforcement learning algorithms to personalized and adaptive educational assessment.

The main objectives are:

* Investigating reinforcement learning for personalized question selection.
* Comparing different reinforcement learning and dynamic programming approaches.
* Studying the effect of reward functions and discount factors.
* Evaluating the ability of different algorithms to improve assessment accuracy.
* Exploring the potential of adaptive assessment in online educational environments.
* Identifying limitations and challenges in applying reinforcement learning to educational assessment.

---

## Algorithms

The repository contains implementations and experiments involving several reinforcement learning and dynamic programming methods:

| Method             | Type                         |
| ------------------ | ---------------------------- |
| Q-Learning         | Temporal-Difference Learning |
| SARSA              | Temporal-Difference Learning |
| Expected SARSA     | Temporal-Difference Learning |
| Double Q-Learning  | Temporal-Difference Learning |
| Bellman            | Dynamic Programming          |
| Bellman Optimality | Dynamic Programming          |
| Value Iteration    | Dynamic Programming          |
| Random             | Baseline                     |

Each method is implemented as a separate Jupyter Notebook.

---

## Repository Structure

```text
quizzingpolicy/
│
├── 1-Q-learning.ipynb
├── 2-SARSA.ipynb
├── 3-Expected SARSA.ipynb
├── 4-Double Q-learning.ipynb
├── 5-Bellman.ipynb
├── 6-Bellman-Optimality.ipynb
├── 7-Value-Iteration-Update-Rule.ipynb
└── 8-Random.ipynb
```

The notebooks provide the experimental implementations of the algorithms investigated in the study.

---

## Main Result

Among the evaluated approaches, **Value Iteration achieved the highest reported accuracy of 0.521** in the experiments presented in the paper.

This result suggests that dynamic programming approaches such as Value Iteration can be useful for personalized question selection under the experimental setting considered in this study.

> Note: The reported results correspond to the experimental setup and dataset used in the associated publication.

---

## Research Area

This project is related to the following research areas:

* Reinforcement Learning
* Machine Learning
* Artificial Intelligence
* Educational Artificial Intelligence
* Personalized Learning
* Adaptive Assessment
* Intelligent Tutoring Systems
* Educational Data Mining
* Online Learning Systems

---

## Publication

This repository is associated with the following publication:

**Zahra Zahedi, Takhtem Ghaffarian**

**"Towards Intelligent Assessment: Using Reinforcement Learning Algorithms to Improve Accuracy and Efficiency in Online Educational Systems"**

Computer Group, Khayyam University, Mashhad, Iran.

Publication page:

https://civilica.com/doc/2353699/

---

## Reproducibility

The experiments are provided as Jupyter Notebooks.

To use the notebooks, clone the repository and install the required Python dependencies.

```bash
git clone https://github.com/zahedi-ac/quizzingpolicy.git
cd quizzingpolicy
```

Then open the notebooks using Jupyter Notebook or JupyterLab.

```bash
jupyter notebook
```

> The exact experimental environment and dependencies may depend on the notebook and dataset configuration.

---

## Dataset

The dataset used in the research is not included in this repository.

Users interested in reproducing the experiments should obtain the dataset from its original source and comply with the applicable dataset terms and conditions.

---

## Limitations

The results presented in this repository should be interpreted within the experimental setting of the associated research.

Potential limitations include:

* Dependence on the characteristics of the educational dataset.
* Sensitivity to reward design and discount factors.
* Limitations of the state and action representations.
* Computational limitations of tabular reinforcement learning methods for larger state spaces.
* Challenges associated with modeling student knowledge dynamically.

These limitations provide opportunities for future research using more advanced reinforcement learning approaches.

---

## Future Research

Possible extensions of this work include:

* Deep Reinforcement Learning approaches such as Deep Q-Networks (DQN).
* Policy-gradient methods.
* Proximal Policy Optimization (PPO).
* More sophisticated student knowledge representations.
* Larger and more diverse educational datasets.
* Statistical comparison across multiple experimental runs.
* More extensive evaluation of reward functions and discount factors.
* Comparison with additional adaptive testing baselines.

---

## Authors

**Zahra Zahedi**
Computer Group, Khayyam University, Mashhad, Iran

**Takhtem Ghaffarian**
Computer Group, Khayyam University, Mashhad, Iran

