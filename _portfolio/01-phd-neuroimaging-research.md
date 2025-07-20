---
title: "Quantifying Brain Ageing with Novel Multimodal AI"
excerpt: "My Oxford PhD, where I developed novel multimodal AI models to identify 191 statistically significant factors and 57 potential new biomarkers in brain aging."
header:
  image: /assets/images/neuron-horizontal-21x9.jpeg
  teaser: /assets/images/neuron-horizontal-cropped.jpg
  caption: "Photo credit: [Unsplash](https://unsplash.com)"
permalink: /projects/phd-neuroimaging-research/
core_discipline: ["AI", "Data Science", "Neuroscience"]
meta_skill: ["Interdisciplinary Research", "Data Fusion"]
project_type: "Academic"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
---


<div class="notice--info" markdown="1">
During my PhD at Oxford, I discovered **191 statistically significant factors** and **57 potential new biomarkers** in brain aging by applying novel multimodal AI techniques, including novel vision transformers, to large-scale 3D neuroimaging datasets.
</div>

## Situation

Brain ageing is influenced by complex biological and environmental factors, and accelerated ageing is linked to diseases like Alzheimer's and Parkinson's. The difference between chronological and apparent brain age is an important biomarker for understanding factors driving accelerated ageing or resilience, crucial for health and longevity research.

However, traditional brain age estimation methods that use single-modality imaging miss critical insights, such as functional or microstructural changes, highlighting the need for a multimodal approach.

## Task

My goal was to develop advanced multimodal deep learning methods capable of accurately estimating brain age from large-scale 3D neuroimaging datasets, enriched with biological and lifestyle phenotypes. Specifically, my objectives included:

1. Expand brain age estimation beyond structural MRI to incorporate five primary neuroimaging modalities, with 57 total contrasts.
2. Develop and evaluate robust multimodal data fusion algorithms (linear, non-linear, deep learning).
3. Pioneer the first-ever 3D SWIN Vision Transformer tailored for neuroimaging, addressing known CNN limitations.
4. Identify and interpret statistically significant factors influencing brain ageing.
5. Validate models clinically and commercially in collaboration with Roche Pharma.

{% include figure
  image_path="/assets/images/exampleContrasts.png"
  alt="Example MRI Contrasts"
  caption="Example MRI contracts: (a) structural, (b) susceptibility-weighted, (c) task-functional, (d) tractography, (e) diffusion fractional anisotropy (FA), (f) diffusion FA skeletonized."
  class="align-right"
%}

## Action

I structured my  research into four phases:

### 1. **End-to-End Multimodal AI Pipeline**

I designed and implemented a scalable, comprehensive data processing pipeline to systematically handle multimodal neuroimaging data:

* **Data Ingestion & Preprocessing:** Developed optimized workflows to manage and preprocess complex 3D neuroimaging scans from the UK Biobank.
* **Model Training & Validation:** Fine-tuned robust VGG-16-based architectures, ensuring stable, reproducible predictions across large datasets.
* **Result Analysis & Interpretation:** Conducted rigorous de-biasing and deconfounding of brain age predictions, identifying statistically significant biological and lifestyle factors.

{% include figure
  image_path="/assets/images/phd-project-1.png"
  alt="Pipeline Overview"
  caption="Overview of pipeline, starting from 3D neuroimaging data ingestion, through model training, to result statistical analysis and interpretation."
  class="align-right"
%}


### 2. **Innovative Multimodal Data Fusion Techniques**

I explored multiple advanced multimodal fusion strategies, systematically evaluating their efficacy:

* **Post-Training Fusion:** Implemented linear (ElasticNet, RENT) and non-linear (MLP) approaches to combine modality predictions.
* **Identification of Independent Factors:** Applied PCA-ICA analysis to reveal independent factors contributing uniquely to brain aging.
* **End-to-End Deep Learning Fusion:** Investigated various deep learning fusion strategies, from early-stage input fusion to latent-space representation and output fusion.

{% include figure
  image_path="/assets/images/phd-project-2.png"
  alt="Pipeline Overview"
  caption="Example latent-space fusion model."
  class="align-right"
%}

### 3. **First-Ever 3D SWIN Vision Transformers for Neuroimaging**

I spearheaded the development of the first 3D SWIN Transformer architecture tailored specifically to neuroimaging data, surpassing conventional CNN limitations:

