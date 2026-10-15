---
layout: single
permalink: /research/
author_profile: true
classes: wide
toc: true
toc_label: "On this page"
toc_sticky: true
---

# Research Story

Six chapters of a research life spent moving between the bench and the terminal — from screening *Trichoderma* and leaf botanicals against a mustard pathogen in Bangladesh, through counting fungal endophytes in aspen and beech leaves, a detour into mycoviruses, a long-running airborne eDNA archive, and now facilitating bioinformatics infrastructure for an entire university.

---

## Biological Control of Crop Disease — Bangladesh

This is where the research life actually began, before any of the mycobiome or sequencing work: a BSc (Hons) in Agricultural Sciences and an MSc in Plant Pathology, both at Sher-e-Bangla Agricultural University, Bangladesh (2008 and 2010). The MSc thesis asked a very applied question — **how do you control leaf blight of mustard without leaning entirely on synthetic fungicides?** The answer I tested was two-sided: *Trichoderma* species as a fungal biocontrol agent, and selected leaf botanicals (plant-derived extracts) as a complementary, lower-input alternative, alongside characterising how variable the pathogen itself was across isolates.

It was hands-on plant pathology in the most literal sense — isolating the pathogen, running in vitro and pot-based bioassays, scoring lesion severity across treatments, and learning early on that a "biological" solution has to be benchmarked against real variability in the thing it's trying to control, not just a single reference strain. That same interest in fungi as allies rather than only as targets resurfaced more than a decade later in a review synthesising the broader case for endophytic fungi as a natural resource for sustainable crop production under climate change, written with the same Bangladeshi collaborator network I trained alongside (*Symbiosis*, 2023, [doi:10.1007/s13199-022-00879-4](https://doi.org/10.1007/s13199-022-00879-4)).

*(A good figure here: a bar chart from the MSc thesis comparing leaf blight lesion severity across the Trichoderma, botanical, and untreated control groups.)*

**Skills learned / applied:** pathogen isolation and culturing; in vitro and pot-based biocontrol bioassays; screening & culturing of fungal antagonists (*Trichoderma* spp.) and plant-derived botanicals for antifungal efficacy; assessing phenotypic variability across pathogen isolates; foundational plant pathology and experimental design — the base everything since has built on.

---

## Aspen Mycobiome

