---
title: "Paint4Brains: Open Source AI Tool for MRI Segmentation"
excerpt: "Coordinated the team building a local tool providing clinicians with editable brain MRI segmentations of problematic neurodegenerative regions."
header:
  image: /assets/images/brain-art-21x9.jpeg
  teaser: /assets/images/brain-art.jpg
  caption: "Photo credit: [Pixabay](https://pixabay.com)"
permalink: /projects/paint4brains-tool/
# core_discipline: ["AI", "Software Engineering", "Project Management"]
# meta_skill: ["Healthcare Tech", "Open Source Development"]
project_type: "Open Source"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
---

<div class="notice--info" markdown="1">
I coordinated the team in building a local tool that provides clinicians with editable brain MRI segmentations of problematic neurodegenerative regions.
</div>

## Situation

Accurate MRI segmentation is essential for the prognosis and research of neurodegenerative diseases. Yet 
existing atlas-based tools are slow and struggle with segmenting brain regions 
impacted by severe atrophy, particularly in lower 
quality clinical data.



<img src="/assets/images/p4b1.png" alt="difference-healthy-alzheimer" class="align-center" style="border-radius: 1%;">

## Task

Part of our PhD-training at [SABS-R3](https://www.sabsr3.ox.ac.uk/home), our small
team partnered with GE HealthCare to engineer an open-source MRI software tool
capable of running locally on clinicians' machines, providing accurate and editable
brain MRI segmentations for patients with severe neurodegeneration.

## Action

Within our team, I took on three responsibilities:
1. Using light Agile, I worked with
clinicians and developers at GE HealthCare to define personas, jobs
to be done (JTBD), and evaluate demand for features and usability. I then worked with
the team to prioritise the backlog, plan sprints, and manage delivery.
2. Internally, I integrated the [QuickNAT](https://github.com/ai-med/quickNAT_pytorch) network into the software.
3. Finally, I wrote the documentation and delivered training sessions
to clinical end-users, supporting the adoption of the tool.

{% include figure
 image_path="/assets/images/p4b2.png"
 alt="paint4brains-screenshots"
 caption="Paint4Brain interface showing, from left to right, the segmentation process, the result, manual editing, and intensity corrections."
 class="align-right"
%}

## Result

Our team delivered [Paint4Brains](https://github.com/SABS-R3-projects/Paint4Brains), 
an open-source tool that boosted segmentation accuracy by 12% while allowing
clinicians to manually edit results. We designed the software to run locally on
standard Linux, Windows, and macOS laptops, ensuring data privacy, while improving
segmentation speed by 90% vs. traditional atlas-based methods.

## Scars

We enthusiastically developed a first version of the
tool, only to find that we misunderstood the clinicians' needs. As the
project coordinator, I understood that this was my failure to understand
our stakeholders' needs properly. This situation prompted me to stop and re-evaluate our approach,
spending time with clinicians to understand their workflows, pain points, current
tools, and desired outcomes. I also implemented regular feedback loops, ensuring that the features we developed aligned with their expectations, ultimately leading to a successful product.

## Interdisciplinary Integration

During the project, I developed skills from the following domains:
* Deep learning, specifically model selection and fine-tuning.
* Software engineering for integrating the model into the software backend.
* Team coordination and stakeholder management.

## Technologies & Skills Used

**Technical**
* Deep Learning (QuickNAT, CNNs)
* Software Engineering (CI/CD, Cross-platform development)
* MRI Segmentation & Neuroimaging Analysis
* Open-Source Development

**Project & Stakeholder Management**
* Agile Project Management
* Persona, JTBD, Demand, and Usability Analysis
* Technical Documentation & User Training
* Stakeholder Communication

## Further Information

* [Paint4Brains GitHub Repository](https://github.com/SABS-R3-projects/Paint4Brains)