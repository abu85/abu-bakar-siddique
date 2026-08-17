<div align="center" style="background:#006AA7; color:#FECC02; padding:28px 18px; border-radius:10px;">

# Bioinformatics for Agricultural Sciences in the Age of AI

### A practical guide for students in plant, animal, forest, veterinary and food sciences — 2026 edition

</div>

<br>

> **TL;DR** — Agriculture is not medicine with tractors. Your data has environments, seasons, pedigrees and a farmer at the end of the pipeline. The AI models are exciting, but the field's oldest tool — the mixed model — is still beating a lot of them. Learn why, and you'll be more useful than someone who only knows how to fine-tune.

---

<h2 style="color:#006AA7;">Why agricultural bioinformatics is its own discipline</h2>

If you read a general "learn bioinformatics with AI" guide, it was almost certainly written about human biomedicine. Much of it transfers. But five things make agricultural data genuinely different, and they shape what you should learn:

1. **Genotype × Environment is the whole game.** A wheat line that yields brilliantly in Skåne may fail in Norrland. In human genetics, environment is a nuisance variable. In yours, it's the object of study.
2. **The phenotype is the bottleneck, not the genotype.** Sequencing got absurdly cheap. Measuring 5,000 plots for lodging, or 200 cows for methane emission, did not.
3. **Generation time is measured in seasons or years.** You cannot iterate the way a cell-line lab can. This puts enormous weight on *prediction* — which is exactly why quantitative genetics matured here first.
4. **Structure everywhere.** Pedigrees, family structure, population stratification, repeated measures across years and locations. Ignore it and your model will look wonderful and predict nothing.
5. **There is a regulatory and commercial endpoint.** Variety registration, breeding value publication, feed regulations, and — as of this summer — a brand-new EU framework for gene-edited plants.

Your comparative advantage as an agricultural student is that you understand all five. The advantage of learning bioinformatics is that you can then act on them at scale.

---

<h2 style="color:#006AA7;">Part 1 — What actually changed by 2026</h2>

### Plants got their own genomic language models

The DNA foundation model wave reached plants properly. **AgroNT** (roughly 991M parameters, pretrained on 48 plant genomes) opened the door; **PlantCaduceus** followed with single-nucleotide tokenization and a Mamba architecture that is natively reverse-complement-equivariant; **PlantCAD2** scaled this to longer context windows; and **BOTANIC-0** arrived in early 2026 as a further series of plant-specific models. Standardized evaluation now runs through the **Plant Genome Benchmark**, covering tasks like promoter and terminator strength, splice site detection and non-coding RNA classification.

The claim these papers make is worth understanding precisely: multispecies pretraining lets you predict regulatory features, tissue-specific expression and functional variants **even in species with sparse experimental annotation**. For agricultural genomics, where most crop and livestock species have a fraction of the functional annotation that human and mouse enjoy, that is the point. There is also **scPlantLLM** for plant single-cell atlases, and general-purpose models like **Evo 2** and **AlphaGenome** that are relevant across kingdoms.

### Pangenomes replaced the single reference

Sticking every accession against one reference genome throws away exactly the variation breeders care about. A sorghum pangenome reference published in *Nature* in 2026 demonstrated improved global trait discovery, and the field is now talking about **super-pangenomes** — genus-wide frameworks that fold in wild relatives to capture structural variation, rare alleles and regulatory elements behind stress adaptation.

Practical consequence for you: learn graph-based and pangenome-aware tooling, and get comfortable with structural variants. "SNPs against one reference" is becoming the legacy workflow.

### Phenomics finally became a data problem instead of a labour problem

UAV and ground-based platforms with multispectral, hyperspectral and LiDAR sensors now generate phenotype data faster than anyone can analyse it. The bottleneck moved from *acquiring* images to *extracting phenotypes from them and analysing the volume*. This is where computer vision meets your field trial, and where a student who can do both plot segmentation and a proper spatial field-trial analysis is genuinely rare.

