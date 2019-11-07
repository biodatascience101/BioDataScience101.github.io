---
layout: page
title: Projects
permalink: /projects/
toggle: on
rank: 1
---



<div class="lab-wrapper">
    <ul class="lab-list">
    {% for project in site.data.projects %}
    {% if project.name and project.description %}
        <li>
            <h2>{{ project.name }}</h2>
            {% if project.photo %}
                <img class="float-right projects-photo" src="{{ project.photo | prepend: site.images_dir | prepend: site.baseurl }}">
            {% endif %}
            {% if project.funding %}
                <p><b>Funding: </b>{{ project.funding }}</p>
            {% endif %}
            {% if project.collaborators %}
                <p><b>Collaborators: </b>{{ project.collaborators }}</p>
            {% endif %}
            {% if project.assignees %}
                <p><b>Assignees: </b>{{ project.assignees }}</p>
            {% endif %}
            <p>{{ project.description }}</p>
        </li>
    {% endif %}
    {% endfor %}
    </ul>
</div>


## **Student Projects**

### **Title:** The role and effects of partitioning

#### **Aim:** The aim of this project is to identify which partitioning method is the most meaningful for data redundancy and least computationally expensive to obtain the best possible predictions when using Deep Learning.

#### **The project:** The student will be working with different partitioning methods to study their effect and role in Deep Learning predictions.

###  **Title:** Benchmarking neoepitope prediction methods

#### **Aim:** Study and compare state of the art neoepitope prediction methods and their relevance in current immunotherapy strategies

###  **Title:** Deep Learning for CDR3 structural feature predictions

#### **Aim:** Improve structural feature predictions of highly variable CDR3 regions using Deep Learning 

###  **Title:** The effect of checkpoint inhibitor therapy on lymphocyte repertoire composition

#### **Aim:** The project aim is to investigate available repertoire sequencing data before and after checkpoint inhibitor therapy, and using computational tools to predict the immunogenicity of sequences

###  **Title:** Lyra 2.0: furtherance of existing template based prediction

#### **Aim:** Optimise Lyra for improved predictions of protein structure models

###  **Title:** Developing a similarity metric for complementarity determining region 3 (CDR3) of T cell receptor ß (TCR ß) based on 3D conformational predictions

#### **Aim:** The goal of the project is to produce a metric to calculate the similarity between CDR3 regions of the TCRβ from primary sequences, however based on 3D structural predictions.

###  **Title:** Diversity of TCR repertoires: state of the art and prospects

#### **Aim:** Exploring current immune repertoire diversity analysis and their implications in patient outcome prediction and therapy engineering

###  **Title:** Machine Learning for pairing structural data

#### **Aim:** Majority of high-throughput sequencing data available in public repositories is unpaired and not on single-cell level. The aim of the project is applying machine learning algorithms in an attempt to match  the quality of existing data with those obtained with more recent techniques, thus improving the informational yield

### **Title:** Embeddings for improved immune system relevant predictions

#### **Aim:** Studying multiple embedding methods for context learning, which will improve Deep Learning prediction methods for immune system relevant problems

### **Title:** Pysam package optimisation

#### **Aim:** Reducing computational cost and data scaling for the Pysam module in relation to current projects
