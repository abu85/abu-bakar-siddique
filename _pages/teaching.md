---
layout: single
permalink: /teaching/
author_profile: true
classes: wide
---

<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>    
        h3 {
            margin-top: 0;
            margin-bottom: 0;
            padding-left: 5px;
        }
        .intro ul {
            margin-top: 4px;
            margin-bottom: 0;
            list-style-type: square
        }
        .intro p {
            margin-top: 0;
            margin-bottom: 0;
            color:gray;
            font-size: 80%;
        }
        .toggle-content {
            display: none; /* Hide content by default */
            opacity: 0; /* Start hidden */
            max-height: 0; /* Start hidden */
            overflow: hidden; /* Prevents content overflow */
            transition: max-height 0.5s ease, opacity 0.5s ease; /* Smooth transition */
            margin-bottom: 20px;
            font-size: 80%;
        }
        .toggle-button {
            cursor: pointer;
            display: flex;
            align-items: center;
            user-select: none; /* Prevent text selection */
            margin-bottom: 15px; /* Add bottom margin for gap */
        }
        .toggle-button .fas {
            margin-left: 10px;
            transition: transform 0.3s;
        }
        .toggle-button.active .fas {
            transform: rotate(90deg);
        }
        .toggle-content.show {
            display: block;
            opacity: 1;
            max-height: 1000px; /* Large enough to display the content */
        }
        .youtube-container {
            position: relative;
            width: 66.66%; /* Set width to 2/3 of the container */
            max-width: 100%; /* Ensure it doesn't exceed the container's width */
            padding-bottom: 37.5%; /* Aspect ratio 16:9 */
            height: 0;
            margin-bottom: 40px; /* Add some space below the video */
        }
        .youtube-iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }D
        @media (max-width: 600px) {
            .youtube-container {
                width: 100%; /* Full width on small screens */
                max-width: none; /* Remove max width on small screens */
            }
        }
    </style>
</head>
<h2>Teaching</h2> 

<body>
<div class="intro">

### 1. Analysis of High-Throughput Sequencing RNA-Seq Data (PhD course)
**Role:** Co-instructor  
**Lecture:** Interactive teaching focusing on biological interpretation (Q&A format) of RNA‑Seq bioinformatic results.  
**Lab:**  
- HPC environment setup  
- Running Nextflow-based **nf-core/rnaseq** pipelines  
- Interpretation of QC metrics, alignment statistics, and expression matrices  
- Downstream analysis in R: **DESeq2**, GO & KO enrichment, and biological result validation

---

### 2. Genome-wide Predictions in Breeding: Genotype–Phenotype Associations and Genomic Selection (PhD course)
**Role:** Co-instructor / Bioinformatics mentor  
**Lecture:** Introduction to Linux, R & RStudio  
**Lab:**
- Hands on linux & R introduction
- Set up for the GWAS analysis: instalation of bioinfo tools and R packages or functions  

**Topics covered:**  
- Statistical genomics foundations  
- SNP calling and variant quality assessment  
- GWAS workflows and visualization  
- Genomic prediction using mixed models and machine‑learning approaches  
- Interpretation of genotype–phenotype associations  
- Best practices for reproducible breeding informatics pipelines

---

### 3. Data Handling and High-Quality Illustrations for Publications (PhD course)
**Role:** Instructor  
**Topics covered:**  
- Data management strategies in R  
- Automated dataset merging, cleaning, and version control  
- Creating publication‑quality multi-panel figures with **ggplot2**  
- Reproducible analysis: project structure, DOIs, and open‑science workflows  
- Hands‑on sessions with tidyverse and #tidytuesday datasets

---

### 4. Multi-omics Analyses of the Microbial Community (PhD course)
**Role:** Co-instructor  
**Topics covered:**  
- Overview of multi-omics: metagenomics, metatranscriptomics, metaproteomics, metabolomics  
- Quality control and assembly strategies for microbial communities  
- Functional annotation, pathway reconstruction, and comparative metagenomics  
- Integration of multi-omics layers using statistical and network-based approaches  
- Reproducible workflows with Nextflow and nf-core pipelines

---

### 5. SLUBI SIDA Training Course — Reproducible Bioinformatics, Best Practices, Nextflow & nf-core (Researcher course)
**Role:** Instructor  
**Topics covered:**  
- FAIR data principles and reproducible scientific workflows  
- Introduction to workflow managers (Nextflow)  
- Building and running nf-core pipelines  
- Containerization (Docker, Singularity/Apptainer)  
- Version control with GitHub  
- Designing transparent and reproducible bioinformatics analyses in collaborative environments

---

### 6. MedBioInfo — Swedish National Graduate School in Medical Bioinformatics (PhD course)
**Role:** Teaching assistant / Guest instructor  
**Topics covered:**  
- Medical bioinformatics fundamentals  
- Genome-scale analysis pipelines  
- Statistical modeling of biological data  
- Reproducibility and data stewardship  
- Hands‑on R and bash training targeted at medical datasets

---

## <h2>Details of One Course</h2>

### **3. Data Handling and High‑Quality Illustrations for Publications (PhD course)**

#### **Learning Outcomes**
- Assess data structure and select appropriate graphical representations in R  
- Create multi‑panel publication‑ready figures using **ggplot2**  
- Merge and update datasets programmatically without altering raw data  
- Prepare for reproducible code and data submission using **DOIs**

#### **Content**
- Practical training in R for dataset integration directly from source files, enabling automated updates to figures and maps  
- Data management best practices to avoid unnecessary file duplication and preserve raw data integrity  
- Guidance on selecting effective data visualizations and avoiding misleading graphical elements  
- Introduction to open science principles focusing on reproducible data, scripts, and DOI‑based sharing

The course uses free software within the R ecosystem, including **tidyverse**, **dplyr**, **tidyr**, **ggplot2**, and **patchwork**. GitHub and DOI workflows are integrated throughout the course. Teaching consists of lectures, guided sessions, hands‑on workshops, group exercises based on #tidytuesday datasets, and a final individual project (using students' own data or #tidytuesday datasets). The course runs as a one‑week on‑campus intensive followed by an independent project presented via Zoom.

#### **Formats and Requirements for Examination**
- Independent project presentation  
- Individual written report demonstrating the techniques learned in the course  

</div>
</body>
