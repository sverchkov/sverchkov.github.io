---
title: Yuriy Sverchkov
author: Yuriy Sverchkov
layout: default
---

## Research Interests

I develop machine learning and statistical methods for problems in biology and medicine.
My focus is on using graphical models to represent complex relationships.
I am interested in statistical methods, Bayesian models, stochastic models, and automated systematic explanation of these models.

## Ongoing Research

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url }})
{{ project.description }}
{% endfor %}

## Education

PhD | 2014 | Intelligent Systems | University of Pittsburgh, Pittsburgh, PA
MS  | 2011 | Intelligent Systems | University of Pittsburgh, Pittsburgh, PA
BS  | 2008 | Computer Science    | University of Maryland, Baltimore County, Baltimore, MD
BS  | 2008 | Mathematics         | University of Maryland, Baltimore County, Baltimore, MD

## Publications

A complete listing available [here](https://www.ncbi.nlm.nih.gov/myncbi/yuriy.sverchkov.1/bibliography/public/) and [on Google Scholar](https://scholar.google.com/citations?user=sx6aKSUAAAAJ).

## Past Research

{% for project in site.past_projects %}
 * [{{ project.title }}]({{ project.url }})
{% endfor %}
