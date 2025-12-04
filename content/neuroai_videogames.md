# Videogames and reinforcement learning for neuroAI

## Overview

In this session you will learn how to train agents to act in complex environments using python and reinforcement learning (RL), and explore a rich neuroAI dataset that applies this class of model to characterize human behaviour and brain activity in a videogame environment.

## Instructors

::::{grid}

:::{grid-item}
```{image} https://avatars.githubusercontent.com/u/94652458?v=4
:alt: profile
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Julien Armand](https://github.com/JulienArmand1)
:::

:::{grid-item}
```{image} images/profile_baptiste_bonin.jpg
:alt: profile
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Baptiste Bonin](https://github.com/bat0001)
:::

:::{grid-item}
```{image} https://github.com/SIMEXP/simexp.github.io/blob/main/images/profile_hugo.jpg?raw=true
:alt: profile
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Hugo Delhaye](https://github.com/HugoDelhaye)
:::

:::{grid-item}
```{image} images/profile_yann_harel.jpg
:alt: profile
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Yann Harel](https://scholar.google.com/citations?user=2K-2LacAAAAJ&hl=fr)
:::
::::

**Julien Armand** is a research Master’s student at Université Laval & Mila in Québec, Canada 🇨🇦. He completed a Bachelor’s degree in Mathematics at the University of Montreal, with a focus on statistics. His work centers on reinforcement learning in multi-agent environments, with a particular interest in how the nature of exploration shapes agent behavior in games blending cooperation and competition. He studies how exploration–exploitation strategies influence coordination and emergent dynamics, with the broader aim of understanding how independent agents adapt when their environment is shaped not only by uncertainty but also by the simultaneous decisions of others.

**Baptiste Bonin** is a research Master’s student at Université Laval & Mila in Québec, Canada 🇨🇦, working on machine learning with a strong interest in reinforcement learning, preference learning, and generative modeling. His current research explores recommendation systems through world models — ways of understanding users and their choices so that agents can learn by exploring realistic virtual environments. He leads a student team working on humanoid robotics 🤖, developing reinforcement learning approaches to teach autonomous skills and decision-making in realistic physical environments. Prior to that, he had a background in software engineering from his educational journey in France 🇫🇷.

**Hugo Delhaye** is a Master’s student in Psychology at Université de Montréal. His research combines behavioral data, artificial intelligence models, and video game simulations to compare how humans and artificial agents explore and learn from their environments.

**Yann Harel** is a post-doctoral fellow in the SIMEXP laboratory in University of Montreal, working at the intersection of brain imaging, cognitive neuroscience and interactive environments. He is a  contributor to the Courtois Neuromod project, where he helped design and build  naturalistic neuroimaging datasets, linking real-time videogame behavior with fMRI, physiological and eye-tracking data. His research draws on large-scale open datasets, electrophysiology (EEG, MEG) and fMRI to study learning, attention and flow, as well as practical aspects of human-AI alignment. Beyond data collection, he develops open-source tools for scene-level segmentation, controller instrumentation, and BIDS-compliant pipelines used across multiple labs. He currently leads projects exploring how videogames and real-world tasks can serve as benchmarks for both neuroscience and AI.

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
```{image} images/logo_colab.png
:alt: logo colab
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Colab notebooks for RL training](https://colab.research.google.com/drive/1SyD9gLEzpx0P3tKsl2_MYb4QmE5QkKMd#scrollTo=DZw_3OusqWWW)
:::

:::{grid-item}
```{image} https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
:alt: logo github
:class: bg-primary mb-1
:height: 200px
:align: center
```
[Github repo for Mario tutorials](https://github.com/courtois-neuromod/mario.tutorials)
:::

::::
