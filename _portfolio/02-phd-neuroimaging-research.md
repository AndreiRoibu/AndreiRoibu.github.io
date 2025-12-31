---
title: "Quantifying Brain Ageing with Novel Multimodal AI"
excerpt: "During my Oxford PhD, I developed multimodal deep learning and data analysis pipelines linking brain ageing dynamics to environmental and lifestyle factors."
header:
  image: /assets/images/neuron-horizontal-21x9.jpeg
  teaser: /assets/images/neuron-horizontal-cropped.jpg
  caption: "Photo credit: [Unsplash](https://unsplash.com)"
permalink: /projects/phd-neuroimaging-research/
# core_discipline: ["AI", "Data Science", "Neuroscience"]
# meta_skill: ["Interdisciplinary Research", "Data Fusion"]
project_type: "Academic"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
original_date: 2025-07-20
---

<div class="notice--info" markdown="1">
I developed 3D multimodal deep learning and data analysis pipelines, linking complex brain ageing processes to over 100 biological, environmental, and lifestyle factors, and supporting research into neurodegenerative diseases.
</div>

## Situation

Lifestyle, biological, and environmental factors influence brain ageing,
with research linking accelerated ageing to neurodegenerative diseases.
The difference between actual and apparent brain age can be a biomarker for
understanding factors driving accelerated ageing or resilience. This link makes brain
ageing estimation potentially important for the prevention and detection of
neurodegenerative diseases, as well as for capturing off-target effects in early
drug development.

However, traditional brain age studies have primarily relied on MRIs capturing
the brain's anatomical structure. These single-modality approaches can miss
potentially important changes captured by other imaging modalities, such as the brain's functions or microstructure.

## Task

My goal was to engineer multimodal deep learning methods capable of estimating
brain age from large-scale biomedical datasets within the UK Biobank. These datasets
included both multiple 3D MRI modalities and extensive phenotypic information. 
Specifically, my objectives included:

1. Expand brain age estimation beyond structural MRI to incorporate five primary 
neuroimaging modalities, with 57 total contrasts. A modality is a specific type
of MRI scan sensitive to different properties of the brain, such as its structure
or function. We can further divide modalities into contrasts, which are specific
types of images representing particular features within that modality.
2. Develop and evaluate linear and non-linear multimodal data fusion algorithms.
3. Developed 3D CNNs and SWIN Vision Transformers trained for brain age estimation.
4. Identify and interpret statistically significant factors influencing brain ageing.
5. Collaborate with Roche Pharma to translate research for internal use cases.

{% include figure
 image_path="/assets/images/exampleContrasts.png"
 alt="Example MRI Contrasts."
 caption="Example MRI contracts: (a) structural, (b) susceptibility-weighted, (c) task-functional, (d) tractography, (e) diffusion fractional anisotropy (FA), (f) diffusion FA skeletonised."
 class="align-right"
%}

## Action

I structured my research into four phases:

### 1. End-to-End Pipeline

The first step involved building a scalable, end-to-end, and fully automated
data processing and deep learning HPC pipeline, using multimodal 3D MRIs from 
30k UK Biobank subjects to predict brain age, which included:

* Accessing, preprocessing, and managing large-scale 3D neuroimaging datasets efficiently.
* Training and optimising 3D VGG-16-based CNN networks for each MRI modality.
* Correcting results for variance, bias, and confounds, identifying statistically significant biological and lifestyle factors correlated with brain ageing deviations.

{% include figure
 image_path="/assets/images/phd-project-1.png"
 alt="Pipeline Overview."
 caption="Overview of pipeline, starting from 3D neuroimaging data ingestion, through model training, to result statistical analysis and interpretation."
 class="align-right"
%}


### 2. Multimodal Data Fusion

Once I established the single-modality models, I focused on multimodal data fusion, which involved comparing several strategies:

* Standard linear (ElasticNet, RENT) and non-linear (MLP) ensembling of single-modality predictions.
* Deep learning based fusion, from early-stage input fusion to latent-space representation and output fusion.
* Data decomposition techniques (PCA-ICA) to identify independent factors contributing to brain ageing within a population.

{% include figure
 image_path="/assets/images/phd-project-2.png"
 alt="Pipeline Overview."
 caption="Example latent-space fusion model."
 class="align-right"
%}


### 3. 3D SWIN Vision Transformers

Despite the success of CNNs in neuroimaging tasks, they have several limitations,
including a tendency to overlook fine-grained details due to their large 
receptive fields, and limited explainability.

This observation motivated the engineering of 3D SWIN Vision Transformers for brain age estimation.
The use of transformers has several advantages over CNNs, including:
* Enhanced contextual understanding due to transformer attention, capturing long-range dependencies across 3D brain volumes.
* Increased robustness to noisy or corrupted clinical-grade data, even when trained initially on high-quality research-grade datasets.
* Improved insights into prediction-relevant features gained through attention activation maps, providing clinical interpretability.

