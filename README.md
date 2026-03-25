# EEG Signal Acquisition and Analysis Project

## Overview
This project focuses on the acquisition of EEG (Electroencephalography) signals from human subjects under varying conditions and analyzing how brain activity changes across those conditions.

EEG signals are highly sensitive, non-stationary, and prone to noise. This project aims to study:

- How EEG signals behave under different physiological and environmental conditions  
- How external and internal factors influence signal quality and interpretation  
- Methods to acquire, preprocess, and analyze EEG data effectively  

## Objectives
- Acquire EEG signals from subjects under controlled and varying conditions  
- Study the variability of EEG signals across:  
  - Cognitive states  
  - Physical conditions  
  - Environmental factors  
- Identify patterns in EEG frequency bands (Alpha, Beta, Theta, Delta)  
- Understand the impact of noise and artifacts on signal quality  
- Implement preprocessing techniques to improve signal clarity  
- Perform comparative analysis between different experimental conditions  
- Build a foundation for applications like:  
  - Brain-Computer Interfaces (BCI)  
  - Cognitive state monitoring  
  - Neurofeedback systems  

## Literature Review

### Paper 1
**Title:** A Review of EEG Acquisition, Processing and Application  
**Source:** IOP Conference Series: Journal of Physics: Conference Series  
**Year:** 2021  
**Link:** https://iopscience.iop.org/article/10.1088/1742-6596/1907/1/012045  

**Summary:**  
The paper provides an overview of EEG signal acquisition, processing, and analysis, highlighting challenges like noise and artifacts, common preprocessing and feature extraction techniques, and applications in medical diagnosis, brain-computer interfaces, and cognitive research, with an emphasis on future AI-driven advancements.

---

### Paper 2
**Title:** Electroencephalography Signal Processing: A Comprehensive Review  
**Source:** Sensors (MDPI)  
**Year:** 2023  
**Link:** https://www.mdpi.com/1424-8220/23/14/6434  

**Summary:**  
This paper reviews the entire EEG processing pipeline including signal acquisition hardware, preprocessing techniques such as filtering and artifact removal, feature extraction methods, and machine learning approaches for EEG classification tasks.

---

### Paper 3
**Title:** Miniaturization for Wearable EEG Systems: Recording Hardware and Data Processing  
**Source:** Biomedical Engineering Letters  
**Year:** 2022  
**Link:** https://link.springer.com/article/10.1007/s13534-021-00242-2  

**Summary:**  
The study explores advancements in miniaturized EEG systems designed for wearable devices. It discusses electrode design, compact amplifiers, and hardware architectures that enable portable EEG acquisition systems.

---

### Paper 4
**Title:** A Portable EEG Signal Acquisition System and Limited-Electrode Classification Network for SSVEP  
**Source:** Frontiers in Neurorobotics  
**Year:** 2025  
**Link:** https://www.frontiersin.org/articles/10.3389/fnbot.2025.771502/full  

**Summary:**  
This research presents a portable EEG acquisition platform using dry electrodes and a limited channel setup designed for steady-state visual evoked potential (SSVEP) brain-computer interface applications.

---

### Paper 5
**Title:** A Systematic Review of Techniques for Artifact Detection in EEG from Wearable Devices  
**Source:** Sensors  
**Year:** 2025  
**Link:** https://www.mdpi.com/1424-8220/25/18/5770  

**Summary:**  
The paper surveys artifact detection and removal methods used in wearable EEG systems. It evaluates techniques such as wavelet filtering, independent component analysis (ICA), and machine learning methods for improving EEG signal quality.

---

### Paper 6
**Title:** AnEEG: Leveraging Deep Learning for Effective Artifact Removal in EEG Data  
**Source:** Scientific Reports  
**Year:** 2024  
**Link:** https://www.nature.com/articles/s41598-024-75091-z  

**Summary:**  
This study proposes a deep learning-based artifact removal method that improves EEG signal quality by eliminating noise caused by eye movement and muscle activity.

---

