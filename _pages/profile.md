---
layout: single
permalink: /profile/
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
        <h3>Bioinformatic project accomplishments</h3> 
        <ul>
            <li> Nine ampliseq data analysis:</li>            
                <ol>
                    <li>ITS: Leaf inhabiting fungal endophytes of European Aspen tree</li>
                    <li>ITS: Leaf inhabiting fungal endophytes of European Beech tree</li>
                    <li>ITS: Leaf inhabiting fungal endophytes of Rye seeds and soils</li>
                    <li>18S: Sequencing of Arbuscular Mycorrhizal (AMF) Communities in Environmental Samples</li>
                    <li>COI: Wildflowers inhabiting terrestrial arthropods</li>
                    <li>ITS: Metagenomics of seeds (empty vs filled)</li>
                    <li>16S: Leaf inhabiting fungal endophytes of Rye seeds and soils</li>
                    <li>16S: Water samples of different rivers of Bangladesh</li>
                    <li>16S: Human Gut microbiome</li>
                </ol></li>
            <li> Three metagenomics data analysis:
            <ol>
                <li>Airfilter data</li>
                <li>Leaf litter data (Alder)</li>
                <li>Human gut microbiome</li>
            </ol>
            <li> Ten RNASeq HTS data analysis and downstream analysis:
            <ol>
                <li>Sugarbeet1</li>
                <li>Sugarbeet2</li>
                <li>Potato1</li>
                <li>Potato2</li>
                <li>Potato3</li>
                <li>Brassica oleracea</li>
                <li>Red clover1</li>
                <li>Red clover2</li>
                <li>QTLSeq</li>
                <li>Meta transcriptome Bioreactor</li>
            </ol>
        </ul>
        <br>
        <h3>Research Interests</h3> 
        <ul>
            <li>Environmental Metagenomics and Molecular Ecology
            <p>Environmental monitoring (Disease and pest by Airborne eDNA), bryophyte phenology, metabarcoding, biodiversity, disease resistance</p></li>
            <li>Computational Multi-Omics
            <p>Genome, transcriptome; AI-driven analysis (ML & DL)</p></li>
        </ul>
        <br>
        <h3>Education</h3>
        <ul>
            <li>Ph.D., Molecular Ecology (12/2013 – 09/2017)
            <p>Greifswald University, Germany</p></li>
            <li>M.S., Ecology (08/2010 – 05/2013)
            <p>Umeå University, Umeå, Sweden</p></li>
            <li>M.S., Plant Pathology (03/2008 – 07/2010)
            <p>Sher-e-Bangla Agricultural University, Dhaka, Bangladesh</p></li>
            <li>B.Sc.Ag(Hons), Agriculral Science (01/2004 – 03/2008)
            <p>Sher-e-Bangla Agricultural University, Dhaka, Bangladesh</p></li>            
        </ul>
        <br>
        <h3>Research projects</h3>
        <ul>
            <li>TanAsp (mycobiome and metabolites in European Aspen)
            <li>Sweden Biodiversity in Time and Space (SweBITS) through meta-genomics
            <li>Mycoviruses
            <li>Leaf-inhabiting endophytes of European beech trees
            <li>Plant-fungi-insect interaction in Swedish Aspen</li>
        </ul>            
        <h3>Research Experience</h3>
        <ul>
            <li>Bioinformatician (Bioinformatiker), <a href="https://www.slu.se/en/profilepages/s/abu-siddique/" target="_blank" style="color: inherit; ">SLUBI</a> (06/2024 – Continue)
            <p>Department of plant biology, SLU - Swedish University of Agricultural Sciences, Uppsala, Sweden<br>
            Research topics: <u>Metagenomics(ITS, 16S, COI, 18S, eDNA: Short reads)</u>, <u>SLUBI</u></p></li>  
            <li>Research Engineer (Forskningsingenjör), 2022-02-15 to 2024-05-31
            <p>Department of Plant Biology, SLU - Swedish University of Agricultural Sciences, Uppsala, Sweden<br>
            Research topics: <u>airborne eDNA</u>, <u>bryophyte phenology</u>, <u>multi-omics integration</u></p></li>  <li>Senior Research Engineer (Senior forskningsingenjör), 2022-01-06 to 2022-02-15
            <p>Department of Ecology and Environmental Sciences, Umeå University, Umeå, Sweden<br>
            Research topics: <u>environmental metagenomics</u>,<u>airborne eDNA</u>, <u>bryophyte phenology</u>, <u>data integration</u></p></li>
            <li>Post-doc Research Fellow (Forskare), from 2020-01-06
            <p>Department of Ecology and Environmental Sciences, Umeå University, Umeå, Sweden<br>
            Research topics: <u>airborne eDNA</u>, <u>bryophyte phenology</u>, <u>multi-omics integration</u>,<u>phenology</u></p></li>
            <li>Post-doc Research Fellow (Forskare), 2018-07-09 to 2019-10-31
            <p>Department of Virology, Institute Of Plant Molecular Biology, Biology Centre CAS, Ceske Budejovice, Czech Republic<br>
            Research topics: <u>Fungal virology</u>, <u>molecular biology</u></p></li>
            <li>PhD Student (Doktorand), 2013-12-01 to 2017-05-31
            <p>Institute of Botany and Landscape Ecology, Ernst-Moritz-Arndt Universität (Greifswald University),Greifswald, Germany<br>
            Research topics: <u>Leaf inhabiting endophytic fungi</u>, <u>ITS metabarcoding</u></p></li>
            <li>Research Assistant (Forskningsassistent), 2012-07-01 to 2012-09-30
            <p>Department of Plant Physiology, UPSC, Umeå University, Sweden<br>
            Research topics: <u>fungal endophytes</u>, <u>molecular ecology</u></p></li>
        </ul>
            <p><i>Note: Family leave for approximately nine months after PhD studies (2017–2018).</i></p>
            <br>
