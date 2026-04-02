---
layout: single
permalink: /training/
author_profile: true
classes: wide
---

<head>
    <!-- Font Awesome Icons -->
        <style>
        h3 {
            margin-top: 0;
            margin-bottom: 0;
            padding-left: 5px;
        }
        .intro ul {
            margin-top: 4px;
            margin-bottom: 0;
            list-style-type: square;
        }
        .intro p {
            margin-top: 0;
            margin-bottom: 0;
            color: gray;
            font-size: 80%;
        }
        /* ✅ TOGGLE STYLES */
        .toggle-content {
            display: none;
            opacity: 0;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s ease, opacity 0.5s ease;
            margin-bottom: 20px;
            font-size: 80%;
        }
        .toggle-button {
            cursor: pointer;
            display: flex;
            align-items: center;
            user-select: none;
            margin-bottom: 15px;
            font-weight: bold;
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
            max-height: 1000px;
        }
        /* YouTube styling (unchanged) */
        .youtube-container {
            position: relative;
            width: 66.66%;
            max-width: 100%;
            padding-bottom: 37.5%;
            height: 0;
            margin-bottom: 40px;
        }
        .youtube-iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        @media (max-width: 600px) {
            .youtube-container {
                width: 100%;
                max-width: none;
            }
        }
    </style>
    <!-- ✅ REQUIRED Javascript for Toggle to work -->
    <script>
        function toggleSection(id) {
            const content = document.getElementById(id);
            const button = document.querySelector(`[onclick="toggleSection('${id}')"]`);
            content.classList.toggle('show');
            button.classList.toggle('active');
        }
    </script>
</head>

<h1>Bioinformatics training materials</h1>

<body>
<div class="intro">
<!-- 1. RNA-Seq Training -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t1')">
    <span><i class="fas fa-dna"></i> 1. Analysis of High-Throughput RNA‑Seq Data</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t1" class="toggle-content">

<p><strong>Quick start:</strong>
    <li><a href="[def]" target="_blank">
    pixi + nextflow RNA‑Seq workflow
    </a></li>
    <li><a href="https://abu85.github.io/Pixi-in-bioinformatics/modules/snakemake_rnaseq_analysis.html" target="_blank">
        pixi + snakemake RNA‑Seq workflow
    </a></li>
</p>

<p><strong>Overview:</strong> End‑to‑end RNA‑Seq workflow training covering raw FASTQ processing, QC, mapping, quantification, and differential expression.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>Nextflow + nf-core/rnaseq Or</li> 
    <li>Snakemake custom script</li>
    <li>FastQC, MultiQC</li>
    <li>STAR or HISAT2</li>
    <li>featureCounts</li>
    <li>DESeq2, clusterProfiler for GO/KO</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>QC reports</li>
    <li>Aligned BAM files</li>
    <li>Count matrices</li>
    <li>Differential expression tables</li>
    <li>Functional enrichment plots</li>
</ul>

</div>
</div>

<hr>

<!-- 2. GWAS / Genomic Prediction -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t2')">
    <span><i class="fas fa-seedling"></i> 2. Genome-Wide Predictions in Breeding (GWAS & GS)</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t2" class="toggle-content">

<p><strong>Training material:</strong> 
    <a href="https://abu85.github.io/intro-to-R-genomic-selection/" target="_blank">
        Genomic Prediction Workshop
    </a>
</p>

<p><strong>Overview:</strong> Hands‑on introduction to variant processing, GWAS pipelines, mixed models, and genomic prediction techniques.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>PLINK for SNP QC</li>
    <li>GEMMA / MLMM for GWAS</li>
    <li>R packages: rrBLUP, BGLR, sommer</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>Filtered genotype sets</li>
    <li>Manhattan/QQ plots</li>
    <li>GWAS hit tables</li>
    <li>Genomic Estimated Breeding Values (GEBVs)</li>
</ul>

</div>
</div>

<hr>

<!-- 3. Data Handling & Visualization -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t3')">
    <span><i class="fas fa-chart-bar"></i> 3. Data Handling & High‑Quality Figures in R</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t3" class="toggle-content">

<p><strong>Training material:</strong>
    <a href="https://abu85.github.io/data-handling-visualization-in-R/" target="_blank">
        Data Visualization in R
    </a>
</p>

<p><strong>Overview:</strong> Training on efficient data wrangling, multi‑table merging, and reproducible, publication-grade figure creation in R.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>tidyverse: dplyr, tidyr, readr</li>
    <li>ggplot2 + patchwork</li>
    <li>rmarkdown</li>
    <li>GitHub for versioning</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>Tidy & merged data structures</li>
    <li>Statistical graphics</li>
    <li>Multi-panel figures</li>
    <li>Reproducible reports</li>