* **Enhanced Contextual Understanding:** Leveraged transformer attention to capture long-range dependencies and contextual relationships across 3D brain volumes.
* **Increased Robustness:** Demonstrated resilience to noisy or corrupted clinical-grade neuroimaging data, even when trained initially on high-quality research-grade datasets.
* **Improved Explainability:** Utilized attention activation maps to gain insights into the features relevant for brain age estimation, providing clinical interpretability.

{% include figure
  image_path="/assets/images/phd-project-3.png"
  alt="Pipeline Overview"
  caption="3D SWIN transformer architecture."
  class="align-right"
%}

### 4. **Strategic Industry Collaboration with Roche Pharma**

Throughout the project, I closely collaborated with Roche Pharma’s R&D teams, ensuring:

* **Model Translation & Integration:** Successfully translated academic findings into scalable solutions for early-stage drug discovery and biomarker validation.
* **Clinical Validation & Interpretation:** Ensured biological plausibility and clinical interpretability, bridging the gap between foundational AI research and real-world pharmaceutical applications.

## Interdisciplinary Integration

My work bridged several critical domains:

* **AI & Data Science:** Developing multimodal deep learning architectures, including novel transformer-based models, and data fusion techniques, enhancing predictive accuracy and interpretability.
* **Software Engineering:** Building and managing large-scale end-to-end data processing and analysis pipelines for 3D neuroimaging datasets, ensuring efficient high-performance computing resource optimization.
* **Neuroscience & Medicine:** Ensuring model outcomes were biologically plausible through in-depth interpretation, highlighting findings such as the association between skeletal measurements, bone mineral density, estrogen levels, and systemic inflammation in pre-menopausal women, facilitating clinical trust.
* **Commercial Strategy & Pharmaceutical Collaboration:** Aligning academic research outcomes with Roche Pharma’s drug development processes and biomarker discovery strategies.

## Result

The research delivered substantial clinical and scientific impacts:

* **Identified 191 statistically significant factors and 57 novel biomarkers**, providing actionable insights for clinical research, biomarker discovery, and drug development.
* **Established a new state-of-the-art for multimodal brain age estimation,**, demonstrating that novel transformer architectures significantly outperform traditional methods.
* **Published rigorous methodological guidelines** for clinical translation, ensuring model interpretability and biological validity.
* **Strengthened commercial research partnerships** between Oxford University and Roche Pharma, directly translating academic innovation into practical clinical applications.

## Technologies & Skills Used

* **Technical**

  * Deep Learning (CNNs, Transformers)
  * Multimodal Data Fusion
  * Data Science & Statistical Analysis (SVD, PCA, ICA, ElasticNet, RENT)
  * Neuroimaging Tools (FSL)
  * High-Performance Computing (HPC) & GPU Optimization
  * Data Pipeline Engineering

* **Research & Collaboration**

  * Clinical AI Development
  * Interdisciplinary Research
  * Biomarker Discovery, Interpretation & Clinical Validation
  * Research Translation & Commercialization
  * Effective Scientific Communication of Complex Results

## Publications & Resources

* Thesis:
  * [PhD Thesis: "Deep learning approaches to multimodal MRI brain age estimation"](https://ora.ox.ac.uk/objects/uuid:a792835e-dac8-4241-978a-97c95085feb5)
* Conferences & Publications:
  * [SDS 2023 Presentation](https://www.youtube.com/watch?v=aqhmJOsvNvU)
  * [SDS 2023 Paper](https://ieeexplore.ieee.org/abstract/document/10196736)
* GitHub Repositories:
  * Models:
    * [AgeMapper: Single-Modality Brain Age Prediction](https://github.com/AndreiRoibu/AgeMapper)
    * [MultiAgeMapper: Multi-Modal Brain Age Prediction](https://github.com/AndreiRoibu/MultiAgeMapper)
    * [SwinAgeMapper: Swin Transformer for Brain Age Prediction](https://github.com/AndreiRoibu/SwinAgeMapper)
  * Analysis Codes:
    * [AgeMapper-Analysis](https://github.com/AndreiRoibu/AgeMapper-Analysis)
    * [MultiAgeMapper-Analysis](https://github.com/AndreiRoibu/MultiAgeMapper-Analysis)
    * [SwinAgeMapper-Analysis](https://github.com/AndreiRoibu/SwinAgeMapper-Analysis)
* Datasets:
  * [UK Biobank](https://www.ukbiobank.ac.uk)
  * [Zenodo: Full Results](https://zenodo.org/records/8110876)