This is where it started. For my MSc thesis at Umeå University (2013, supervised by Assoc. Prof. Benedicte R. Albrectsen), I looked at the endophytic fungi living inside aspen (*Populus tremula*) leaves, and asked a simple question: **does insect herbivory change who lives there?** The thesis compared fungal communities in leaves with and without beetle damage, and it was my first real exposure to the whole pipeline — from field sampling to culturing in petridish to PCR to to identifying to interpreting a community dataset. [Thesis (DiVA)](https://umu.diva-portal.org/smash/record.jsf?pid=diva2:655908)

That question came back years later, once I had proper amplicon-sequencing tools instead of culturing plates. Together with Benedicte Albrectsen we returned to it at scale, showing that both plant genotype and herbivory shape the aspen endophyte community — not just one or the other (*Oecologia*, 2018, [doi:10.1007/s00442-018-4097-3](https://doi.org/10.1007/s00442-018-4097-3)). Around the same period I also helped optimise a protocol for building fungal ITS amplicon libraries specifically for the aspen mycobiome work, aimed at making high-throughput Illumina sequencing of these communities cheaper and more consistent (*Applied Sciences*, 2022, [doi:10.3390/app12031136](https://doi.org/10.3390/app12031136)).

*(A good figure here would be an ordination plot — PCoA or NMDS — from the Oecologia paper showing genotype × herbivory separation of fungal communities.)*

**Skills learned / applied:** field sampling design; DNA extraction and PCR from plant tissue; fungal ITS amplicon library preparation for Illumina; early community-ecology statistics (ordination, permutation tests); first hands-on experience turning a biological question into a sequencing experiment.

---

## Beech Endophytes

My PhD (Dr. rer. nat., Greifswald University, 2013–2017, supervised by PD Dr. Martin Unterseher) is where the aspen question became a research programme: how do leaf-inhabiting fungal communities respond to habitat, biochemistry, and season? The cumulative thesis pulled together several studies on beech (*Fagus sylvatica*) leaf mycobiomes across altitudinally distinct sites in Germany, tracked over two years. [Thesis](https://nbn-resolving.org/urn:nbn:de:gbv:9-002881-5)

The first output was methodological, and it's the paper I still get cited for: a cost-effective, efficient Illumina sequencing strategy for fungal communities, using the beech endophyte system as the case study and identifying elevation as the main driver of diversity and composition (*Fungal Ecology*, 2016, [doi:10.1016/j.funeco.2015.12.009](https://doi.org/10.1016/j.funeco.2015.12.009)). In parallel, work with Martin Unterseher and colleagues showed that habitat conditions and leaf biochemistry together shape beech leaf mycobiome composition (*PLOS ONE*, 2016, [doi:10.1371/journal.pone.0152878](https://doi.org/10.1371/journal.pone.0152878)).

A second strand asked a more methodological question that mattered a lot at the time: what do culture-based surveys miss compared to high-throughput sequencing, and what do they still tell us that sequencing doesn't? Working with MSc student Anis Mahmud Khokon (whom I co-supervised), we compared cultivation and sequencing of beech leaf endophytes and found the two approaches gave complementary - not redundant - pictures of the community (*MycoKeys*, 2017, [doi:10.3897/mycokeys.20.11265](https://doi.org/10.3897/mycokeys.20.11265)). Years later I returned to the beech system once more, this time asking whether mycobiomes are organised more by plant organ (leaf vs. twig) than by habitat — they are, and the twig fungi showed signs of competing with each other (*Frontiers in Microbiology*, 2021, [doi:10.3389/fmicb.2021.646302](https://doi.org/10.3389/fmicb.2021.646302)).

*(A good figure here: the elevation-vs-diversity relationship from the Fungal Ecology 2016 paper, or a community-composition barplot from PLOS ONE 2016.)*

**Skills learned / applied:** designing and running a multi-year, multi-site sampling programme; amplicon bioinformatics pipelines (OTU/ASV-era tools); comparative culture-dependent vs. culture-independent methodology; community ecology statistics (diversity indices, ordination, mixed models); co-supervising a thesis student through to publication; academic writing and thesis composition.

---

## Mycovirus

After the PhD I took a sideways step into virology, 2018–2019 as a mobility postdoctoral fellow at the Institute of Plant Molecular Biology, Biology Centre CAS, in České Budějovice, Czech Republic. The question changed scale — from fungal communities to what infects individual fungi. I worked on identifying and characterising mycoviruses in endophytic and pathogenic forest fungi, combining dsRNA and total RNA extraction, RT-PCR, cloning and phylogenetics with expression analysis, and asked what viral infection does to fungal growth and whether it could be turned into a biological control strategy against fungal plant disease.

One concrete case from that period: a mycoparasitic and opportunistic fungus found to be inhabited by a mycovirus, worked out with Karel Petrzik (*Archives of Virology*, 2019, [doi:10.1007/s00705-019-04359-x](https://doi.org/10.1007/s00705-019-04359-x)). I later pulled the broader picture together as a sole-authored review of viruses found in endophytic and pathogenic forest fungi (*Virus Genes*, 2020, [doi:10.1007/s11262-020-01763-3](https://doi.org/10.1007/s11262-020-01763-3)) — the first paper I wrote entirely on my own, and a useful exercise in synthesising a scattered literature into one coherent argument.

*(A good figure here: a phylogenetic tree of mycovirus sequences, or an RT-PCR gel image confirming viral dsRNA presence.)*

**Skills learned / applied:** dsRNA and total RNA extraction from fungal tissue; RT-PCR and cloning; phylogenetic tree building and interpretation (MAFFT, RAxML, MrBayes); viral genome characterisation; literature synthesis and independent scientific writing.

---

## SweBITS

Back in Sweden, at Umeå University's Department of Ecology & Environmental Sciences (postdoc 2020–2022, then briefly Senior Research Engineer in early 2022), I joined SweBITS — Swedish Biodiversity in Time and Space — a project built around a genuinely unusual resource: a 34-year archive of weekly aerosol filters collected in northern Sweden (Kiruna). The core idea was to **reconstruct historical biodiversity from airborne eDNA** trapped on filters that had simply been sitting in storage, filter by filter, week by week, for over three decades.

My part was to turn that archive into biodiversity and biosurveillance signal: reconstructing fungal and wider community trends from the filter sequences, assembling reference genomes for forest fungal pathogens so they could be traced through the archive, and integrating the sequence-derived community data with weather and land-use records to model seasonal patterns and outbreak risk — an early-warning approach to biosurveillance. The scale of the project meant the results took years to fully mature into publications: the headline paper showing that airborne eDNA captures three decades of ecosystem biodiversity appeared in *Nature Communications* in 2025 ([doi:10.1038/s41467-025-67676-7](https://doi.org/10.1038/s41467-025-67676-7)), with a companion study on rapid shifts in bryophyte phenology revealed by the same airborne eDNA archive in *Journal of Ecology* the same year ([doi:10.1111/1365-2745.70180](https://doi.org/10.1111/1365-2745.70180)).

*(A good figure here: the multi-decade biodiversity trend plot from the Nature Communications paper — it's the single most visually compelling result from this chapter.)*

**Skills learned / applied:** large-scale environmental eDNA metabarcoding and shotgun metagenomics; reference genome assembly for non-model fungal pathogens; integrating sequence data with independent environmental time series (weather, land use); long-horizon project thinking — data generated years before the analysis that made sense of it; HPC-scale processing (HPC2N).

---

## SLUBI

Since 2022 I've been on the infrastructure side rather than running my own research questions — first as a Research Engineer, then since June 2024 as Bioinformatician, within SLU's Bioinformatics Infrastructure (SLUBI) in the Department of Plant Biology, Uppsala. The job is different in kind from everything above: instead of one long research thread, it's dozens of other people's questions, each needing the right method, run cleanly on HPC, and handed back as something they can rerun themselves or use for publication. Over 4.5 years that has added up to 40 SLUBI projects for 120+ people, spanning metagenomics, metatranscriptomics, RNA-seq, genome assembly and more, plus designing and teaching the reproducibility, genomic selection, RNA-seq and multi-omics courses that pass those practices on.

A good share of the publications elsewhere in this story exist because of this role rather than in spite of it: the transcriptomic analyses behind studies of beet mild yellowing virus (*BMC Plant Biology*, 2025, [doi:10.1186/s12870-025-07514-6](https://doi.org/10.1186/s12870-025-07514-6)), potato mop-top virus in *Nicotiana benthamiana* (*Molecular Plant-Microbe Interactions*, 2026, [doi:10.1094/MPMI-10-25-0146-R](https://doi.org/10.1094/MPMI-10-25-0146-R)), turnip yellows virus risk under milder autumns (*Phytopathology*, 2023, [doi:10.1094/PHYTO-11-22-0446-V](https://doi.org/10.1094/PHYTO-11-22-0446-V)), and facemask waste effects on freshwater fungal communities (*Scientific Reports*, 2026, [doi:10.1038/s41598-026-45795-5](https://doi.org/10.1038/s41598-026-45795-5)) all ran through SLUBI. It's a role built on making other people's science reproducible rather than authoring the headline result myself — which suits the infrastructure-builder instinct better than the sole-author-review instinct from a few years earlier.

*(A good figure here: a screenshot of one of the Nextflow/nf-core pipeline DAGs you run most often, or a simple diagram of the SLUBI service model — request in, method chosen, HPC run, code handed back.)*

**Skills learned / applied:** Nextflow/nf-core and Snakemake pipeline engineering across omics types; SLURM/HPC operations across NAISS systems (UPPMAX, PDC Dardel, HPC2N); containerisation (Docker, Singularity/Apptainer, Conda); running many concurrent projects for many different research groups; course design and teaching at researcher and PhD level; translating a biologist's question into a reproducible, handoff-ready analysis.

---

*Figure placeholders above mark where a screenshot or exported plot from the cited paper (or your own pipeline output) would fit — I don't have access to the actual published figures to embed directly, so drop in image files and I can wire up the markdown links once you have them.*