</ul>

</div>
</div>

<hr>

<!-- 4. Microbial Multi‑Omics -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t4')">
    <span><i class="fas fa-bacteria"></i> 4. Multi‑omics Analysis of Microbial Communities</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t4" class="toggle-content">

<p><strong>Training material:</strong> 
    <a href="[def2]" target="_blank">
        Metagenomics & Multi‑omics Training
    </a>
</p>

<p><strong>Overview:</strong> End‑to‑end training covering metagenomic assembly, binning, taxonomy, and functional annotation.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>nf-core/mag</li>
    <li>Kraken2 + Bracken</li>
    <li>MetaBAT2, MaxBin</li>
    <li>Prokka, eggNOG-mapper</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>Taxonomic profiles</li>
    <li>MAGs (assembled genomes)</li>
    <li>Functional annotation reports</li>
    <li>Pathway reconstructions</li>
</ul>

</div>
</div>

<hr>

<!-- 5. Reproducible Bioinformatics Training -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t5')">
    <span><i class="fas fa-recycle"></i> 5. Reproducible Bioinformatics, Nextflow & nf-core</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t5" class="toggle-content">

<p><strong>Training material:</strong>
    <a href="https://abu85.github.io/Reproducible_Bioinformatics/" target="_blank">
        Reproducible Bioinformatics Workshop
    </a>
</p>

<p><strong>Overview:</strong> A fully hands‑on introduction to reproducible bioinformatics workflows using containers, CI, and modern pipeline design.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>Nextflow scripting</li>
    <li>nf-core template + modules</li>
    <li>Docker, Apptainer</li>
    <li>GitHub Actions for CI</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>Reusable Nextflow pipelines</li>
    <li>Containerized reproducible environments</li>
    <li>Automated CI testing</li>
    <li>Releases with version tracking</li>
</ul>

</div>
</div>

<hr>

<!-- 6. MedBioInfo -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t6')">
    <span><i class="fas fa-user-graduate"></i> 6. MedBioInfo — Medical Bioinformatics</span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t6" class="toggle-content">

<p><strong>Training material:</strong> 
    <a href="https://medbioinfo.se/training/modules" target="_blank">
        MedBioInfo Training Modules
    </a>
</p>

<p><strong>Overview:</strong> Modules covering biomedical data analysis, clinical genomics, multi‑omics, and statistical learning.</p>

<p><strong>Tools included:</strong></p>
<ul>
    <li>R/Bioconductor workchains</li>
    <li>Bash automation</li>
    <li>Variant calling & annotation tools</li>
    <li>Machine‑learning packages</li>
</ul>

<p><strong>Results generated:</strong></p>
<ul>
    <li>Clinical variant tables</li>
    <li>DGE and expression matrices</li>
    <li>Prediction model outputs</li>
    <li>Exploratory and diagnostic plots</li>
</ul>

</div>
</div>

<hr>

<!-- 7. Other complete resources list -->
<div class="course-block">
<div class="toggle-button" onclick="toggleSection('t7')">
    <span>
        <i class="fas fa-bacteria"></i>
        Bioinformatics training materials compiled by SIB (GLITTR)
    </span>
    <i class="fas fa-chevron-right"></i>
</div>

<div id="t7" class="toggle-content">

<p><strong>Overview:</strong>
This is a curated and actively maintained collection of bioinformatics training
materials compiled by the Swiss Institute of Bioinformatics (SIB) and integrated
into <a href="https://glittr.org" target="_blank">glittr.org</a>.
</p>

<p>
All resources in this collection are:
</p>
<ul>
    <li>Free and openly accessible</li>
    <li>Hosted on GitHub or GitLab</li>
    <li>Written in Markdown or similar formats</li>
    <li>Cover a wide range of bioinformatics topics</li>
</ul>

<p><strong>Live README (auto-updated):</strong></p>

<iframe
    src="https://github.com/sib-swiss/training-collection/blob/main/README.md?plain=1"
    width="100%"
    height="800px"
    style="border:1px solid #ccc; border-radius:6px;">
</iframe>

<p style="margin-top:10px;">
🔗 <a href="https://github.com/sib-swiss/training-collection/blob/main/README.md" target="_blank">
Or click on here to see if avobe window does not show up
</a>
</p>

<p style="margin-top:10px;">
🔗 <a href="https://glittr.org" target="_blank">
Visit GLITTR for the full interactive platform
</a>
</p>

</div>
</div>


[def]: ttps://abu85.github.io/Pixi-in-bioinformatics/modules/nextflow_rnaseq_analysis.htm
[def2]: ttps://abu85.github.io/nfcore_metagenomics_training