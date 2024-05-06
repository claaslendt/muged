# Machine Learning for Unsupervised Gait Event Detection

This repository is dedicated to the research project 'Machine Learning for Unsupervised Gait Event Detection'. This project is supported by a fellowship of the German Academic Exchange  Service (DAAD) for Claas Lendt.

*All code and data for this research project will be added to this repository at a later stage of the project.*



## Short background

Thigh-worn accelerometers are becoming more and more popular in physical activity research because they let researchers monitor how people behave physically in real-world settings. Several large-scale cohort studies in the Prospective Physical Activity, Sitting and Sleep consortium (ProPASS) have now started using thigh-worn accelerometers. Data from these devices can be used to classify different types of activity and postures when they're used with data-driven algorithms. This can help researchers to find out more about how different activities affect our health. This approach can also help us measure new digital biomarkers, such as how we walk, using the information in the raw acceleration signal.



## Our approach

We are developing and validating a data analytics pipeline (see below) to help us identify when someone is walking and when gait events take place without any human intervention. This involved several key steps:
1. **Pre-processing**: We resample and filter the raw acceleration signal to a common sampling frequency.
2. **Walking sequence detection**: A deep learning algorithm identifies walking sequences based on fixed time-intervals of acceleration data.
3. **Gait event prediction**: A second deep learning algorithm predicts the probability for gait events for each timepoint within each walking sequence.
4. **Post-processing and filtering**: Gait events are identified based on the probability distributions. Identified gait events are filtered using heuristic approaches.
5. **Gait analysis**: Gait-specific parameters (stride time, swing time and stance time) are calculated for each stride and then summarised across individual walking sequences.



![Fig1](https://github.com/claaslendt/muged/blob/main/figures/Fig1.jpg)



## Progress of the project :rocket:

(Last update: 2024-05-07)

We have made significant progress since the start of the project. We have collected all our data at GSU Cologne. We have managed to pool several existing activity classification datasets (based on GSU and AUT data) to train our deep learning walking classification algorithm. And in the last few weeks, we have been able to build and validate the analytics pipeline. Currently, we are in the process of documenting and submitting our results to a scientific journal for peer-review.



**A quick overview on our progress so far**

- [x] **Data collection** at GSU Cologne.
- [x] **Cleaning and pre-processing** of the collected data.
- [x] **Training of a deep learning walking classification model** using a pooled dataset.
- [x] **Final analysis and validation** using an external dataset.
- [ ] **Submitting und publishing our results** in a scientific journal.



We are looking forward to share our final pipeline, the validation results and methods in the near future. Stay tuned!



**Figure 1**. Example of the gait event predictions

![StrideSegmentationWalking](https://github.com/claaslendt/muged/blob/main/figures/Fig2.png)