Adjacent to this is **envirotyping** — characterizing environments as carefully as you characterize genotypes — which is the only honest way to model G×E.

### Microbiome work went predictive

Soil, rumen and rhizosphere microbiome studies have moved from "who is there" to "what will happen." Random forests, gradient boosting and deep models are being used to predict community composition, infer functional potential, and model ecosystem processes like CO₂ and N₂O emissions from combined sensor, environmental and metagenomic data. Note the honest caveat from a 2026 *Scientific Reports* study: predictions were generally more accurate at **higher taxonomic levels** like phylum and class. Fine-grained prediction remains hard.

### The regulatory ground shifted under plant breeding

On 17 June 2026 the European Parliament gave final approval to the EU regulation on plants obtained through **new genomic techniques (NGTs)**, published in the Official Journal on 26 June and in force from 16 July 2026 as Regulation (EU) 2026/1388. Most provisions apply after a 24-month transition, so the framework is expected to bite from **mid-2028**.

The structure matters for anyone doing plant genomics in Europe:

- **Category 1** — plants that could have arisen naturally or through conventional breeding (targeted mutagenesis, cisgenesis). Simplified pathway, verified by national authorities and the Commission, no GMO risk assessment, labelling on seed and reproductive material rather than the final product. Herbicide-tolerant plants are excluded from this category.
- **Category 2** — remains under the existing GMO framework.
- All NGT plants go into a **public database** and are banned from organic production. Member states can restrict Category 2 cultivation.
- Patent information must be declared publicly, with a dedicated expert group and a Commission study on patenting impacts due one year after entry into force.

Why does a bioinformatics student care? Because "could this have arisen by conventional breeding?" is, at bottom, a **sequence and provenance question**. Documenting edits, proving equivalence, and maintaining auditable data lineage is going to be somebody's job. It should probably be someone who understands both the genome and the pipeline.

---

<h2 style="color:#006AA7;">Part 2 — The reality check that should shape your training</h2>

This is the section that separates a useful agricultural bioinformatician from someone who read a press release.

**Deep learning has not swept genomic selection.** A 2025 study compared deep learning against **GBLUP** across 14 real plant breeding datasets with careful per-dataset hyperparameter tuning. Deep learning did capture non-linear patterns and often predicted better, especially on smaller datasets — but **neither approach consistently won across all traits and scenarios**, and DL performance depended heavily on rigorous tuning. The authors' conclusion was explicitly about complementarity, not replacement.

The livestock literature says the same thing in a different accent:

- In beef cattle, GBLUP achieved the highest accuracy for birth weight and yearling weight, while Random Forest won on weaning weight — and GBLUP showed superior model fit overall.
- In a 2026 layer chicken study, Random Forest performed best for egg shape index and most egg quality traits, while GBLUP was optimal for egg weight traits.

<div style="border-left:6px solid #FECC02; background:#f7f7f7; padding:12px 16px;">

**The pattern:** which method wins depends on the trait's genetic architecture, the training population size, and the heritability. Not on which method is newer.

</div>

There is a real gift buried here. In agricultural genetics, **the baseline is a well-established, statistically principled method** — GBLUP, Bayes B, pedigree BLUP — rather than a made-up straw man. That means you can always answer the question that AI-hype papers so often dodge: *did it beat the standard tool?* Build the habit of running GBLUP first, every time. If your fancy model doesn't beat it, you've learned something worth publishing.

---

<h2 style="color:#006AA7;">Part 3 — The core that AI does not remove</h2>

