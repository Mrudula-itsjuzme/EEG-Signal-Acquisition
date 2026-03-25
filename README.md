# EEG Signal Acquisition and Analysis Project

## Overview

This project focuses on the acquisition of **EEG (Electroencephalography)** signals from human subjects under varying conditions and analyzing how brain activity changes across those conditions.

EEG signals are highly sensitive, non-stationary, and prone to noise. This project aims to study:

- How EEG signals behave under different physiological and environmental conditions
- How external and internal factors influence signal quality and interpretation
- Methods to acquire, preprocess, and analyze EEG data effectively

---

## Objectives

- Acquire EEG signals from subjects under controlled and varying conditions
- Study the variability of EEG signals across:
  - Cognitive states
  - Physical conditions
  - Environmental factors
- Identify patterns in EEG frequency bands (**Alpha, Beta, Theta, Delta**)
- Understand the impact of noise and artifacts on signal quality
- Implement preprocessing techniques to improve signal clarity
- Perform comparative analysis between different experimental conditions
- Build a foundation for applications like:
  - Brain-Computer Interfaces (BCI)
  - Cognitive state monitoring
  - Neurofeedback systems

---

## Literature Review

The following papers form the core of the literature review for this project, spanning hardware design, signal processing, preprocessing, source localization, machine learning, and clinical applications. Each paper was selected to provide both theoretical grounding and practical relevance to the experimental work planned.

---

### Paper 1 — A Review of EEG Acquisition, Processing and Application

