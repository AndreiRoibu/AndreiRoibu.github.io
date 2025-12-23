---
title: "Market Modelling for Hybrid-Electric Aviation"
excerpt: "Modelled regional aviation market dynamics, investigating the feasibility and total addressable market of hybrid-electric regional aircraft."
header:
  image: /assets/images/cities-21x9.jpeg
  teaser: assets/images/cities.jpg
  caption: "Photo credit: [Unsplash](https://unsplash.com)"
permalink: /projects/rolls-royce-market-strategy/
# core_discipline: ["Data Science", "Business Strategy"]
# meta_skill: ["Market Simulation", "Strategic Forecasting"]
project_type: "Professional"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
---

<div class="notice--info" markdown="1">
I modelled regional aviation market dynamics, investigating the feasibility and total addressable market of hybrid-electric regional aircraft, informing the group CTO and external partners.
</div>

## Situation

Rolls-Royce and its airline partners were exploring electrification in aviation. While progress existed in larger aircraft platforms, the viability of electrifying regional aviation markets remained uncertain. Key questions included:

* Was regional aviation a disruptive, viable entry point for electrification?
* Could an electrified regional aircraft be profitable, given existing market dynamics and high development costs?
* What design parameters, performance targets, and regulatory considerations would be required to succeed?

## Task

During my internship in the Future Technologies Group, and internal Rolls-Royce 
consultancy team, my team tasked me with determining the following:

1. Market attractiveness and total addressable market (TAM) for regional hybrid-electric aircraft.
2. Optimal aircraft design parameters and KPIs.
3. Estimated strategic and financial benefits to Rolls-Royce.

Despite being an intern, I was tasked with this project given my good performance
in a prior summer internship. While my manager gave me autonomy, I worked closely and
received mentorship from senior engineers and managers.

{% include figure
 image_path="/assets/images/regional-aircraft.jpg"
 alt="A regional turboprop aircraft."
 caption="Photo credit: [Unsplash](https://unsplash.com)"
 class="align-center"
%}

## Action

To address these questions, I adopted the following approach:
* Firstly, I adapted an internal agent-based transportation model to simulate regional air dynamics, augmenting it with models of aircraft operating costs and airport noise perception.
* I then populated the model with two datasets for specific geographies: one containing socio-economic information of population centers, and another with detailed airport infrastructure information.
* Finally, I tested different aircraft designs under scenarios incorporating regulatory, noise, legal, and route‑economics constraints and counterfactuals.

{% include figure
 image_path="/assets/images/rolls-royce-transportation-model.png"
 alt="rolls-royce-transportation-model"
 caption="Diagram of the agent-based transportation model, simulating millions of passenger transportation decisions based on economics, demographics, and travel preferences."
 class="align-right"
%}

## Result

I delivered my results as a strategic study to the CTO and external partners. My analysis found that regional hybrid-electric aircraft could be disruptive in markets such as the US and India under certain conditions, with a total addressable market estimated at USD 840 million annually. The findings were later validated by Cranfield University and Mott MacDonald, with the proposed aircraft design influencing the [2022 Airbus ZeroE regional concept](https://www.airbus.com/en/innovation/energy-transition/hydrogen/zeroe-our-hydrogen-powered-aircraft).

## Scars

The grilling I received from Rolls-Royce's CTO in the first presentation I gave will always stay with me: I was simultaneously too technical, not technical enough, and did not answer the strategic questions he had in mind. This experience taught me several points:
1. Know your audience, their pain points, needs, and interests.
2. When the question is ambiguous, use systems thinking, as non-obvious aspects may play a key role, such as runway materials to public noise perception.
3. Use the right tools for the job, and when they are not available, don't be afraid to build them yourself.


## Interdisciplinary Integration

This project combined tools and insights from multiple domains:
* Aerospace engineering and aircraft design.
* Data analysis and modeling with counterfactuals.
* Economics and market dynamics.
* Regulatory, social, and political analysis.

{% include figure
 image_path="/assets/images/rolls-royce-plane.png"
 alt="rolls-royce-plane"
 caption="Subset of parameters found to impact the market viability of regional aviation electrification, ranging from technical properties to regulatory constraints and public perceptions."
 class="align-center"
%}

## Technologies & Skills Used

* **Technical:** 
  * Agent-Based Modeling
  * Market Simulation
  * Data Analysis
  * Counterfactual Modeling

* **Strategic:** 
  * Technology Roadmapping
  * Business Case Development
  * Market and Regulatory Analysis
  * C-Suite Engagement & Communication

## Disclaimer

> Rolls-Royce has permitted me to share the above information for academic and fair personal use. Further details remain confidential.