| Skill | Why it survives |
|---|---|
| **Quantitative genetics** | Heritability, breeding values, selection intensity, genetic gain, inbreeding. Without this, a genomic prediction is a number with no unit. |
| **Mixed models** | Random effects, variance components, spatial adjustment of field trials, repeated measures. `ASReml`, `lme4`, `sommer`, `BLUPF90`. |
| **Experimental design** | Randomized blocks, incomplete block designs, alpha lattices, multi-environment trial networks. AI cannot rescue a badly laid-out trial. |
| **G×E and envirotyping** | Reaction norms, AMMI, GGE biplots, and increasingly ML-based interaction modelling. |
| **Data management and FAIR** | Field metadata is chronically undocumented. Which plot? Which year? Which sensor calibration? This is where most ag data goes to die. |
| **Reproducibility engineering** | Git, conda/mamba, containers, and Nextflow or Snakemake. |
| **Domain biology and agronomy** | Knowing that your "significant" QTL sits in a region that always segregates with flowering time, which confounds everything. |

Note the fourth row especially. In human genomics, sample metadata is usually structured because a hospital demanded it. In agriculture, the crucial covariates are often in a field notebook and a supervisor's memory. Becoming the person in your group who fixes this is a career move disguised as a chore.

---

<h2 style="color:#006AA7;">Part 4 — A path by degree level</h2>

<h3 style="color:#FECC02; background:#006AA7; display:inline-block; padding:4px 12px; border-radius:4px;">Bachelor's: build the floor</h3>

**Months 0–6.**

1. **R first, for most of you.** Agricultural statistics runs on R — `tidyverse`, `lme4`/`sommer`, `agricolae`, and increasingly `FIELDimageR` for plot-level image analysis. Add Python later for image and sequence work.
2. **Command line and Git.** Bash, ssh, file handling, version control from your very first script.
3. **Statistics with your own data.** Take a dataset from a course field trial or teaching herd and analyse it properly: blocking, random effects, model diagnostics.
4. **One complete omics analysis.** An RNA-seq experiment in a crop or livestock species, from raw reads to differential expression to enrichment.

**Project idea:** get a public genotype + phenotype dataset for a crop or livestock species, fit GBLUP, and cross-validate it. Report prediction accuracy honestly. This one project teaches you more about applied genetics than a semester of lectures.

<h3 style="color:#FECC02; background:#006AA7; display:inline-block; padding:4px 12px; border-radius:4px;">Master's: specialize and industrialize</h3>