| Field | Detail |
|-------|--------|
| **Source** | IOP Conference Series: Journal of Physics: Conference Series |
| **Year** | 2021 |
| **Link** | [https://iopscience.iop.org/article/10.1088/1742-6596/1907/1/012045](https://iopscience.iop.org/article/10.1088/1742-6596/1907/1/012045) |

**Summary:**
If you're just getting started with EEG research, this paper is a great first read. It gives a broad overview of how EEG signals are acquired, processed, and applied — covering everything from noise challenges and artifact handling to feature extraction techniques. The authors also look ahead at where AI is likely to take the field, making it a solid foundational reference for understanding the full pipeline.

---

### Paper 2 — Electroencephalography Signal Processing: A Comprehensive Review

| Field | Detail |
|-------|--------|
| **Source** | Sensors (MDPI) |
| **Year** | 2023 |
| **Link** | [https://www.mdpi.com/1424-8220/23/14/6434](https://www.mdpi.com/1424-8220/23/14/6434) |

**Summary:**
This one digs deeper into the technical side of the EEG processing pipeline. It walks through acquisition hardware, preprocessing methods like filtering and artifact removal, various feature extraction approaches, and how machine learning is being applied for classification. It's a well-organized reference if you need to understand how each stage connects to the next.

---

### Paper 3 — Miniaturization for Wearable EEG Systems: Recording Hardware and Data Processing

| Field | Detail |
|-------|--------|
| **Source** | Biomedical Engineering Letters |
| **Year** | 2022 |
| **Link** | [https://link.springer.com/article/10.1007/s13534-022-00232-0](https://link.springer.com/article/10.1007/s13534-022-00232-0) |

**Summary:**
As EEG moves out of the lab and into the real world, hardware needs to shrink. This paper looks at the engineering challenges behind making that happen — covering compact amplifiers, electrode design for wearables, and ASIC-based signal processing. It also discusses in-ear EEG and onboard artifact rejection, which is particularly relevant for portable acquisition systems like the one in this project.

---

### Paper 4 — A Portable EEG Signal Acquisition System and Limited-Electrode Classification Network for SSVEP

| Field | Detail |
|-------|--------|
| **Source** | Frontiers in Neurorobotics |
| **Year** | 2025 |
| **Link** | [https://www.frontiersin.org/journals/neurorobotics/articles/10.3389/fnbot.2024.1502560/full](https://www.frontiersin.org/journals/neurorobotics/articles/10.3389/fnbot.2024.1502560/full) |

**Summary:**
This paper presents a practical, working prototype: a 10-channel dry-electrode EEG headset built on a ROS-based platform, paired with a channel-attention neural network for SSVEP-based BCI tasks. What's interesting here is the combination of hardware portability and a custom classification network (SEMSCS) that performs well even with limited channels — something directly applicable when designing constrained acquisition setups.

---

### Paper 5 — A Systematic Review of Techniques for Artifact Detection in EEG from Wearable Devices

| Field | Detail |
|-------|--------|
| **Source** | Sensors |
| **Year** | 2025 |
| **Link** | [https://www.mdpi.com/1424-8220/25/18/5770](https://www.mdpi.com/1424-8220/25/18/5770) |

**Summary:**
Artifacts are one of the biggest headaches in real-world EEG recording, especially with wearables. This systematic review surveys the main techniques used to detect and remove them — wavelet filtering, ICA, Artifact Subspace Reconstruction (ASR), and supervised learning approaches. It gives a clear sense of where each method works best and where the field is heading with deep learning-based cleaning.

---

### Paper 6 — AnEEG: Leveraging Deep Learning for Effective Artifact Removal in EEG Data

| Field | Detail |
|-------|--------|
| **Source** | Scientific Reports |
| **Year** | 2024 |
| **Link** | [https://www.nature.com/articles/s41598-024-75091-z](https://www.nature.com/articles/s41598-024-75091-z) |

**Summary:**
Rather than just reviewing artifact removal, this paper actually proposes a new deep learning model — called AnEEG — specifically designed to clean EEG data contaminated by eye movements and muscle activity. Benchmarked against traditional wavelet denoising, it shows notable improvements in RMSE and SNR, making it a strong candidate for inclusion in any preprocessing pipeline aimed at signal quality.

---

### Paper 7 — A Systematic Review of EEG Source Localization Techniques and Their Applications

| Field | Detail |
|-------|--------|
| **Source** | Journal of Neuroscience Methods |
| **Year** | 2020 |
| **Link** | [https://www.sciencedirect.com/science/article/pii/S0165027020301631](https://www.sciencedirect.com/science/article/pii/S0165027020301631) |

**Summary:**
Once you have clean EEG data, the next question is: where in the brain is it coming from? This paper reviews the main computational methods for answering that — from dipole fitting to distributed inverse solutions. It also covers how these techniques are being applied to diagnose brain disorders, providing a good grounding in source imaging theory before getting into more recent applied work.

---

### Paper 8 — Evaluation of EEG Pre-processing and Source Localization in Ecological Research

| Field | Detail |
|-------|--------|
| **Source** | Frontiers in Neuroimaging |
| **Year** | 2025 |
| **Link** | [https://www.frontiersin.org/articles/10.3389/fnimg.2025.1479569/full](https://www.frontiersin.org/articles/10.3389/fnimg.2025.1479569/full) |

**Summary:**
This paper tackles something genuinely tricky: can you do reliable source reconstruction in natural, real-world EEG experiments — without individual MRI scans? Using template-based eLORETA, the authors show you can still get meaningful results separating visual and cognitive workload activations even without individual MRI. It's a practically useful reference for projects where full neuroimaging data isn't available.

---

### Paper 9 — Efficient Feature Extraction for EEG-Based Classification: A Comparative Review of Deep Learning Models

| Field | Detail |
|-------|--------|
| **Source** | AI (MDPI) |
| **Year** | 2024 |
| **Link** | [https://www.mdpi.com/2673-2688/7/2/50](https://www.mdpi.com/2673-2688/7/2/50) |

**Summary:**
With so many deep learning architectures out there, it's genuinely useful to have a systematic comparison. This paper reviews 88 models — CNNs, RNNs, and Transformer variants — specifically for EEG feature extraction and classification. The key takeaway: compact CNNs offer the best efficiency-to-performance ratio, while hybrid models and Transformers handle long-range temporal patterns better, at the cost of higher compute.

---

### Paper 10 — Deep Learning-Based EEG Emotion Recognition: Current Trends and Future Perspectives

| Field | Detail |
|-------|--------|
| **Source** | Frontiers in Psychology |
| **Year** | 2023 |
| **Link** | [https://www.frontiersin.org/articles/10.3389/fpsyg.2023.1126994/full](https://www.frontiersin.org/articles/10.3389/fpsyg.2023.1126994/full) |

**Summary:**
Emotion recognition from EEG is one of the more challenging application domains, partly because of how subjective and variable emotional responses are. This review covers the deep learning approaches that have been applied to the problem — including DBNs, CNNs, and RNNs — along with commonly used datasets and evaluation practices. Useful for understanding what's realistic when designing emotion-related EEG experiments.

---

### Paper 11 — Epileptic Seizure Detection Using Machine Learning: A Systematic Review and Meta-Analysis

| Field | Detail |
|-------|--------|
| **Source** | Brain Sciences |
| **Year** | 2025 |
| **Link** | [https://www.mdpi.com/2076-3425/15/6/634](https://www.mdpi.com/2076-3425/15/6/634) |

**Summary:**
Seizure detection is one of the most clinically significant EEG applications, and this meta-analysis gives a rigorous look at how well current ML methods perform across 60 studies and 93 datasets. The pooled results — around 96% sensitivity and 97% specificity — are impressive, though the paper also flags important questions around generalizability and evaluation standards that still need addressing.

---

### Paper 12 — Toward Multi-Dimensional Depression Assessment Using EEG-Based Machine Learning

| Field | Detail |
|-------|--------|
| **Source** | Brain Sciences |
| **Year** | 2026 |
| **Link** | [https://www.mdpi.com/2076-3425/16/2/139](https://www.mdpi.com/2076-3425/16/2/139) |

**Summary:**
This is one of the most recent papers in the set and explores using EEG functional connectivity features — coherence, phase-lag index, Granger causality — to both classify and measure depression severity. Using KNN and ANN models, the authors report around 97.7% classification accuracy and strong regression fits for severity, suggesting EEG could support more nuanced mental health assessment in the future.

---

### Paper 13 — The EEG Analysis and Identification of Alzheimer's Disease: A Review

| Field | Detail |
|-------|--------|
| **Source** | Frontiers in Aging Neuroscience |
| **Year** | 2025 |
| **Link** | [https://www.frontiersin.org/articles/10.3389/fnagi.2025.1686628/full](https://www.frontiersin.org/articles/10.3389/fnagi.2025.1686628/full) |

**Summary:**
Alzheimer's disease is notoriously difficult to detect early, and EEG biomarkers offer a non-invasive path worth exploring. This meta-analysis of 141 studies surveys EEG-based approaches for identifying AD and mild cognitive impairment — reviewing signal features, preprocessing choices, and ML classifiers. It's a comprehensive entry point into EEG's potential role in neurodegenerative disease monitoring.

---

### Paper 14 — Design Decisions for Wearable EEG Systems to Detect Motor Imagery

| Field | Detail |
|-------|--------|
| **Source** | Sensors |
| **Year** | 2024 |
| **Link** | [https://www.mdpi.com/1424-8220/24/15/4763](https://www.mdpi.com/1424-8220/24/15/4763) |

**Summary:**
There are a lot of variables to juggle when designing a wearable EEG system — electrode count, placement, sampling frequency, signal processing approach. This paper goes through those trade-offs specifically in the context of motor imagery BCI. One practical finding: sampling at 1 kHz or higher with as few as 1–3 well-placed electrodes can still yield stable classification, which has direct implications for experimental setup design.

---

### Paper 15 — Dry EEG Electrodes: A Review of Design for Brain-Computer Interface Applications

| Field | Detail |
|-------|--------|
| **Source** | Sensors |
| **Year** | 2014 |
| **Link** | [https://www.mdpi.com/s140/7/12847](https://www.mdpi.com/1424-8220/14/7/12847) |

**Summary:**
A bit older, but still highly cited and relevant. This review covers the landscape of dry electrode designs — contact and non-contact types — and evaluates their suitability for BCI use. It notes the lack of standardized testing across different electrode types, a gap that the field has only partially closed since. Worth reading as background before choosing electrodes for a portable or wearable EEG system.

---

### Paper 16 — Wearable EEG Electronics for a Brain–AI Closed-Loop System

| Field | Detail |
|-------|--------|
| **Source** | NPJ Flexible Electronics |
| **Year** | 2022 |
| **Link** | [https://www.nature.com/articles/s41528-022-00164-w](https://www.nature.com/articles/s41528-022-00164-w) |

**Summary:**
This paper presents a genuinely novel device — a wearable earbud-style EEG system using tattoo electrodes that feeds into an AI system for real-time adaptive control. The "Brain–AI closed loop" concept it demonstrates has strong implications for neurofeedback applications and next-generation BCIs. It's also a good example of how far hardware miniaturization has come in enabling continuous, ambient brain monitoring.

---

## Work To Be Done

- [ ] Obtain EEG signal **informed consent forms** following **ICMR guidelines**, signed by **129 student participants**.

- [ ] Design the **EEG signal acquisition experimental setup**, including:
  - Equipment configuration
  - Electrode placement
  - Recording protocol
  - Data storage procedure

- [ ] Develop **questions and test-case scenarios** for participants to evaluate EEG responses under different conditions.
