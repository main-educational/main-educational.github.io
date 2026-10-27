# Alignment across modalities and across brains

:::{note}
The instructors for this session are confirmed. Session details may still change.
:::

**When:** Tuesday October 27th 2026

 * 13:00-13:50: talk by Aishwarya Agrawal, followed by questions
 * 14:00-16:00: hands-on tutorial with Elizabeth DuPre

## Overview

This session is about alignment: finding a common space in which different representations can be compared and combined. It covers two complementary problems.

**Aligning modalities.** Multimodal models learn to align representations of images and language, so that a model can describe what it sees or answer questions about an image. A 45-minute talk, followed by questions, will present how vision-language models achieve this alignment, and how to evaluate whether they truly ground language in vision.

**Aligning brains.** No two brains are organized exactly alike, and anatomical registration alone does not bring functional responses into correspondence. A two-hour hands-on tutorial will introduce functional alignment with [fmralign](https://fmralign.github.io/fmralign/), a Python library built on nilearn and scikit-learn that aligns brain activity across human participants, using methods such as Procrustes, shared response modeling and optimal transport.

## Instructors

:::::{grid} 1 2 2 2

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_aishwarya_agrawal.jpg
:alt: Aishwarya Agrawal
:width: 200px
:align: center
```
**[Aishwarya Agrawal](https://www.iro.umontreal.ca/~agrawal/index.html)**\
Université de Montréal and Mila
:::
::::

::::{grid-item}
:::{div}
:class: text-center
```{image} images/profile_elizabeth_dupre.jpg
:alt: Elizabeth DuPre
:width: 200px
:align: center
```
**[Elizabeth DuPre](https://elizabeth-dupre.com/)**\
Université de Montréal
:::
::::
:::::

**Aishwarya Agrawal** is an assistant professor in the Department of Computer Science and Operations Research (DIRO) at Université de Montréal, a Canada CIFAR AI Chair, and a core academic member of Mila. Her research lies at the intersection of computer vision, deep learning and natural language processing, with a focus on AI systems that can "see" and "talk".

**Elizabeth DuPre** is a postdoctoral fellow in the Department of Psychology at Université de Montréal. As a psychologist and computational neuroscientist, her work focuses on modeling individual brain activity across a range of cognitive states, and assessing how well these individualized models generalize. She is an active developer of open source Python tools for neuroimaging, including nilearn and fmralign, with a focus on the reproducibility of analysis workflows. She previously gave a keynote on aligning representations in brains and machines at MAIN educational 2022.

## Objectives

 * Understand how vision-language models align visual and linguistic representations.
 * Learn how to evaluate multimodal models, and the pitfalls of current benchmarks.
 * Learn the basics of functional alignment, and why anatomical alignment alone is not enough to compare brain activity across participants.
 * Align fMRI data across participants with fmralign, comparing methods such as Procrustes and optimal transport.
 * Build a group template, and evaluate alignment quality using inter-subject decoding.

## Materials

::::{grid} 1 2 3 3
:::{grid-item}
```{image} images/logo_gslides.png
:alt: Google Slides logo
:class: bg-primary mb-1
:height: 150px
:align: center
```
[Presentation slides by Aishwarya Agrawal](https://docs.google.com/presentation/d/18NVP5FZKoD1mqpV167Gqux6WosndwrftG5V6RcXPPSE/edit?usp=sharing)
:::

:::{grid-item}
```{image} images/logo_website.svg
:alt: Website icon
:class: bg-primary mb-1
:height: 150px
:align: center
```
[fmralign tutorial by Elizabeth DuPre](https://emdupre.github.io/MAIN2026-fmralign/)
:::

:::{grid-item}
```{image} images/logo_website.svg
:alt: Website icon
:class: bg-primary mb-1
:height: 150px
:align: center
```
[fmralign documentation and examples](https://fmralign.github.io/fmralign/)
:::
::::
