---
layout: page
title: Can we measure someone’s preference without asking them directly?
description: Mathematical modeling
img: assets/img/projects/cover/project2.jpg
importance: 2
category: Research
---

<br/> 

## | Motivation

How can you know how much your friend likes a movie? One way is to ask your friend to rate the movie on a five-point scale. However, there's also another cool method to figure out their preference by having them choose between two movies.

Choice and response times have a systematic relationship. The stronger your preference for one option over another, the quicker you make your decision. By using a computational model, the Diffusion Model, that captures this relationship, we can infer someone’s preference based on their choices and response times, without needing to ask them directly!

<br/> 

## | Analysis 

As a research assistant, I led the entire process of implementing the Drift Diffusion Model (DDM). My contribution includes: 

- Built 6 DDM in Python to show the validity of a novel method for inferring preferences
- Validated Bayesian parameter estimation by examining posterior distributions, trace plots, and R hat values in R
- Provided parameter estimates for a main figure (shown in green in the below figure) and three supplementary figures, which contributed to the successful publication of a paper in a journal

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-0 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/project2/fig.jpeg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<br/> 

## | Reference 

- <a href="https://github.com/MinheeYoo/Research_infer_preference">GitHub repository</a>.
- <a href="https://www.science.org/doi/full/10.1126/sciadv.adf1665">Journal paper</a> 
  - Berlinghieri, R., Krajbich, I., Maccheroni, F., Marinacci, M., & Pirazzini, M. (2023). Measuring utility with diffusion models. Science Advances, 9(34), eadf1665.
