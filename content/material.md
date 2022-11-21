# Material

```{warning}
The descriptions and material below are provisional, and may be updated until Dec 1st 2022.
```

(material:supervised_learning)=
## Supervised learning using scikit-learn

### Instructor

**Nikhil Bhagwat, PhD** is an Academic Associate in the [ORIGAMI lab](https://neurodatascience.github.io/) (PI: [Dr. JB Poline](https://www.mcgill.ca/neuro/jean-baptiste-poline-phd)) at McGill University. He completed his PhD thesis on prognostic applications for Alzheimer’s disease using MR imaging and machine-learning (ML) techniques in the [CoBrA Lab](https://www.cobralab.ca/) (PI: [Dr. Mallar Chakravarty](http://cobralab.ca/members/commander/)) at the University of Toronto. Subsequently, he worked as a researcher at the University of Massachusetts and the Allen Institute. His current research interests include disease staging, subtyping, and prognosis using ML models, along with development of neuroinformatics tools for improving [reproducibility](https://github.com/neurodatascience/mr_proc) and [sustainability](https://neuropipelines.github.io/10carbon) of computational pipelines. 

### Objectives
  * Define machine-learning nomenclature
  * Describe basics of the “learning” process
  * Explain model design choices and performance trade-offs
  * Introduce model selection and validation frameworks
  * Explain model performance metrics

### Questions you will be able to answer after taking this module:
  * Model training - what is under/over-fitting?
  * Model selection - what is (nested) cross-validation?
  * Model evaluatation - what are type-1 and type-2 errors?
  
### Materials
[GitHub Link](https://github.com/neurodatascience/main-2021-ml-parts-1-2)

## Representational structure in neural time series using calcium imaging and electrophysiology

### Instructors
**Quinn Lee, PhD** is a CIHR/FRQ postdoctoral research fellow in the Brandon Lab at McGill University (Montreal, QC, Canada). Prior to joining the Brandon Lab, he completed my PhD at the University of Lethbridge (Lethbridge, AB, Canada) with Drs. Robert Sutherland and Robert McDonald studying how long-term memory is organized at the systems-level in the brain. His current work aims to understand how aspects of experience and memory are represented in neuronal population activity in the rodent hippocampus across protracted experience. To this end, he uses a combination of miniscope calcium imaging in freely moving animals, advanced behavioral tracking, and computational methods to explore questions about neuronal representation and behavior.

**Giuseppe P Gava, PhD** is a postdoctoral neuroscientist in the Dupret Lab at the MRC BNDU, University of Oxford. He was awarded a PhD from the Centre for Doctoral Training in Neurotechnology at Imperial College London, where he also graduated in Biomedical Engineering. He aims to use concepts from network science, topology and information theory to understand the complex neural circuitry and dynamics that shape memory and cognition.

### Objectives
 * Data analysis for in vivo calcium imaging time series from freely-behaving animals
 * Data analysis for electrophysiological time series from freely-behaving animals
 * Compare representation in neural data to theoretical models with representational similarity analysis (RSA) and manifold-based analyses
 * Assess the co-firing structure and topology of neuronal networks and compare them using Riemannian metrics.

### Materials
[GitHub link to ephys material](https://github.com/drsax93/cofiringTopology)

## Keynote Patrick Mineault

**Patrick Mineault, PhD** is a neurotechnologist and CEO of xcorr consulting. His career spans academia and industry: he was a data scientist at Google, research scientist at Meta on brain-computer-interfaces, founder of a medtech startup and founding CTO of the educational nonprofit Neuromatch. His research at the intersection of neuroscience and AI has been published in NeurIPS, Neuron, PNAS, J Neurosci and Plos Comp Bio. He is the author of the Good Research Code Handbook and writes a popular computational neuroscience blog, [xcorr.net](https://xcorr.net/). He obtained his PhD in computational neuroscience at McGill University.

**Title**: What's the endgame of neuroAI?

**Summary**: Neuroscience and AI have a long, intertwined history. Artificial intelligence pioneers looked to the principles of the organization of the brain as inspiration to make intelligent machines. In a surprising reversal, AI is now helping us understand its very source of inspiration: the human brain. Over the next decade, we’ll make ever more precise in silico brain models. As a result, we’ll soon be able to download and use sensory models, on demand, with the same convenience that we can do object recognition or natural language processing.

In this talk, I will take you on a tour of the near future. I will argue that we should use this newfound capability to help improve human health, both for people with neurological disorders and to enhance the well. I discuss enabling technological trends: advances in AI, industrial use cases, AR/VR and BCI. I invite everyone to reflect on the role of innovation and academia to help humans flourish.

## Introduction to deep learning using Pytorch

### Instructors
Mohammad Yaghoubi, Thomas Jiralerspong and Krystal Pan

### Objectives
 * Understand basic concepts in deep learning
 * Discover the pytorch interface to build artificial neural networks
 * Train a basic model using pytorch

### Materials
The training material is adapted from NeuroMatch Academy.
[Google collab Link](https://colab.research.google.com/drive/1Arf7Ydg1VjNx5wv9IOI5xTCYbQ5Djo-7?usp=sharing)

## Machine learning in functional MRI using [Nilearn](https://nilearn.github.io)

### Instructors
**Yasmin Mzayek** obtained her Master's in Brain and Cognitive Sciences from the University of Amsterdam. During this time she did an internship at the Netherlands Cancer Institute in Amsterdam and worked on analyzing diffusion-weighted imaging data. Then she went to Aix Marseille University to work on pulse sequence programming for diffusion MR spectroscopy as well as processing and analysis of data from this modality. She also worked as scientific programmer and data scientist at the University of Groningen. Currently, she is a research engineer at INRIA working on maintaining the Nilearn Python toolkit.

**Hao-Ting Wang, PhD** is a IVADO postdoctoral fellow at CRIUGM. Her project focuses on discovery of transdiagnostic brain biomarkers amongst neurodegenerative conditions from multiple open access datasets. Her expertise lies in fMRI data processing, functional connectivity, and data workflow construction. She is also a core developer of Nilearn with a focus on fMRI data processing and feature extraction.

### Objectives
 * Understand the structure of functional magnetic resonance imaging data.
 * Generate correlation matrices using fMRI time series (aka "connectomes").
 * Visualize brain maps and connectomes.
 * Train machine learning models to classify subjects by age groups based on brain connectivity.

### Materials
[Github Link](https://github.com/main-educational/intro_ML)
[Jupyter Book Link](https://main-educational.github.io/intro_ML/intro.html)

## Keynote Elizabeth Dupre

**Elizabeth Dupre, PhD** is a [Wu Tsai interdisciplinary postdoctoral research fellow](https://neuroscience.stanford.edu/people/elizabeth-dupre) at Stanford University, working between Prof. Russ [Poldrack](https://poldracklab.stanford.edu/) and Prof. Scott [Linderman](https://web.stanford.edu/~swl1/). As a psychologist and computational neuroscientist, her work focuses on modeling individual brain activity across a range of cognitive states—and assessing the generalizability of these individualized models—by extending statistical methods for human neuroimaging data analysis. Through her work, Dr DuPre has taken an active role developing tools in the open source Python ecosystem, with a focus on improving the reproducibility of analysis workflows.

**Title**: Aligning representations in brains and machines

**Summary**: Computational neuroscience is focused on uncovering general organizational principles supporting neural activity and behavior; however, uncovering these principles relies on making appropriate comparisons across individuals. This presents a core technical and conceptual challenge, as individuals differ along nearly every relevant dimension: from the number of neurons supporting computation to the exact computation being performed. Similarly in artificial neural networks, multiple initializations of the same architecture—on the same data—may recruit non-overlapping hidden units, complicating direct comparisons of trained networks.

In this talk, I will introduce techniques for aligning representations in both brains and in machines. I will argue for the importance of considering alignment methods in developing a comprehensive science at the intersection of artificial intelligence and neuroscience that reflects our shared goal of understanding principles of computation. Finally, I will consider current applications and limitations of these techniques, discussing relevant future directions for this area.


## Model selection and validation

### Instructor

Jérôme Dockes

### Objectives
 * Understand how to evaluate the performance of machine learning models.
 * Learn about hyperparameters and model selection.
 * Learn about pitfalls when validating machine learning models and how to easily avoid them using scikit-learn.

### Materials
[GitHub Link](https://github.com/neurodatascience/main-2021-ml-parts-1-2)

## Introduction to electro- and magneto-encephalography using [MNE-python](https://mne.tools/stable/index.html)

### Instructor
Alexandre Gramfort

### Objectives
 * Understand the structure of electro- and magneto-encephalography data.
 * Prepare and visualize MEG brain activity
 * Train machine learning models on MEG data

### Materials
TBA

## Brain decoding
### Instructors
Dr Peer Herholz

## Objectives
 * Understand the principles of brain decoding
 * Use ridge regression for brain encoding using features of a pretrained artificial neural network in functional magnetic resonance imaging
 * Use searchlight for brain decoding with multiple stimuli category
 * Use deep graph neural networks for brain decoding with multiple stimuli category.

## Materials

[Jupyter book link](https://main-educational.github.io/brain_encoding_decoding/); [Github Link](https://github.com/main-educational/brain_encoding_decoding)

## Brain encoding
### Instructors
Dr Isil Bilgin, Mr Alexandre Pasquiou and Mr Pravish Sainath

## Objectives
 * Understand the principles of brain encoding
 * Use ridge regression to encode brain activity in functional magnetic resonance imaging using direct representation of visual stimuli
 * Use ridge regression to encode brain activity in functional magnetic resonance imaging during a movie watching task using a large artificial language network

## Materials

[Jupyter book link](https://main-educational.github.io/brain_encoding_decoding/); [Github Link](https://github.com/main-educational/brain_encoding_decoding)
[Github repository](https://github.com/jashna14/DL4Brain)