1. **Pick your vertical.** Plant breeding and genomic selection; animal breeding and genetics; forest genomics; veterinary/animal health genomics; soil and rumen microbiome; food and fermentation microbiology; aquaculture genetics.
2. **Learn workflow management properly.** Rewrite your pile of scripts as a Nextflow pipeline, then read [nf-core](https://nf-co.re/) to see how professionals do it.
3. **Learn HPC.** Slurm, resource requests, GPU jobs. In Sweden, this means an account through NAISS/UPPMAX — arrange it before you need it.
4. **Touch the frontier models critically.** Score variants in your species with PlantCaduceus or AgroNT. Try a deep genomic prediction model. Then run GBLUP on the same data and compare. Write down what you find, especially when the classical method wins.
5. **Add one adjacent skill.** Computer vision for phenotyping, or spatial statistics, or metagenomic assembly and binning. Pick the one your future group needs.

**Project idea:** a small honest benchmark. Three genomic prediction methods, three traits with different heritabilities, one dataset, pre-registered metrics, proper cross-validation that respects family structure. This is master's-thesis-sized and immediately useful to a breeding programme.

<h3 style="color:#FECC02; background:#006AA7; display:inline-block; padding:4px 12px; border-radius:4px;">PhD: contribute what models can't</h3>

1. **Own a biological or agronomic question**, not a method. Methods age in 18 months; "how do we breed for methane efficiency without losing milk yield" does not.
2. **Become the person who knows the failure modes** of the tools your subfield relies on. It's the fastest route to being genuinely consulted.
3. **Cross-validate like the deployment context, not like Kaggle.** Random k-fold across a pedigreed population leaks relatedness and inflates accuracy. Split by family, by year, by location — whatever mirrors how the prediction will actually be used.
4. **Take data governance seriously.** Between the NGT regulation's traceability requirements and the EU AI Act's staged rollout through 2027, provenance and logging are becoming compliance features, not just good manners.
5. **Build one durable thing.** A package, a curated phenotype database, a documented pipeline the breeding programme actually runs.

---

<h2 style="color:#006AA7;">Part 5 — Using LLMs well while you learn</h2>

**Delegate freely:** plotting code, file format conversion, regex, "explain this Slurm error", literature triage, translating an analysis between R and Python, first-draft documentation.

**Do not delegate:** the choice of statistical model, the cross-validation scheme, the interpretation of whether a genetic parameter is plausible, or the reasoning in your methods section.

Three habits:

1. **Predict before you run.** Write down the heritability or accuracy you expect. Every surprise is a lesson; every unexamined surprise is a future retraction.
2. **Demand the baseline out loud.** *"What's the standard method in this field, and how would I compare against it?"* Then run it.
3. **Watch for the biomedical default.** LLMs have read vastly more human genomics than crop or livestock genomics. They will cheerfully suggest a human-centric pipeline, a human reference build, or an analysis that ignores pedigree structure entirely. Ask explicitly about your species, your ploidy, and your population structure.

That third one is a genuine and recurring failure mode. Polyploidy, high heterozygosity, poor reference assemblies, and family structure are normal in your world and exceptional in the training data.

---

<h2 style="color:#006AA7;">Part 6 — Where to learn (Swedish edition 🇸🇪)</h2>

<div style="border-left:6px solid #006AA7; background:#f7f7f7; padding:12px 16px;">

**[SLUBI — SLU Bioinformatics Infrastructure](https://www.slubi.se/)** is the single most useful resource for agricultural students in Sweden, and it is underused.

- Staff based at **Ultuna, Umeå and Alnarp**, supporting all four faculties: LTV (landscape, horticulture, crop production), NJ (natural resources and agricultural sciences), S (forest sciences) and VH (veterinary medicine and animal science).
- **Online drop-in sessions** — bring your question, no appointment. These moved online, so all campuses join the same session.
- **Courses** in Nextflow and reproducible bioinformatics, metagenomics, R, genetic variation and breeding strategies, quantitative genetics, and data handling and figures. Several run with SLU's graduate schools and research schools.
- The **"Three Bees"** workshop series, run with SLU's Centre for Statistics — statistical concepts and bioinformatics tools with hands-on coding.
- SLUBI also collaborates with **NADAS**, the Nordic Network of Agricultural Data Scientists, and with UPPMAX for compute and storage.

**Also at SLU:** the [Course Package in Bioinformatics](https://www.slu.se/en/study/programmes-courses/professional-development/course-package-in-bioinformatics/) (Genome Analysis BK0003 + Bioinformatics BK0004), which can build toward a 60 or 120 ECTS MSc in Bioinformatics, taught in English. And **emPLANT**, the Erasmus Mundus master's programme in plant breeding, if you want an international breeding-focused route.

**Beyond SLU:** [NBIS](https://nbis.se/) (Sweden's ELIXIR node) and the [SciLifeLab Training Portal](https://training.scilifelab.se/) run excellent courses that are open to Swedish university students generally — spatial omics, population genomics, reproducible research. NAISS for national computing.

</div>

**Free and international:**

- [nf-core](https://nf-co.re/) — production-grade pipelines, including several relevant to non-model organisms.
- [Bioconductor](https://bioconductor.org/) and [Galaxy](https://usegalaxy.eu/) for GUI-based entry points.
- [FIELDimageR](https://github.com/OpenDroneMap/FIELDimageR) and the plant phenomics tool ecosystem for orthomosaic field trial images.
- The [Carpentries](https://carpentries.org/) for shell, Git and R foundations.
- bioRxiv, *Plant Phenomics*, *Genetics Selection Evolution* and *G3* alerts in your subfield.

---

<h2 style="color:#006AA7;">A 12-week starter plan</h2>

| Weeks | Focus | Deliverable |
|---|---|---|
| 1–2 | Shell, Git, project structure | A repo with a sane layout and a README |
| 3–4 | R and data wrangling on real trial data | A cleaned, documented dataset with metadata |
| 5–6 | Mixed models and field trial analysis | A spatially-adjusted analysis with justified model choices |
| 7–8 | Genomic prediction: GBLUP end to end | Cross-validated accuracy for one trait, split sensibly |
| 9–10 | Environments, containers, Nextflow | The same analysis as a portable pipeline |
| 11 | Add one AI-era tool (a plant gLM, or an ML predictor) | Head-to-head comparison against your GBLUP baseline |
| 12 | Write-up | A report or post someone else can reproduce |

Twelve weeks won't make you a bioinformatician. It will make you a biologist who can be trusted with data — which is what breeding programmes, research groups and agri-tech companies are actually short of.

---

<div style="border-left:6px solid #FECC02; background:#f7f7f7; padding:12px 16px;">

**The thing worth remembering:** agriculture has been doing prediction under uncertainty, with structured populations and expensive phenotypes, since long before anyone said "foundation model." That tradition is not an obstacle to learning AI — it is the best possible preparation for using it honestly.

</div>

---

<h2 style="color:#006AA7;">References and further reading</h2>

- Montesinos-López et al. (2025). *Artificial intelligence meets genomic selection: comparing deep learning and GBLUP across diverse plant datasets.* **Frontiers in Genetics** 16:1568705. [doi:10.3389/fgene.2025.1568705](https://doi.org/10.3389/fgene.2025.1568705)
- *A sorghum pangenome reference improves global crop trait discovery.* **Nature** 652:1245–1253 (2026). [doi:10.1038/s41586-026-10229-9](https://www.nature.com/articles/s41586-026-10229-9)
- *From the genome to super-pangenome: a new paradigm for accelerated crop improvement.* **npj Science of Plants** 2:4 (2026). [link](https://www.nature.com/articles/s44383-025-00019-z)
- *BOTANIC-0: a series of foundation models for plant genomic data.* bioRxiv (2026). [link](https://www.biorxiv.org/content/10.64898/2026.02.23.706817v1.full)
- *PlantCAD2: a DNA foundation model for interpreting genomes across flowering plants.* bioRxiv (2026). [link](https://www.biorxiv.org/content/10.1101/2025.08.27.672609v4)
- PlantCaduceus project page — [plantcaduceus.github.io](https://plantcaduceus.github.io/)
- *Comparative Accuracy of Machine Learning and GBLUP for Predicting Genomic Estimated Breeding Values in Chickens.* **Genes** 17(3):315 (2026). [doi:10.3390/genes17030315](https://doi.org/10.3390/genes17030315)
- *Soil microbiome prediction using traditional machine learning and deep learning models.* **Scientific Reports** 16:11069 (2026). [doi:10.1038/s41598-026-39537-w](https://www.nature.com/articles/s41598-026-39537-w)
- *Next-generation soil monitoring: linking metagenomics, biosensors, and ecological modeling for sustainable agriculture.* **Frontiers in Microbiology** (2026). [link](https://www.frontiersin.org/journals/microbiology/articles/10.3389/fmicb.2026.1861333/full)
- European Commission — [New Genomic Techniques](https://food.ec.europa.eu/plants/new-genomic-techniques_en) and Council of the EU — [NGT policy page](https://www.consilium.europa.eu/en/policies/new-genomic-techniques-for-plant-breeding/)
- SLUBI courses — [slubi.se/courses.html](https://www.slubi.se/courses.html)

<div align="center" style="background:#006AA7; color:#FECC02; padding:14px; border-radius:8px;">

*Written August 2026. The tool names here have a short shelf life; the habits — baseline first, structure respected, metadata written down — do not.*

</div>
