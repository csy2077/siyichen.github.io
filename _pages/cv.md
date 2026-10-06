---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D. in Electrical and Computer Engineering, University of Michigan, Ann Arbor, 01/2026 – Present
  * Advisors: [Jun Gao](https://www.cs.toronto.edu/~jungao/), [Qing Qu](https://qingqu.engin.umich.edu/)
  * Research directions: video diffusion distillation, VLM harness for robot, LLM harness for scientific problems, etc.
* B.S. in Physics, School of Physics, Peking University, 09/2021 – 07/2025
  * Research directions: probabilistic machine learning, diffusion models, computational imaging, inverse problems, etc.

Work experience
======
* 06/2025 – 12/2025: Computational Scientific Imaging Lab, AI for Science Institute, Peking University
  * Adopting current LLM agents to automatically solve scientific problems, mainly computational imaging problems, including automatically understanding the problem settings, planning, and code generation.
* 01/2025 – 03/2025: ByteDance, Douyin Group Content Quality and Data Service, Beijing
  * Enhancing the "intelligence" of LLMs: improving the model's performance across the entire pipeline (pretraining, supervised fine-tuning, RLHF).
  * Following cutting-edge industry research advancements and facilitating their practical implementation with the team.
  * Participating in exploratory projects, researching data-producing methods and formats for large models.
* 06/2024 – 12/2024: Electrical and Computer Engineering, University of Michigan, Ann Arbor
  * Lead the ML for scientific application project in Qing's group, the main project is to use the generative models to model and predict chaotic dynamic systems like fluids and use it to solve real-world problems, we primarily focus on the data assimilation task.
  * Introduce the current research projects in various seminars and symposiums, like IMSI workshop, CSP seminar etc.
  * Work on basic medical imaging tasks, like MRI and ultrasonic computed tomography.

Research experience
======
* Video generation: Data-Forcing Distillation for few-step video diffusion, University of Michigan, 01/2026 – Present
  * Advisors: [Jun Gao](https://www.cs.toronto.edu/~jungao/), [Shaowei Liu](https://stevenlsw.github.io)
  * Identify two failure modes of reverse-KL distribution-matching distillation (DMD/DMD2) for video diffusion: collapsed sample diversity and over-saturated outputs.
  * Propose Data-Forcing Distillation (DFD), a simple post-training framework that uses the teacher score discrepancy at real data to pull the few-step student toward the true data distribution.
  * Validate on text-to-video, image-to-video, and autoregressive generation with Wan2.1-1.3B and Cosmos-Predict2.5-2B; with only 100–300 finetuning steps, DFD restores diversity and fidelity and surpasses the teacher in video dynamics and visual quality.
* LLM agents: Benchmarking coding agents on scientific computational imaging, Peking University, 06/2025 – 12/2025
  * Advisor: [He Sun](https://ai4imaging.github.io/team.html)
  * Build Imaging-101, a benchmark of 57 expert-verified computational imaging tasks across six scientific domains, each grounded in a peer-reviewed paper and canonicalized into a four-stage pipeline (preprocessing, forward physics modeling, inverse solver, visualization).
  * Design three evaluation tracks (planning, function-level unit tests, end-to-end reconstruction) to probe distinct agent capabilities across the full pipeline.
  * Evaluate seven frontier LLMs, uncovering systematic gaps in algorithm selection, physical convention handling, and pipeline integration, and pointing toward skill-augmented, domain-specialized agents.
* Deep learning models: Flow models for data assimilation, University of Michigan, 06/2024 – 12/2024
  * Advisors: [Qing Qu](https://qingqu.engin.umich.edu/), [Jeffrey A. Fessler](https://web.eecs.umich.edu/~fessler/)
  * Use the stochastic interpolants framework to model stochastic dynamic systems and develop data assimilation algorithms on top of it.
  * Apply the proposed method to real-world settings, like climate modeling, weather forecasting, seismology analysis.
* Deep learning models: Diffusion models for inverse problems, Peking University, 02/2024 – 06/2024
  * Advisor: [He Sun](https://ai4imaging.github.io/team.html)
  * Use the latent diffusion model to solve blind inverse problems in 2D (blind motion deblurring) and 3D (pose-free sparse-view reconstruction).
  * Combine the PnP Monte Carlo algorithm to iteratively estimate clean images from noisy measurements and train the diffusion model.
* Computational optics: Multi-channel detection in SMLM, Peking University, 06/2023 – 01/2024
  * Advisor: [He Sun](https://ai4imaging.github.io/team.html)
  * Simulate the physics of detection in single-molecule localization microscopy, and denoise, filter and detect molecules with conventional signal processing methods.
* Quantum physics: Design and simulation of quantum chips, Peking University, 10/2022 – 05/2023
  * Advisor: [Jianwei Wang](https://sites.google.com/view/qchip/home)
  * Design quantum optical devices on chips, test and compare device structures experimentally, and simulate them with COMSOL and custom Python programs.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Open-source contributions
======
* [NVIDIA FastGen](https://github.com/NVlabs/FastGen) (contributor)
  * Fixed a per-frame timestep allocation bug in the video2world (image2world) inference mode of Cosmos-Predict2 ([merged PR #26](https://github.com/NVlabs/FastGen/pull/26)).
* [Data-Forcing Distillation (DFD)](https://github.com/csy2077/data-forcing-distillation) (author and maintainer)
  * Implemented the DFD method on top of the NVIDIA FastGen codebase, with support for Wan2.1 text-to-video, autoregressive and Cosmos-Predict2.5 image-to-video distillation.

Awards & honors
======
* 12/2021: Scholarship for Freshman Students, 3rd prize, Peking University

Membership
======
* 12/2024 – Present: IEEE Member

<!-- Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3 -->

<!-- Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams -->
