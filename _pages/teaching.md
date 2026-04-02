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
<h3>1. Analysis of High-Throughput Sequencing RNA-Seq Data (PhD course)</h3>
<p><strong>Role:</strong> Co-instructor</p>
<p><strong>Lecture:</strong> Interactive teaching focusing on biological interpretation (Q&amp;A format) of RNA‑Seq bioinformatic results.</p>
<p><strong>Lab:</strong></p>
<ul>
    <li>HPC environment setup</li>
    <li>Running Nextflow-based <strong>nf-core/rnaseq</strong> pipelines</li>
    <li>Interpretation of QC metrics, alignment statistics, and expression matrices</li>
    <li>Downstream analysis in R: <strong>DESeq2</strong>, GO &amp; KO enrichment, and biological result validation</li>
</ul>

<hr>

<h3>2. Genome-wide Predictions in Breeding: Genotype–Phenotype Associations and Genomic Selection (PhD course)</h3>
<p><strong>Role:</strong> Co-instructor / Bioinformatics mentor</p>
<p><strong>Lecture:</strong> Introduction to Linux, R &amp; RStudio</p>
<p><strong>Lab:</strong></p>
<ul>
    <li>Hands on Linux &amp; R introduction</li>
    <li>Setup for the GWAS analysis: installation of bioinformatics tools and R packages/functions</li>
</ul>
<p><strong>Topics covered:</strong></p>
<ul>
    <li>Statistical genomics foundations</li>
    <li>SNP calling and variant quality assessment</li>
    <li>GWAS workflows and visualization</li>
    <li>Genomic prediction using mixed models and machine‑learning approaches</li>
    <li>Interpretation of genotype–phenotype associations</li>
    <li>Best practices for reproducible breeding informatics pipelines</li>
</ul>

<hr>

<h3>3. Data Handling and High-Quality Illustrations for Publications (PhD course)</h3>
<p><strong>Role:</strong> Instructor</p>
<p><strong>Topics covered:</strong></p>
<ul>
    <li>Data management strategies in R</li>
    <li>Automated dataset merging, cleaning, and version control</li>
    <li>Creating publication‑quality multi-panel figures with <strong>ggplot2</strong></li>
    <li>Reproducible analysis: project structure, DOIs, and open‑science workflows</li>
    <li>Hands-on sessions with tidyverse and #tidytuesday datasets</li>
</ul>

<hr>

<h3>4. Multi-omics Analyses of the Microbial Community (PhD course)</h3>
<p><strong>Role:</strong> Co-instructor</p>
<p><strong>Topics covered:</strong></p>
<ul>
    <li>Overview of multi-omics: metagenomics, metatranscriptomics, metaproteomics, metabolomics</li>
    <li>Quality control and assembly strategies for microbial communities</li>
    <li>Functional annotation, pathway reconstruction, and comparative metagenomics</li>
    <li>Integration of multi-omics layers using statistical and network-based approaches</li>
    <li>Reproducible workflows with Nextflow and nf-core pipelines</li>
</ul>

<hr>

<h3>5. SLUBI SIDA Training Course — Reproducible Bioinformatics, Best Practices, Nextflow &amp; nf-core (Researcher course)</h3>
<p><strong>Role:</strong> Instructor</p>
<p><strong>Topics covered:</strong></p>
<ul>
    <li>FAIR data principles and reproducible scientific workflows</li>
    <li>Introduction to workflow managers (Nextflow)</li>
    <li>Building and running nf-core pipelines</li>
    <li>Containerization (Docker, Singularity/Apptainer)</li>
    <li>Version control with GitHub</li>
    <li>Designing transparent and reproducible bioinformatics analyses in collaborative environments</li>
</ul>

<hr>

<h3>6. MedBioInfo — Swedish National Graduate School in Medical Bioinformatics (PhD course)</h3>
<p><strong>Role:</strong> Teaching assistant / Guest instructor</p>
<p><strong>Topics covered:</strong></p>
<ul>
    <li>Medical bioinformatics fundamentals</li>
    <li>Genome-scale analysis pipelines</li>
    <li>Statistical modeling of biological data</li>
    <li>Reproducibility and data stewardship</li>
    <li>Hands‑on R and bash training targeted at medical datasets</li>
</ul>

<hr>

<h2>Details of One Course</h2>

<h3>3. Data Handling and High‑Quality Illustrations for Publications (PhD course)</h3>

<h4>Learning Outcomes</h4>
<ul>
    <li>Assess data structure and select appropriate graphical representations in R</li>
    <li>Create multi‑panel publication‑ready figures using <strong>ggplot2</strong></li>
    <li>Merge and update datasets programmatically without altering raw data</li>
    <li>Prepare for reproducible code and data submission using <strong>DOIs</strong></li>
</ul>

<h4>Content</h4>
<ul>
    <li>A practical overview of handling data in R, including merging datasets directly from the original data files within R. This enables automatic updates to illustrations and maps.</li>
    <li>Data handling strategies to avoid multiple dataset versions and preserve raw data integrity, especially in projects with continuous updates.</li>
    <li>Guidance on selecting suitable figures to convey dataset characteristics and what to avoid.</li>
    <li>An introduction to open science with emphasis on reproducible data, scripts, and DOI-based sharing.</li>
</ul>

<p>
The course uses free software within the R environment, including packages such as <strong>tidyverse</strong>, <strong>dplyr</strong>, <strong>tidyr</strong>, <strong>ggplot2</strong>, and <strong>patchwork</strong>.  
GitHub is used for DOI and data sharing.  
#tidytuesday datasets are used extensively for exercises.  
Teaching includes lectures, presentations, hands-on workshops, group work, and a final individual project using students’ own data or #tidytuesday datasets.  
The course is delivered as a one‑week on‑campus class followed by an independent project presented via Zoom.
</p>

<h3>Formats and Requirements for Examination</h3>
<ul>
    <li>The course objectives are examined through independent project presentations and individual written reports on the techniques used.</li>
</ul>

</div>