### Paper 7
**Title:** A Systematic Review of EEG Source Localization Techniques and Their Applications  
**Source:** Journal of Neuroscience Methods  
**Year:** 2020  
**Link:** https://www.sciencedirect.com/science/article/pii/S0165027020301631  

**Summary:**  
The paper reviews computational methods used for reconstructing neural sources from EEG recordings, including dipole modeling and distributed source localization algorithms.

---

### Paper 8
**Title:** Evaluation of EEG Pre-processing and Source Localization in Ecological Research  
**Source:** Frontiers in Neuroimaging  
**Year:** 2025  
**Link:** https://www.frontiersin.org/articles/10.3389/fnimg.2025.1479569/full  

**Summary:**  
This research evaluates preprocessing pipelines and source localization techniques in real-world EEG experiments involving cognitive workload analysis.

---

### Paper 9
**Title:** Efficient Feature Extraction for EEG-Based Classification: A Comparative Review of Deep Learning Models  
**Source:** AI (MDPI)  
**Year:** 2024  
**Link:** https://www.mdpi.com/2673-2688/7/2/50  

**Summary:**  
The paper compares deep learning architectures including CNNs, RNNs, and Transformer models for EEG feature extraction and classification tasks.

---

### Paper 10
**Title:** Deep Learning-Based EEG Emotion Recognition: Current Trends and Future Perspectives  
**Source:** Frontiers in Psychology  
**Year:** 2023  
**Link:** https://www.frontiersin.org/articles/10.3389/fpsyg.2023.1126994/full  

**Summary:**  
This study reviews deep learning approaches used for emotion recognition from EEG signals and discusses commonly used datasets and evaluation methods.

---

### Paper 11
**Title:** Epileptic Seizure Detection Using Machine Learning: A Systematic Review and Meta-Analysis  
**Source:** Brain Sciences  
**Year:** 2025  
**Link:** https://www.mdpi.com/2076-3425/15/6/634  

**Summary:**  
The paper analyzes multiple machine learning approaches for EEG-based seizure detection and evaluates their diagnostic accuracy.

---

### Paper 12
**Title:** Toward Multi-Dimensional Depression Assessment Using EEG-Based Machine Learning  
**Source:** Brain Sciences  
**Year:** 2026  
**Link:** https://www.mdpi.com/2076-3425/16/2/139  

**Summary:**  
This research proposes machine learning techniques for detecting depression severity using EEG functional connectivity features.

---

### Paper 13
**Title:** The EEG Analysis and Identification of Alzheimer’s Disease: A Review  
**Source:** Frontiers in Aging Neuroscience  
**Year:** 2025  
**Link:** https://www.frontiersin.org/articles/10.3389/fnagi.2025.1686628/full  

**Summary:**  
The study reviews EEG biomarkers and signal analysis methods used to identify Alzheimer’s disease and mild cognitive impairment.

---

### Paper 14
**Title:** Design Decisions for Wearable EEG Systems to Detect Motor Imagery  
**Source:** Sensors  
**Year:** 2024  
**Link:** https://www.mdpi.com/1424-8220/23/22/9324  

**Summary:**  
The paper investigates optimal electrode placement, sampling frequencies, and signal processing techniques for wearable EEG systems used in motor imagery brain-computer interfaces.

---

### Paper 15
**Title:** Dry EEG Electrodes: A Review of Design for Brain-Computer Interface Applications  
**Source:** Sensors  
**Year:** 2014  
**Link:** https://www.mdpi.com/1424-8220/14/4/7827  

**Summary:**  
This classic review discusses the design and performance of dry EEG electrodes, highlighting their advantages for portable EEG acquisition systems.

---

### Paper 16
**Title:** Wearable EEG Electronics for a Brain–AI Closed-Loop System  
**Source:** NPJ Flexible Electronics  
**Year:** 2022  
**Link:** https://www.nature.com/articles/s41528-022-00178-z  

**Summary:**  
The paper introduces a wearable EEG system integrated with AI that allows continuous monitoring of brain signals for adaptive human-machine interaction.

