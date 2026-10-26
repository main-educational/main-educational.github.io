# World models and embodied agents

:::{note}
The instructors for this session are confirmed. Session details may still change.
:::

**When:** Monday October 26th 2026

 * 09:05-09:50: lecture by Sonia Joseph, followed by questions
 * 10:05-12:05: hands-on tutorial with Glen Berseth: *Building World Models from the Ground Up*

## Overview

This session opens the "reasoning about the world" day. A 45-minute lecture, followed by questions, introduces world models: AI systems that learn to predict how their environment evolves, and to use these predictions to perceive, plan and act. The lecture will focus on video world models such as V-JEPA, and on what interpretability methods reveal about how they represent physical structure. It is followed by a two-hour hands-on tutorial, *Building World Models from the Ground Up*:

> World models have become a popular tool for building predictive models and using them inside algorithms across many applications. But which world model should you use? The answer depends on the data you have, your objectives, and where the technology is heading. In this tutorial, we build the main world models in use today from the ground up. We cover forward dynamics models that predict future frames, latent models that predict future embeddings, and world action models that predict actions alongside the future, all trained on the same robot data.

## Instructors

:::::{grid} 1 2 2 2

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_sonia_joseph.jpg
:alt: Sonia Joseph
:width: 200px
:align: center
```
**[Sonia Joseph](https://soniajoseph.github.io/)**\
McGill University and Mila
:::
::::

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_glen_berseth.png
:alt: Glen Berseth
:width: 200px
:align: center
```
**[Glen Berseth](https://www.fracturedplane.com/)**\
Université de Montréal and Mila
:::
::::
:::::

**Sonia Joseph** is an AI researcher working on interpretable video world models, and a PhD student at McGill University and Mila. She conducted research on the JEPA team at Meta, where she also led the company's internal interpretability community, and published the first mechanistic interpretability work on physical reasoning in video world models such as V-JEPA 2. She is also a developer of Prisma, an open source toolkit for mechanistic interpretability in vision and video models.

**Glen Berseth** is an associate professor in the Department of Computer Science and Operations Research (DIRO) at Université de Montréal, a core academic member of Mila, and a Canada CIFAR AI Chair. He co-directs the Robotics and Embodied AI Lab (REAL). His research uses deep reinforcement learning to build generalist robots that learn from real-world, sequential decision making. He will lead the hands-on tutorial.

## Objectives

 * Understand what a world model is, and how world models are learned from data.
 * Discover how world models support perception, prediction and planning in artificial and biological agents.
 * Learn how interpretability methods can reveal how video world models represent physics.
 * Build and compare forward dynamics, latent and world action models on the same robot data.

## Materials

::::{grid}
:::{grid-item}
```{image} https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
:alt: logo github
:class: bg-primary mb-1
:height: 150px
:align: center
```
[Github repo for the world models tutorial (mini-wm)](https://github.com/milarobotlearningcourse/mini-wm)
:::

:::{grid-item}
```{image} images/logo_colab.png
:alt: logo colab
:class: bg-primary mb-1
:height: 150px
:align: center
```
[Colab notebook for the tutorial](https://colab.research.google.com/github/milarobotlearningcourse/mini-wm/blob/main/mini_wm_tutorial.ipynb)
:::

::::