{% include figure
 image_path="/assets/images/phd-project-3.png"
 alt="Pipeline Overview."
 caption="3D SWIN transformer architecture."
 class="align-right"
%}

### 4. Industry Collaboration with Roche

Throughout the project, I collaborated with Roche's pRED and Biomarkers teams.
The collaboration focused on:

* Translating research into prototype models supporting early drug discovery.
* Ensuring biological plausibility and clinical interpretability of identified associations and biomarkers.
* Aligning research objectives with Roche's strategic goals in neurodegenerative disease research.

## Result

The research had several key outcomes:
1. Determined that all 57 MRI contracts contain unique information relevant to understanding brain ageing.
2. Identified over 100 statistically significant lifestyle, biological, and environmental factors associated with brain ageing deviations.
3. Demonstrated that ElasticNet ensembling surpasses deep fusion for multimodal predictions, indicating trade-offs.
4. Showcased the advantages of 3D SWIN Vision Transformers over CNNs for brain age estimation, including robustness and interpretability.
5. Established a set of methodological guidelines for clinical translation of brain age models, ensuring the biological validity of findings.

## Scars

_Iterate quickly, test thoroughly, and ask for regular feedback._

I spent the first 1.5 years of my 3-year PhD engineering deep autoencoders to 
predict brain function from structural maps. While getting positive results
outperforming PCA/PLS methods, and addressing a core
gap in neuroscience, they were inconclusive.
Instead of stopping and reassessing, I persevered, refining hyperparameters and the 
architecture, instead of zooming out and reframing the problem. When I finally
did this, it was too late, endangering my completing the PhD, which required "3
significant contributions", forcing me to pivot to brain age predictions at the
cost of having publications.

## Interdisciplinary

My work bridged several domains:

* AI & Data Science: Developing multimodal deep learning architectures and data fusion techniques.
* Software Engineering: Building and managing large-scale end-to-end data processing and analysis pipelines for 3D imaging and biomedical datasets.
* Neuroscience & Medicine: Ensuring model outcomes were biologically plausible, highlighting findings such as the association between skeletal measurements, bone mineral density, oestrogen levels, and systemic inflammation in pre-menopausal women.
* Research Translation: Aligning research outcomes with Roche's drug development processes and biomarker discovery work.

## Technologies & Skills Used

* Technical

  * Deep Learning (CNNs, Transformers)
  * Multimodal Data Fusion (Linear, Non-Linear)
  * Data Science & Statistical Analysis (SVD, PCA, ICA, ElasticNet, RENT)
  * Neuroimaging Tools (FSL)
  * HPC Tools (Slurm, Bash scripting)
  * Data Pipeline Engineering

* Research & Collaboration

  * Clinical AI Development
  * Interdisciplinary Research
  * Biomarker Discovery, Interpretation & Clinical Validation
  * Research Translation & Commercialisation
  * STEM Outreach & Scientific Communication

## Publications & Resources

* Thesis:
  * [PhD Thesis: "Deep learning approaches to multimodal MRI brain age estimation"](https://ora.ox.ac.uk/objects/uuid:a792835e-dac8-4241-978a-97c95085feb5)
* Conferences & Publications:
  * [SDS 2023 Presentation](https://www.youtube.com/watch?v=aqhmJOsvNvU)
  * [SDS 2023 Paper](https://ieeexplore.ieee.org/abstract/document/10196736)
* GitHub Repositories:
  * Models:
    * [AgeMapper: Single-Modality Brain Age Prediction](https://github.com/AndreiRoibu/AgeMapper)
    * [MultiAgeMapper: Multimodal Brain Age Prediction](https://github.com/AndreiRoibu/MultiAgeMapper)
    * [SwinAgeMapper: Swin Transformer for Brain Age Prediction](https://github.com/AndreiRoibu/SwinAgeMapper)
    * [BrainMapper: Linking the Brain's Structural and Functional Connectivity](https://git.fmrib.ox.ac.uk/aroibu/functionmapper)
  * Analysis Codes:
    * [AgeMapper-Analysis](https://github.com/AndreiRoibu/AgeMapper-Analysis)
    * [MultiAgeMapper-Analysis](https://github.com/AndreiRoibu/MultiAgeMapper-Analysis)
    * [SwinAgeMapper-Analysis](https://github.com/AndreiRoibu/SwinAgeMapper-Analysis)
* Datasets:
  * [UK Biobank](https://www.ukbiobank.ac.uk)
  * [Zenodo: Full Results](https://zenodo.org/records/8110876)