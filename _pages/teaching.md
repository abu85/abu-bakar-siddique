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
        }
        @media (max-width: 600px) {
            .youtube-container {
                width: 100%; /* Full width on small screens */
                max-width: none; /* Remove max width on small screens */
            }
        }
    </style>
</head>
<body>
    <div class="intro">
        <h3>- Analysis of High-Throughput Sequencing RNA-Seq Data (PhD course)</h3>
        <h3>- Genome-wide predictions in breeding: genotype-phenotype associations and genomic selection (PhD course)</h3>
        <h3>- Data handling and high-quality illustrations for publications (PhD course)</h3>
        <h3>- Multi-omics analyses of the microbial community (PhD course)</h3>
        <h3>- SLUBI SIDA training course—Reproducible bioinformatics, best practices, Nextflow and nf-core (researcher course)</h3>
        <h3>- MedBioInfo —Swedish National Graduate School in Medical Bioinformatics (PhD course)</h3>
        <h4>Details of the one: Data handling and high-quality illustrations for publications (PhD course)</h4> 
        <ul>
            <h4>Learning outcome</h4>
            <ul>
            <li> Assess their data, choose and create suitable graphs with R.
            <li> Create multi-panel figures for publications and presentation with R.
            <li>Merge and update datasets in R without the need to modify the source data files.
            <li>Plan for code and raw data submission by creating Digital Object Identifiers (DOIs) to be used for publications.<br>
            <h4>Content</h4>
            <ul>
            <li>A practical overview of handling data in R, including merging datasets directly from the original data files within R. During the course this knowledge will be used to automatically update illustrations and maps. Learning a proper Data handling strategy is important to minimize the usual multiple versions of the dataset(s) that are created by many students. At the same time, it is important to preserve the original data to prevent irreversible errors due to manual handling. This is of particular interest in many projects where data is added and updated continuously.
                <li>A practical and theoretical background to choose suitable figures to convey graphically the nature of a specific dataset and what to avoid.
                <li>An introduction to open science, with an emphasis on reproducible data and scripts, and sharing these through DOIs.
                <p>The course will use free software within the R environment, including packages such as tidyverse, dplyR, tidyR, and ggplot2. For DOI and data sharing, GitHub will be used. The #tidytuesday project on GitHub will be the primary source of example datasets. Theoretical lectures will be mixed with presentations and hands-on workshops. Students will work in groups to solve given problems that tie back to the lectures using #tidytuesday data. A final individual project will be given where the students will use their own data (when available) or use the #tidytuesday datasets to implement the learning objectives and present their project. Teaching will be conducted as a one week on-campus class followed by an independent project that will be presented via zoom.</p><br>
            <h4>Formats and requirements for examination</h4>
            <ul>
                <li>The course objectives will be examined through independent project presentations and individual written reports on the use of different techniques included in the course. 