---
layout: default
title: Getting Started
nav_order: 2
---
This document provides some of the useful reading material and resource to help you get started with your research in our group.

As the field of theoretical and computational neuroscience is rapidly growing, it is becoming increasing hard to follow all the frontiers for newcomers. However, it is always rewarding to go back to read the classic literature in the field, especially the classic reviews on the milestones in the field. This document summarizes literature that are relevant to our current research topics and are more suitable for students in physics and mathematical background.

- [Reading list](#reading-list)
  - [Overview of the landscape](#overview-of-the-landscape)
  - [Neural Representation and Coding](#neural-representation-and-coding)
    - [Sensory coding](#sensory-coding)
    - [Population code](#population-code)
  - [Classic work in Theoretical and Computational Neuroscience](#classic-work-in-theoretical-and-computational-neuroscience)
    - [Perceptron](#perceptron)
    - [Hopfield model](#hopfield-model)
    - [Random Recurrent Neural Networks](#random-recurrent-neural-networks)
    - [Continuous Attractors Neural Networks](#continuous-attractors-neural-networks)
    - [Motion detection](#motion-detection)
    - [Computation through dynamics](#computation-through-dynamics)
  - [References](#references)


# Reading list

## Overview of the landscape
The following materials are accessible for general readers. To get a quick flavor of how the field has evolved over the years, you can't do better by starting reading the information on[2024 Brain Prize](https://lundbeckfonden.com/the-brain-prize/computational-theoretical-neuroscience-2024), which was awarded to the three giants in the field: Haim Sompolinsky, Larry Abbott, and Terry Sejnowski.

The popular information for the [Nobel Prize in physics 2024](https://www.nobelprize.org/prizes/physics/2024/popular-information/). If you want dive deeper to their contribution, see the [advanced information](https://www.nobelprize.org/uploads/2024/11/advanced-physicsprize2024-3.pdf).

Larry Abbott's review on the field of theoretical neuroscience. It is not very new, but still worth reading. 
- [L. F. Abbott. Theoretical neuroscience rising. Neuron, 60(3):489–495, 2008.](https://www.sciencedirect.com/science/article/pii/S0896627308008921)

The perspective paper by Sejnowskii, Koch and Churchland marked the birth of Computational Neuroscience.
- [T. J. Sejnowski, C. Koch, and P. S. Churchland. Computational neuroscience. Science, 241(4871):1299–1306, 1988.](https://www.science.org/doi/10.1126/science.3045969)


William Bialek has a recent account on John Hopfield's contribution to biological physics. So you can get a better idea about Hopfield's legendary career.
- [W. Bialek. Moving boundaries: An appreciation of John Hopfield. arXiv preprint arXiv:2412.18030, 2024.](https://arxiv.org/abs/2412.18030)

Hopfield also has memoroire-style articles, which are worth reading. In the [article](https://pni.princeton.edu/people/john-j-hopfield/now-what), he shared his view on how to choose research questions

## Neural Representation and Coding
### Sensory coding
The sensory systems are most extensively studied in neuroscience and several principles have been found. For example, the efficient coding hypothesis for InfoMax, Predictive coding, Information Bottleneck etc.

**Efficient Coding and InfoMax**
The earliest idea of efficient coding can be dated by to At. The formal definition is Horace Barlow in 1961 as a theoretical model of sensory neuroscience in the brain.
- Attneave, Fred (1954). "[Some informational aspects of visual perception](https://www.semanticscholar.org/paper/Some-informational-aspects-of-visual-perception.-Attneave/6d0198460198fdb49b89d1646049712b3a0683df)". Psychological Review. 61 (3): 183–93.
- Barlow, H. (1961) "[Possible principles underlying the transformation of sensory messages](https://www.cnbc.cmu.edu/~tai/microns_papers/Barlow-SensoryCommunication-1961.pdf)" in Sensory Communication, MIT Press.

The idea was further developed by Laughlin, Linsker in the form of *InfoMax*. The idea has been rigorously tested in early visual and auditory systems, providing a very useful framework to think about early sensory processing.
- Laughlin, Simon (1981). “[A simple coding procedure enhances a neuron’s information capacity](https://www.princeton.edu/~wbialek/rome/refs/laughlin_81.pdf)”.Zeitschrift für Naturforschung c 36.9-10, pages 910–912.
- Linsker, Ralph (1988). “[Self-Organization in a Perceptual Network](https://ieeexplore.ieee.org/document/36)”. In: Computer 21.3, pages 105–117.
- J. J. Atick. [Could information theory provide an ecological theory of sensory processing?](https://iopscience.iop.org/article/10.1088/0954-898X/3/2/009) Network: Computation in neural systems, 3(2):213–251, 1992.
- Lewicki, M.S. (2002). "[Efficient coding of natural sounds](https://www.nature.com/articles/nn831)". Nature Neuroscience. 5 (4): 356–363.

Similar idea, such as minimize the energy while optimize the information transmission has also been proposed.
- Laughlin, Simon B (2001). “[Energy as a constraint on the coding and processing of sensory information](https://pubmed.ncbi.nlm.nih.gov/11502395/)”.Current opinion in neurobiology 11.4, pages 475–480.
- V. Balasubramanian, D. Kimber, and M. J. Berry II. Metabolically efficient information processing. Neural computation, 13(4):799–815, 2001
- S. B. Laughlin, R. R. de Ruyter van Steveninck, and J. C. Anderson. The metabolic cost of neural information. Nature neuroscience, 1(1):36–41, 1998
- W. B. Levy and R. A. Baxter. Energy efficient neural codes. Neural computation, 8(3):531–543, 1996

**Physical Limit**
See Bialek’s Biophysics:searching for principles chapter 4.4. Here are a few examples
- W. Bialek. Physical limits to sensation and perception. Annual review of biophysics and biophysical chemistry, 16(1):455–478, 1987
- A. W. Snyder. Acuity of compound eyes: physical limitations and design. Journal of comparative Physiology, 116:161–182, 1977
- A. W. Snyder, D. G. Stavenga, and S. B. Laughlin. Spatial information capacity of compound eyes. Journal of Comparative Physiology, 116:183–207, 1977

**Predictive Coding**
-  R. L. Gregory. Perceptions as hypotheses. Philosophical Transactions of the Royal Society of London. B, Biological Sciences, 290(1038):181–197, 1980
- M. V. Srinivasan, S. B. Laughlin, and A. Dubs. Predictive coding: a fresh view of inhibition in the retina. Proceedings of the Royal Society of London. Series B. Biological Sciences, 216(1205):427–459, 1982.
- R. P. N. Rao and D. H. Ballard, Predictive coding in the visual cortex: a functional interpretation of some extra-classical receptive-field effects. Nature Neuro, 1999.
- T. S. Lee and D. Mumford. Hierarchical Bayesian inference in the visual cortex. JOSA A, 20(7):1434–1448, 2003

Reviews and Tutorials
- Y. Huang and R. P. Rao. Predictive coding. Wiley Interdisciplinary Reviews: Cognitive Science, 2011.
- R. Bogacz. A tutorial on the free-energy framework for modelling perception and learning. Journal of mathematical psychology, 2017.


### Population code
**Noise Correlation**
All biological systems are subject to noise, when talking about how neural population encode certain quantities, their noise correlation structure become relevant. Two of the review papers can give you a good idea about this subject.
- B. B. Averbeck, P. E. Latham, and A. Pouget. [Neural correlations, population coding and computation](https://www.nature.com/articles/nrn1888). Nature reviews neuroscience, 7(5):358–366, 2006
• S. Panzeri, M. Moroni, H. Safaai, and C. D. Harvey. [The structures and functions of correlations in neural population codes](https://www.nature.com/articles/s41583-022-00606-4). Nature Reviews Neuroscience, 23(9):551–567, 2022.

It has also becomes clear that the representational geometry is very import for coding and decoding. The review by Kriegeskorte and Wei showes this clearly.
- N. Kriegeskorte and X.-X. Wei. [Neural tuning and representational geometry](https://www.nature.com/articles/s41583-021-00502-3). Nature Reviews Neuroscience, 22(11):703–718, 2021.
  
A more recent review on representational geometry in the prefrontal cortex  by Tatiana Engel.
- [The dynamics and geometry of choice in the premotor cortex](https://www.nature.com/articles/s41586-025-09199-1)

## Classic work in Theoretical and Computational Neuroscience

### Perceptron
A perceptron is an abstract of a single-layer neural network first proposed by Rosenblatt. This is the prototype or simpliest network model.
- F. Rosenblatt. The perceptron: a probabilistic model for information storage and organization in the brain. Psychological review, 65(6):386, 1958.

The calculation of the capacity of a perceotron is due to the pioneering work by Gardner.  Using the "replica trick" developed in studying of disordered systems, such as the spin glass.
  - E. Gardner. Maximum storage capacity in neural networks. EPL (Europhysics Letters), 4(4):481, 1987

### Hopfield model
The Hopfield model is perhaps the most famous model in comp neuro. This network model was proposed to explain the mechanism of auto-associative memories. The early idea is due to Amari:
- S.-I. Amari. Learning patterns and pattern sequences by self-organizing nets of threshold elements. IEEE Transactions on computers, 100(11):1197–1206, 1972

Hopfield proposed a slightly different model which is now called Hopfield net:
-  J. J. Hopfield. Neural networks and physical systems with emergent collective computational abilities. Proceedings of the national academy of sciences, 79(8):2554–2558, 1982
- J. J. Hopfield. Neurons with graded response have collective computational properties like those of two-state neurons. Proceedings of the national academy of sciences, 81(10):3088–3092, 1984.

The capacity of the Hopfield model, namely, how many random patterns can a network store and then by retrieved by partial information, was calculated also via the "replica trick".
-  M. V. Tsodyks and M. V. Feigel’man. The enhanced storage capacity in neural networks with low activity level. EPL (Europhysics Letters), 6(2):101, 1988.
-  S. Fusi, P. J. Drew, and L. F. Abbott. Cascade models of synaptically stored memories. Neuron, 45(4):599–611, 2005


### Random Recurrent Neural Networks
One of the powerful methods to understand the dynamics of randomly recurrent neural networks (RNNs) is the *Dynamical Mean Field Theory* developped in the 80s.
- H. Sompolinsky, A. Crisanti, and H.-J. Sommers. Chaos in random neural networks. Physical review letters,61(3):259, 1988
- A. Crisanti and H. Sompolinsky. Path integral approach to random neural networks. Physical Review E, 98(6):062120, 2018

DMFT of RNNs with self-coupling
- M. Stern, H. Sompolinsky, and L. Abbott. Dynamics of random neural networks with bistable units. Physical Review E, 90(6):062710, 2014.

DMFT of RNNs with learning. This work consider the neural dynamcis and synaptic dynamics simultaneuosly.
- D. G. Clark and L. Abbott. Theory of coupled neuronal-synaptic dynamics. arXiv preprint arXiv:2302.08985, 2023

### Continuous Attractors Neural Networks
Continuous attractors neural networks (CANNs) have been proposed as a model for representing continuous variables in the brain, such as our head direction, location in a physical environment, and so on. They are among the most successful networks in neuroscience. See the review by Khona and Fiete.
- [Attractor and integrator networks in the brain](https://www.nature.com/articles/s41583-022-00642-0). Nature Reviews Neuroscience, 2022.

The line attractor was first proposed by Sabastian Seung to explain the ocular motor control.
- H. S. Seung. [How the brain keeps the eyes still]((https://www.pnas.org/doi/10.1073/pnas.93.23.13339)). Proceedings of the National Academy of Sciences, 93(23):13339–13344, 1996
-  H. S. Seung. Continuous attractors and oculomotor control. Neural Networks, 11(7-8):1253–1258, 1998

The first ring attractor models were proposed to explain both the head direction and the direction selectivity in the visual cortex.
- K. Zhang. Representation of spatial orientation by the intrinsic dynamics of the head-direction cell ensemble: a theory. Journal of Neuroscience, 16(6):2112–2126, 1996
- R. Ben-Yishai, R. L. Bar-Or, and H. Sompolinsky. Theory of orientation tuning in visual cortex. Proceedings of the National Academy of Sciences, 92(9):3844–3848, 1995.


### Motion detection
How does our eye perceive the movement of objects? The classic model is the Hassenstein-Reichardt model proposed to explain how the fly detect movement of objects in its visual field.
- B. Hassenstein and W. Reichardt. Systemtheoretische analyse der zeit-, reihenfolgen-und vorzeichenauswer-tung bei der bewegungsperzeption des rüsselkäfers chlorophanus. Zeitschrift für Naturforschung B, 11(9-
10):513–524, 1956
- W. Reichardt. Autocorrelation, a principle for evaluation of sensory information by the central nervous system. In Symposium on Principles of Sensory Communication 1959, pages 303–317. MIT press, 1961.

### Computation through dynamics
The idea that neural computation is fundamentally a dynamical process is due to Hopfield.
- J. J. Hopfield and D. W. Tank. Computing with neural circuits: A model. Science, 233(4764):625–633, 1986. 
- J. J. Hopfield and D. W. Tank. “Neural” computation of decisions in optimization problems. Biological cybernetics, 52(3):141–152, 1985.
- J. J. Hopfield, "Brain, neural networks, and computation", Review of Modern Physics, 71(2):431, 1999.



## References