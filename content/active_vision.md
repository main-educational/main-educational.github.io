# Active vision with deep neural networks

**When:** Monday October 26th 2026, 13:00-14:45

## Overview

This workshop explores active vision in deep neural networks, moving beyond the standard passive setting in which models process entire images at once. We will begin with a brief introduction to supervised and self-supervised representation learning approaches such as JEPA, then connect these models to the active nature of biological vision, where information is acquired sequentially through selective sampling. We will introduce seqJEPA as a step toward active vision modeling by learning visual representations from sequences of observations, and examine how sampling strategies affect what is learned. Finally, we will show how a model can learn where to look and accomplish goals such as visual search. Along the way, we will discuss evaluation through downstream task performance, computational efficiency, and behavioral and neural similarity to biological vision.

## Instructors

:::::{grid} 1 2 2 2

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_motahareh_pourrahimi.jpg
:alt: Motahareh Pourrahimi
:width: 200px
:align: center
```
**[Motahareh Pourrahimi](https://mila.quebec/en/directory/motahareh-pourrahimi)**\
Mila and McGill University

<a href="mailto:motahareh.pourrahimi@mail.mcgill.ca"><img src="images/icons/email.svg" alt="Email" width="20"></a>&emsp;<a href="https://bsky.app/profile/motaharehpr.bsky.social"><img src="images/icons/bluesky.svg" alt="Bluesky" width="20"></a>&emsp;<a href="https://x.com/MotaharehPR"><img src="images/icons/x.svg" alt="X" width="20"></a>
:::
::::

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_hafez_ghaemi.jpg
:alt: Hafez Ghaemi
:width: 200px
:align: center
```
**[Hafez Ghaemi](https://hafezgh.github.io/)**\
Mila and Université de Montréal

<a href="mailto:hafez.ghaemi@umontreal.ca"><img src="images/icons/email.svg" alt="Email" width="20"></a>&emsp;<a href="https://bsky.app/profile/hafezghm.bsky.social"><img src="images/icons/bluesky.svg" alt="Bluesky" width="20"></a>&emsp;<a href="https://x.com/hafezghm"><img src="images/icons/x.svg" alt="X" width="20"></a>
:::
::::
:::::

**Motahareh Pourrahimi** is a PhD student at Mila and McGill University, working at the intersection of neuroscience and artificial intelligence in the Bashivan Lab. Her research focuses on understanding how neural systems generate behavior in ecologically grounded settings. In particular, she is interested in the cognitive processes and neural computations that support closed-loop perception and action, such as in free viewing visual search. Before joining McGill and Mila, she received her BSc in electrical engineering from the University of Tehran.

**Hafez Ghaemi** is a third-year PhD candidate at Mila and Université de Montréal. His research focuses on self-supervised learning and world modeling for perception and control, under the supervision of Eilif Muller and Shahab Bakhtiari. He holds MSc degrees in computer engineering from the University of Tehran and in data science and engineering from Politecnico di Torino, as well as a BSc in mechanical engineering with a minor in computer engineering from the University of Tehran.

## Objectives

 * Understand the motivation for active vision and how sequential visual sampling differs from standard passive vision models.
 * Explore how sampling strategies and learned fixation policies shape visual representations and enable tasks such as visual search.
 * Evaluate active vision models using downstream task performance, computational efficiency, and behavioral and neural similarity to biological vision.

## Materials

::::{grid}
:::{grid-item}
```{image} images/logo_pytorch.png
:alt: logo jupyter notebook
:class: bg-primary mb-1
:height: 150px
:align: center
```
{download}`Hands-on notebook (download) <materials/active_vision_seqjepa.ipynb>`
:::
::::

The notebook runs on a laptop CPU in a few minutes. Its first cell links to the data pack (`active_vision_data.zip`,
about 380 MB), which you unzip next to the notebook.
