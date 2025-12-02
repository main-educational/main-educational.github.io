# Videogames and reinforcement learning for neuroAI

## Overview

In this session you will learn how to train agents to act in complex environments using python and reinforcement learning (RL), and explore a rich neuroAI dataset that applies this class of model to characterize human behaviour and brain activity in a videogame environment.

## Instructors

::::{grid}
:::{grid-item}
![Yann Harel](https://cdn.bsky.app/img/avatar/plain/did:plc:twxrontuww4omebwkep6htas/bafkreihsejmz2zwfnbnssmh4cbwshylvflg6vxp4s7nfl3t7g7nkpbhmoy@jpeg)
[Yann Harel](https://scholar.google.com/citations?user=2K-2LacAAAAJ&hl=fr)
:::

::::{grid}
:::{grid-item}
![Hugo Delhaye](https://github.com/SIMEXP/simexp.github.io/blob/main/images/profile_hugo.jpg?raw=true)
[Hugo Delhaye](https://github.com/HugoDelhaye)
:::

:::{grid-item}
![Jean-Baptiste Bonin](images/empty_profile.png)
[Jean-Baptiste Bonin](https://github.com/bat0001)
:::

:::{grid-item}
![Julien Armand](https://avatars.githubusercontent.com/u/94652458?v=4)
[Julien Armand](https://github.com/JulienArmand1)
:::
::::

**Yann Harel** is a post-doctoral fellow in the SIMEXP laboratory in University of Montreal, working at the intersection of brain imaging, cognitive neuroscience and interactive environments. He is a  contributor to the Courtois Neuromod project, where he helped design and build  naturalistic neuroimaging datasets, linking real-time videogame behavior with fMRI, physiological and eye-tracking data. His research draws on large-scale open datasets, electrophysiology (EEG, MEG) and fMRI to study learning, attention and flow, as well as practical aspects of human-AI alignment. Beyond data collection, he develops open-source tools for scene-level segmentation, controller instrumentation, and BIDS-compliant pipelines used across multiple labs. He currently leads projects exploring how videogames and real-world tasks can serve as benchmarks for both neuroscience and AI.

**Hugo Delhaye** is a Master’s student in Psychology at Université de Montréal, co-supervised by Lune Bellec and Audrey Durand. His research combines behavioral data, artificial intelligence models, and video game simulations to compare how humans and artificial agents explore and learn from their environments.

**Jean-Baptiste Bonin** is a Master student in Computer Science ...

**Julien Armand** is a Master student in Computer Science ...

## Objectives

This session is divided into two parts:
### **training agents with RL**.
  * Learn the basics of reinforcement learning.
  * Discover the [Gym](https://github.com/openai/gym) environment which offers a standard interface to a variety of control tasks.
  * Implement a Deep Q Network to try and solve a simple control task called `cartpole`.
  * Evalute the quality of the agent behaviour

### **using RL agents for brain encoding**
  * learn the basics of brain encoding.
  * Discover the [cneuromod Mario dataset](https://docs.cneuromod.ca/en/latest/DATASETS.html#mario) which features about 84 hours of human gameplay and concurrent functional MRI recordings, collected on 5 participants.
  * Extract the latent representations of a pretrained RL agent.
  * Align the artificial and brain representations using ridge regression.
  * Evaluate the quality of the brain encoding.

## Materials

::::{grid}
:::{grid-item}
![colab logo](images/logo_colab.png)
[Colab notebooks for RL training](https://colab.research.google.com/drive/1SyD9gLEzpx0P3tKsl2_MYb4QmE5QkKMd#scrollTo=DZw_3OusqWWW)
:::

:::{grid-item}
![github logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
[Github repo for Mario tutorials](https://github.com/courtois-neuromod/mario.tutorials)
:::

::::
