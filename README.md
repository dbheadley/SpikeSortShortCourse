# **Spike Sorting Short Course**

## Overview

The goal of this short course is to provide an introduction to key concepts, both analytical and practical, for analyzing extracellularly recorded action potentials. This is a rich topic. It has a long history, stretching back to the first recordings of 'unit' activities in the mid-Twentieth century. And it has new horizons, with advances in machine learning and biophysical simulation offering fundamentally new insights.

**We will not discuss any of that heady stuff (maybe another day).** Instead, we will stay in the present and cover how to do *spike sorting*. Spike sorting is the process of detecting extracellularly recorded action potentials and assigning them to groups based on their properties. From this, we conclude whether each group reflects an artifact, multiple neurons, or a single neuron. Sometimes we even infer the type of neuron. Since this is an early step in the processing of neural data, it affects all subsequent analyses. Thus, it is important.

Given its importance, it is surprising how most of us learn it. Some learn spike sorting from a colleague or mentor, using their preferred software and adopting their interpretive biases. Others cobble together code and heuristics based on some papers they read. Both approaches produce blind spots.

The goal of this short course is to take the best of both approaches. We will explore spike sorting together, with experienced practitioners from multiple backgrounds offering unique insights. In addition, we will read papers and look over code for a thorough and grounded treatment of technical aspects.

## Meeting topics

We will cover four topics that should provide a sufficient understanding of spike sorting. Each meeting will be centered around a discussion of  two or three relevant papers.

1. **Basic algorithms and current issues:** We will discuss how spike sorting was performed for most of the last 30 years. The algorithms discussed here are still widely used and help frame the various problems that can arise with spike sorting. We will also touch on recent advances in recording electrodes that have overwhelmed this approach.
    - *A review of methods for spike sorting: the detection and classification of neural action potentials.* [link](http://www.stat.columbia.edu/~liam/teaching/neurostat-fall17/papers/EM/Lewicki-Network-98_1.pdf)
    - *Continuing progress of spike sorting in the era of big data.* [link](https://www.sciencedirect.com/science/article/pii/S0959438818301375)
2. **Kilosort and high-density silicon probes:** Electrodes with hundreds of closely spaced sites require new algorithms for spike sorting. Kilosort has become one of the more popular packages for this, so we will examine how it works.
    - *Kilosort: realtime spike-sorting for extracellular electrophysiology with hundreds of channels* [link](https://www.biorxiv.org/content/biorxiv/early/2016/06/30/061481.full.pdf)
    - *Neuropixels 2.0: A miniaturized high-density probe for stable, long-term brain recordings* [link](https://www.science.org/doi/10.1126/science.abf4588)
3. **Quality control metrics:** The quality of spike groups can be evaluated for strength over background noise, distinctiveness from other groups, and consistency with arising from a single neuron. We will cover multiple metrics for evaluating these.
    - *Accuracy of Tetrode Spike Separation as Determined by Simultaneous Intracellular and Extracellular Measurements* [link](https://journals.physiology.org/doi/full/10.1152/jn.2000.84.1.401)
    - *Quality Metrics to Accompany Spike Sorting of Extracellular Signals* [link](https://www.jneurosci.org/content/31/24/8699.short)
    - *Quantitative measures of cluster quality for use in extracellular recordings* [link](https://www.sciencedirect.com/science/article/pii/S0306452204008425?via%3Dihub)
4. **Interpreting spike waveforms** Spikes from single neurons reflect their transmembrane currents and orientation and distance from the recording electrodes. These can systematically
    - *On the Origin of the Extracellular Action Potential Waveform: A Modeling Study* [link](https://journals.physiology.org/doi/full/10.1152/jn.00979.2005)
    - *Characterization of neocortical principal cells and interneurons by network interactions and extracellular features* [link](https://journals.physiology.org/doi/full/10.1152/jn.01170.2003)
