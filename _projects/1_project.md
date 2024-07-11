---
layout: page
title: Are consumers more likely to buy a product when it is surrounded by high-value options?
description: Mathematical modeling
img: assets/img/projects/cover/project1.jpg
importance: 1
category: Research
---

<br/> 

## | Motivation

Imagine a chocolate lover who is deciding whether to buy a chocolate bar. If they are in Belgium, known for its renowned chocolate craftsmanship, they might be more eager to make the purchase. They could be quicker to decide, more inclined to buy, or even willing to spend more money on a chocolate bar compared to if they were in Iceland. 

As illustrated in the above example, context can affect the choice and valuation of options. There are two possible mechanisms of context effects. These two mechanisms differentially affect choices and response times. Also, different parameters of the Drift Diffusion Model (DDM) capture these two mechanisms. 

- **Mechanism 1: A high-value context might make items appear less attractive or more attractive.**
  - Context effect in both slow and fast responses
  - Drift rate in the DDM
- **Mechanism 2: A high-value context might set prior expectations about the item’s value.**
  - Context effect only in fast responses
  - Starting point in the DDM

<br/> 

## | Analysis 

- Built 12 DDM in R and Python to explain the choices and response times of 153 participants (>22,000 records)
- Evaluated the performance of models using BPIC and DIC
- Conducted EDA on the choices and response times using t-test and mixed-effect logistic/linear regression models in R

<br/> 

## | Results

### EDA 

- Context had **a positive effect** on choice and valuation.
    - The target product was more likely to be chosen and valuated to be higher, when it was surrounded by high value context products.
- Interestingly, the positive effect of context on choice and valuation was observed **only in fast responses** (First and second RT bins).

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-6 mt-md-0">
        {% include figure.liquid path="assets/img/projects/project1/exp1_eda.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-6 mt-md-0">
        {% include figure.liquid path="assets/img/projects/project1/exp2_eda.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<br/> 

### Modeling 

- Among the six computational models considered for Experiment 1, the best-fitting model included context effects on both starting point and drift rate.

<div class="row justify-content-sm-center">
    <div class="col-sm-9 mt-0 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/project1/exp1_model.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- Also, simulation of six models for Experiment 2 showed that the starting point bias model showed the observed relationship between bids and response time. 

<div class="row justify-content-sm-center">
    <div class="col-sm-9 mt-0 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/project1/exp2_model.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<br/> 

## | Conclusion

In summary, this study shows that context affects the choice and valuation of options by setting prior expectations for upcoming choices and valuations. 

<br/> 

## | Reference 

- <a href="https://github.com/MinheeYoo/Research_context">GitHub repository</a>.
- <a href="https://academic.oup.com/pnasnexus/article/3/7/pgae232/7697877?login=true">Journal paper</a> 
  - Izakson, L.<sup>1</sup>, **Yoo, M.**<sup>1</sup>, Hakim, A., Krajbich, I., Webb, R., & Levy, D. J. (2024). Valuations of target items are drawn towards unavailable decoy items due to prior expectations. PNAS nexus, 3(7).
    - 1 denotes equal contribution
