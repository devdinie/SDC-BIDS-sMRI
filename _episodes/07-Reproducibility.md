---
title: "Reproducibility considerations"
teaching: 20
exercises: 10
questions:
- "How sensitive are the findings to your MR pipeline parameters?"
objectives:
- "Understand impact of software and atlas choices"
keypoints:
- "It is crucial to assess biological vs methodological variation in your findings to avoid reproducibility crisis."
---
## You Are Here!
![course_flow](../fig/episode_8/Course_flow_8.png)

## MR image processing pipeline selection choices
- Compute environment 
    - OS / system math libararies 
    - Programming libraries Python / R versions

- Software (algorithms and their versions)
    - Image clean-up
    - Image preproc
    - Image quantification

- Quality control
    - Manual protocol specifics
    - Automatic outlier criteria

- Biological priors
    - Templates 
    - Atlases/parcellations: ROI definitions

## Example software analysis

- Task: compare cortical thickness between FreeSurfer and CIVET
![reproducibility](../fig/episode_8/Reproducibility.png)

_Note: See [this]([https://academic.oup.com/cercor/article/30/9/5014/5831485]) for details on brain plots]_

- Correlation between thickness measurements:
  - Software: FreeSurfer (v5.1, v5.3, v6.0), CIVET (2.1) and ANTs
  - Parcellation: DKT
    
![software_compare](../fig/episode_8/CT_compare_software.png)

{% include links.md %}
