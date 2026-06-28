---
title: "Q2 2026: Much Reckoning"
excerpt: "In which I reflect on who I am and what is truly sustainable."
layout: single
header:
  image: /assets/quartely-audits/2026Q2.003.png
  teaser: /assets/quartely-audits/2026Q1.002.png
  caption: "Photo credit: [Andrew Neel](https://unsplash.com/@andrewtneel)"
category: "Career"
section: blog
tags:
  - Career
author_profile: true
read_time: true
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
original_date: 2026-06-27
---

<div class="notice--info" markdown="1">
In which I reflect on who I am and what is truly sustainable.
</div>

# Q2 2026

Q2 was a strategy-reset quarter. The output was not only shipped artefacts, but a clearer operating model for the next phase: German as the main long-term personal-development stream, AI systems as the professional direction, and fewer parallel projects.

## Who am I (Professionally)?

The main event of Q2 was attending [SDS 2026](https://sds2026.ch/), where I gave a [business talk about my customer-facing work at Synthara](https://andreiroibu.com/business/sds/). Beyond networking, the event prompted a reflection on my professional identity:

> Am I still a _mainstream_ ML engineer?

The answer I reached is:

> I am an AI systems engineer working at the interface between ML, DSP, systems, hardware, customers, and benchmarking. My role is to understand workloads well enough to map, benchmark, diagnose, deploy and explain them on specialised hardware.

This realisation shifts my development focus away from trying to keep up with the entire ML field, and towards owning the application-to-hardware translation layer: workload analysis, benchmarking, performance trade-offs, customer constraints, and system-level reasoning.

Concretely, after completing the transformer-classification project, I plan to focus on:

- SoC, NoC, and computer architecture fundamentals;
- Efficient mapping of workloads such as transformers onto specialised hardware;
- Performance-oriented software fundamentals, including practical C/C++; and
- Small passion projects that maintain my ML and data science literacy.

Longer term, useful adjacent topics include MLIR and compiler toolchains, as well as applied algorithms relevant to performance engineering.

## German

In Q2, I completed the Goethe-Institut A2.1 German module, spending ~80 hours on this.

German is becoming a central part of my long-term plan because I want to settle permanently in Switzerland. For this, I first need to obtain a [C EU/EFTA permit](https://www.sem.admin.ch/sem/en/home/themen/aufenthalt/eu_efta/ausweis_c_eu_efta.html), and later pursue Swiss citizenship.

For an early C-permit in Zürich, I need to demonstrate at least [B1 spoken German and A1 written German](https://www.zh.ch/content/dam/zhweb/bilder-dokumente/themen/migration-integration/einreise-aufenthalt/weisungen/Niederlassungsbewilligung%20IW.pdf). In practice, this means aiming for a solid B1 level overall.

The A2.1 module made clear that this will require sustained effort over the next 1-2 years. German will therefore become my main personal-development stream outside work.

To count my German studies as ISH, I added a [`Deutsch`](https://andreiroibu.com/deutsch/) section to this website, serving as a personal language-learning journal. The plan is to publish weekly or bi-weekly collections of short texts, spoken reflections, and notes on what I learned. I will keep the main `Blog` focused on technical and professional topics.

The first posts are:
- [27 Juni 2026: Die Ersten Schritte](https://andreiroibu.com/deutsch/deutsch/): a collection of texts written during A2.1
- [28 Juni 2026: Mein Lebenslauf](https://andreiroibu.com/deutsch/mein-lebenslauf/): a German version of my CV

## Engineering in the Age of AI

I have also been reflecting on where software engineering is going in the age of AI, concluding that:

> Software engineering is moving away from traditional coding and towards defining, constraining, verifying, integrating, and owning technical systems.

I find recent developments analogous to my aerospace engineering experience, where, during my studies, I learned the underlying equations behind fluid dynamics, while in practice, much of the engineering work involved using tools such as Ansys Fluent: defining the problem, setting the constraints, validating assumptions, interpreting results, and understanding when the tool output was misleading.

Something similar is happening with AI-assisted software engineering. The value of writing code manually is not disappearing, but it is becoming less differentiated. The more durable skills are likely to be:

1. **_Specification and problem decomposition_**, through writing design intent and specifications, defining acceptance criteria, splitting work into reviewable tasks, writing architectural decision records, maintaining good documentation, and creating agent-ready GitHub issues.
2. **_Verification, testing, and quality engineering_**, to ensure that code doesn't just look correct, but is correct.
3. **_Debugging, tracing, and observability_**, to ensure that when things go wrong, they can be diagnosed and fixed quickly.
4. **_Architecture and maintainability_**, as architecture matters more when implementation is easy and cheap.
5. **_Domain Depth_** as agents do not substitute for understanding the problem, and a well-defined problem amplifies agent effectiveness.
6. **_Soft, Transferable Professional Skills_**, such as ownership, communication, documentation, customer work and cross-functional collaboration.

In Q3 and beyond, I want to apply these ideas more deliberately to my own projects. This may also become a separate blog post.

## Sustainable Routines

After over six months of sustained career development, I have enough data to reassess what is sustainable. During a typical work-week, I spend ~113.5 hours on various activities, leaving ~1.3 hours/day outside these fixed commitments. This is insufficient for any meaningful personal development work.

| Task | Hours |
| --- | ---: |
| Work | 42.5 |
| Commute | 5.0 |
| German | 6.0 |
| Exercise | 5.0 |
| Sleep | 42.5 |
| Cooking and household | 12.5 |
| **Total** | **113.5** |

I tried to compensate by pushing more work into the weekend. The result was predictable: diminishing returns and rising cognitive fatigue.

The conclusion is that a sustainable routine should not depend on large weekend workloads. A realistic ceiling is around three to four additional focused hours on the weekend, most of which will likely go to German while I work towards B1.

For professional development, this means I need to be selective. Projects should be tightly coupled to my current work at Synthara and my longer-term AI-systems direction. Otherwise, I risk spreading myself too thin and producing neither good work nor useful rest.


# Career Capital Tracker

| Project | Total ISH | Status | Notes |
| --- | ---: | --- | --- |
| Adversarial Prompt Classification with Transformers | 4.5 | Below plan | Stopped the large project build, focusing on cleaning up the old notebook. |
| Data Structures and Algorithms | 16 | On plan | Steady progress, mostly maintenance work. |
| SDS 2026 submission | 8 | On plan | Poster and write-up. |
| German A2.1 | 80 | On plan | Completed the A2.1 module, starting A2.2 and B1.1 in Q3 2026. First blog post contains texts I wrote during A2.1 |

In total, I accumulated 108.5 Inspectable Shipped Hours (ISH) in Q2 2026. 

The quarter involved significant reflection, which is not directly measurable in ISH. Even so, it was valuable. I finish Q2 with a clearer understanding of who I am professionally, what I need to learn, and how much I can sustainably take on.

{% include figure
 image_path="/assets/quartely-audits/2026Q2.001.png"
 alt="Q2 2026 ISH."
 caption="Inspectable Shipped Hours (ISH) for Q2 2026."
 class="align-right"
%}

# Books Read

I have not made much progress on reading this quarter, and I am still reading the books I started in Q1 2026:
- [Big Trust](https://www.shadezahrai.com/bigtrust) by Dr Shadé Zahrai and Faysal Sekkouah
- [Stoicism For Dummies](https://www.dummies.com/book/body-mind-spirit/philosophy/general-philosophy/stoicism-for-dummies-301324/) by Tom Morris and Gregory Bassham

# Next Quarter

In Q3 2026, my focus will be on:

- The Goethe-Institut German course, aiming to complete the _A2.1_ and start the _B1.1_ module (~100 ISH hours)
- Cleaning up the _Adversarial Prompt Classification with Transformers_ project, and publishing a blog post about it (~4 ISH hours)
- Investigating Transformer workload architectures, and their deployment on specialised hardware (~9 ISH hours)