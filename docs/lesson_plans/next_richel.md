# Lesson plan

- Author: Richel

Here I keep my notes for preparing the next course iteration.

Open questions, for literature study:

- What are the most important ways of biomarker discovery?
  `[Zhang et al., 2025]` is a modern paper on this. 
- The MOFA dataset is a public data set used in many
  biomarker discovery techniques. Is it?
  I found it [at the MOFA2 homepage](https://biofam.github.io/MOFA2/index.html).
  Datasets can be found at [the MOFAdata GitHub repository](https://github.com/bioFAM/MOFAdata).
  They even have [tutorials](https://biofam.github.io/MOFA2/tutorials.html)
  that can be used directly


## 2026-09-22

I feel I need to take a good at the data,
datasets can be found at [the MOFAdata GitHub repository](https://github.com/bioFAM/MOFAdata).
They even have [tutorials](https://biofam.github.io/MOFA2/tutorials.html)
that can be used directly


## 2026-09-25

The course is called 'Biomarker Discovery:
from theory to real world examples'.
However, there may be two places where biomarker discovery starts:

- **From a research question**, discovering the most likely/useful biomarkers.
  In such a case, the dataset needs to be found.
    - [Open Biomarker datasets](https://data.biomarkerkb.org/)
    - Multi-cohort data
    - Evaluation a biomarker being valid when using two datasets

- **From a dataset**, where one or more analyses are done
  to conclude if a biomarker has an effect yes/no

I ask Prasoon, because I do need the answer before I continue :+1:


I can imagine that learning outcomes can be:

- Learners can distinguish the four different types of biomarkers:
    - diagnostic biomarkers: helps to diagnose if there is a disease yes/no
    - prognostic biomarkers: predict an outcome of a disease
    - predictive biomarkers: predicts the effect of a drug
    - pharmacodynamic biomarkers: measures the interaction between a drug
    and its receptor
- Learners can conclude the type of biomarker

## 2026-09-29

I spoke to Prasoon at the NAISS retreat:

- He wants to start from a research question. I like that
- He wants teaching to be interactive. I like that
- He wants to assume our learners already know the types of biomakers

## 2026-10-28

What are Evidence-based best practices for biomarker discovery?

I read, from a Consensus answer:

> Evidence-based biomarker discovery relies on structured multi-phase
> frameworks spanning early candidate selection to analytical validation
> and independent clinical qualification
> (Nakayasu et al., 2021; Rifai et al., 2006; Califf, 2018). 
> Translating initial omics or mass-spectrometry findings into
> reliable clinical assays requires strict adherence to statistical
> rigor, standardized sample handling, and pre-specified contexts of
> use (Nakayasu et al., 2021; Ahmad et al., 2023; Fernandez-Metzler et al., 2022).

I check these references first.

Reference                |Comment on title
-------------------------|-----------------------------------------------------------------
`[Nakayasu et al., 2021]`|Is mass-spectrometry-based, should we use this?
`[Rifai et al., 2006]`   |Seems good, is oldest
`[Califf, 2018]`         |Seems good

Open questions:

- Should this course be mass-spectrometry based yes/no
- What are the differences in approaches

I start with the most recent paper.

???- question "Answer from Consensus"

    # Evidence-based best practices require **prospective study design**, robust quality control, and **multicohort validation**.

    Evidence-based biomarker discovery relies on structured multi-phase frameworks spanning early candidate selection to analytical validation and independent clinical qualification (Nakayasu et al., 2021; Rifai et al., 2006; Califf, 2018). Translating initial omics or mass-spectrometry findings into reliable clinical assays requires strict adherence to statistical rigor, standardized sample handling, and pre-specified contexts of use (Nakayasu et al., 2021; Ahmad et al., 2023; Fernandez-Metzler et al., 2022).

    ## Evidence Supporting Biomarker Discovery Standards

    | Evidence Strength | Claim |
    | :--- | :--- |
    | Evidence strength: Strong (9/10) | Establishing a **prospective experimental design** with blinding, randomization, and adequate statistical power prevents high false-discovery rates and non-reproducible candidates (Nakayasu et al., 2021; Ekström et al., 2025). |
    | Evidence strength: Strong (9/10) | Confirmation across **independent multicohort test sets** is mandatory to prevent statistical overfitting before clinical qualification (Glaab et al., 2021; Mischak et al., 2010; Ekström et al., 2025; López-López et al., 2018). |
    | Evidence strength: Strong (8/10) | Pre-defining a **context of use (COU)** guides fit-for-purpose analytical assay validation including sensitivity, precision, and stability thresholds (Rajapaksha & Farmer, 2026; Fernandez-Metzler et al., 2022; Bakker et al., 2022). |

    **Figure 1:** Evidence strength for methodological best practices in biomarker discovery

    ## Methodological Workflow for Biomarker Translation

    The translational pipeline from discovery to clinical adoption follows a sequential series of quality gates designed to mitigate attrition (Ou et al., 2021; Rifai et al., 2006; Califf, 2018).

    **Translational Biomarker Development Pipeline**

    ```mermaid
    flowchart LR; A[Define Context of Use] --> B[Cohort Design & Powering]; B --> C[Discovery & QC Screening]; C --> D[Verification Assay Optimization]; D --> E[Independent Multicohort Validation]; E --> F[Regulatory Qualification]
    ```
    **Figure 2:** Sequential phases of biomarker development from initial discovery to qualification

    A critical primary pitfall in early discovery is underpowered sample sizes and reliance on unadjusted p-values without independent testing (Nakayasu et al., 2021; Ekström et al., 2025). A systematic analysis of 7,631 biomarker citations highlighted that common failures stem from inappropriate control cohorts and omission of blinding (Nakayasu et al., 2021). Investigators should formulate explicit sample procurement plans, allocate matched concurrent controls, and balance cohorts prior to data acquisition (Ekström et al., 2025; Ahmad et al., 2023). 

    In high-throughput platforms such as mass spectrometry and metabolomics, standardized quality controls (QCs) and standardized specimen handling are essential to control technical variability (Nakayasu et al., 2021; Ahmad et al., 2023; López-López et al., 2018). Studies employing extreme phenotype selection can enrich candidate signals in early exploratory phases, allowing biological differentiation before expanding cohort sizes (Pérez-Gracia et al., 2017).

    ## Key Statistical and Analytical Best Practices

    * **Power optimization and pre-specification**: Calculate sample size requirements prior to study initiation using statistical simulations, such as Receiver Operating Characteristic (ROC) framework models, to avoid underpowered candidate discovery (Ekström et al., 2025).
    * **Fit-for-purpose analytical validation**: Define assay acceptance criteria—including sensitivity, precision, selectivity, dilutional parallelism, and matrix stability—calibrated to the pre-defined clinical context of use (Rajapaksha & Farmer, 2026; Fernandez-Metzler et al., 2022).
    * **Cross-disciplinary team partnerships**: Form collaborative alliances among clinicians, bioinformaticians, epidemiologists, and statisticians to align biological plausibility with regulatory compliance and trial design (Ou et al., 2021; Glaab et al., 2021; Califf, 2018).
    * **Rigorous multi-cohort external validation**: Test candidate performance on external, multi-center cohorts using fixed thresholds to confirm clinical utility and sensitivity benchmarks (Glaab et al., 2021; Mischak et al., 2010; Palmqvist et al., 2025; Savva et al., 2023).

    Following established regulatory guidelines, such as those from the FDA, EMA, or CLSI, ensures candidate biomarkers satisfy evidentiary standards required for clinical and diagnostic translation (Maslova et al., 2026; Kraus, 2018; Bakker et al., 2022).
     
    _These search results were found and analyzed using Consensus, an AI-powered search engine for research. Try it at https://consensus.app. © 2026 Consensus NLP, Inc. Personal, non-commercial use only; redistribution requires copyright holders’ consent._
     
    ## References
     
    Ahmad, A., Imran, M., & Ahsan, H. (2023). Biomarkers as Biomedical Bioindicators: Approaches and Techniques for the Detection, Analysis, and Validation of Novel Biomarkers of Diseases. *Pharmaceutics, 15*. https://doi.org/10.3390/pharmaceutics15061630
     
    Bakker, E., Hendrikse, N. M., Ehmann, F., Van Der Meer, D. S., Vetter, T., Starokozhko, V., & Mol, P. G. M. (2022). Biomarker Qualification at the European Medicines Agency: A Review of Biomarker Qualification Procedures From 2008 to 2020. *Clinical Pharmacology and Therapeutics, 112*, 69 - 80. https://doi.org/10.1002/cpt.2554
     
    Califf, R. (2018). Biomarker definitions and their applications. *Experimental Biology and Medicine, 243*, 213 - 221. https://doi.org/10.1177/1535370217750088
     
    Ekström, J., Stoimenov, I., Ögren, J., & Sjöblom, T. (2025). Biomarker discovery study design consistent with the Receiver-Operator Characteristic. *Computer methods and programs in biomedicine, 276*, 109215. https://doi.org/10.1101/2025.04.23.25326188
     
    Fernandez-Metzler, C., Ackermann, B., Garofolo, F., Arnold, M. E., Desilva, B. S., Gu, H., Laterza, O., Mao, Y., Rose, M., Vazvaei-Smith, F., & Steenwyk, R. (2022). Biomarker Assay Validation by Mass Spectrometry. *The AAPS Journal, 24*. https://doi.org/10.1208/s12248-022-00707-z
     
    Glaab, E., Rauschenberger, A., Banzi, R., Gerardi, C., García, P., & Demotes, J. (2021). Biomarker discovery studies for patient stratification using machine learning analysis of omics data: a scoping review. *BMJ Open, 11*. https://doi.org/10.1136/bmjopen-2021-053674
     
    Kraus, V. (2018). Biomarkers as drug development tools: discovery, validation, qualification and use. *Nature Reviews Rheumatology, 14*, 354-362. https://doi.org/10.1038/s41584-018-0005-9
     
    López-López, Á., López-Gonzálvez, Á., Barker-Tejeda, T. C., & Barbas, C. (2018). A review of validated biomarkers obtained through metabolomics. *Expert Review of Molecular Diagnostics, 18*, 557 - 575. https://doi.org/10.1080/14737159.2018.1481391
     
    Maslova, K., Chechlińska, M., Michalek, I., Taraszkiewicz, L., Kober, P., Trulson, I., Worf, K., Gabriel, S., Knoblauch, L., Campbell, F., Cree, I. A., Holdenrieder, S., & Kowalewska, M. (2026). Tumour markers and evidence-based pathology.. *Tumour biology : the journal of the International Society for Oncodevelopmental Biology and Medicine, 48*, 14230380251410478. https://doi.org/10.1177/14230380251410478
     
    Mischak, H., Allmaier, G., Apweiler, R., Attwood, T., Baumann, M., Benigni, A., Bennett, S. E., Bischoff, R., Bongcam-Rudloff, E., Capasso, G., Coon, J., D'Haese, P., Dominiczak, A., Dakna, M., Dihazi, H., Ehrich, J., Fernández-Llama, P., Fliser, D., Frøkiær, J., . . . Vlahou, A. (2010). Recommendations for Biomarker Identification and Qualification in Clinical Proteomics. *Science Translational Medicine, 2*, 46ps42 - 46ps42. https://doi.org/10.1126/scitranslmed.3001249
     
    Nakayasu, E., Gritsenko, M., Piehowski, P., Gao, Y.-Q., Orton, D., Schepmoes, A., Fillmore, T., Frohnert, B., Rewers, M., Krischer, J., Ansong, C., Suchy-Dicey, A. M., Evans-Molina, C., Qian, W., Webb-Robertson, B., & Metz, T. (2021). Tutorial: best practices and considerations for mass-spectrometry-based protein biomarker discovery and validation. *Nature protocols, 16*, 3737 - 3760. https://doi.org/10.1038/s41596-021-00566-6
     
    Ou, F., Michiels, S., Shyr, Y., Adjei, A., & Oberg, A. (2021). Biomarker Discovery and Validation: Statistical Considerations. *Journal of thoracic oncology : official publication of the International Association for the Study of Lung Cancer, 16*, 537 - 545. https://doi.org/10.1016/j.jtho.2021.01.1616
     
    Palmqvist, S., Whitson, H. E., Allen, L. A., Suárez-Calvet, M., Galasko, D., Karikari, T., Okrahvi, H. R., Paczynski, M., Schindler, S., Teunissen, C., Zetterberg, H., Carrillo, M. C., Edelmayer, R., Mahinrad, S., McAteer, M. B., Kahale, L. A., Pahlke, S., & Tampi, M. (2025). Alzheimer's Association Clinical Practice Guideline on the use of blood‐based biomarkers in the diagnostic workup of suspected Alzheimer's disease within specialized care settings. *Alzheimer's & Dementia, 21*. https://doi.org/10.1002/alz.70535
     
    Pérez-Gracia, J., Sanmamed, M., Bosch, A., Patiño-García, A., Schalper, K., Segura, V., Bellmunt, J., Tabernero, J., Sweeney, C., Choueiri, T., Martín, M., Fusco, J., Rodriguez Ruiz, M., Calvo, A., Prior, C., Paz-Ares, L., Pio, R., González-Billalabeitia, E., González Hernández, Á., . . . Melero, I. (2017). Strategies to design clinical studies to identify predictive biomarkers in cancer research.. *Cancer treatment reviews, 53*, 79-97. https://doi.org/10.1016/j.ctrv.2016.12.005
     
    Rajapaksha, R., & Farmer, J. T. (2026). Regulatory and scientific considerations in PK and biomarker assay validation: lessons from bioanalytical practice.. *Bioanalysis, 18 3*, 293-311. https://doi.org/10.1080/17576180.2026.2658614
     
    Rifai, N., Gillette, M., & Carr, S. (2006). Protein biomarker discovery and validation: the long and uncertain path to clinical utility. *Nature Biotechnology, 24*, 971-983. https://doi.org/10.1038/nbt1235
     
    Savva, K., Kawka, M., Vadhwana, B., Penumaka, R., Patton, I., Khan, K., Perrott, C., Das, S., Giot, M., Mavroveli, S., Hanna, G. B., Ni, M., & Peters, C. J. (2023). The Biomarker Toolkit — an evidence-based guideline to predict cancer biomarker success and guide development. *BMC Medicine, 21*. https://doi.org/10.1186/s12916-023-03075-3
 
Which dataset to use?

???- question "Answers"

    ???- question "What did Claude suggest?"

        Good teaching datasets for biomarker discovery, grouped by use:

        Omics / multi-omics (large, real-world)

        TCGA (via GDC portal or TCGAbiolinks/curatedTCGAData in R): tumor vs. normal expression, mutations, methylation and survival across 33 cancers. The standard choice for prognostic and diagnostic biomarker exercises.
        GEO (NCBI Gene Expression Omnibus): thousands of case/control microarray and RNA-seq studies. Useful for teaching discovery in one cohort and validation in another, e.g. several independent breast cancer or sepsis datasets.
        METABRIC: about 2,000 breast cancer samples with expression and long follow-up. Good for survival and subtype biomarkers.
        CPTAC: proteomics matched to TCGA tumors. Useful for comparing RNA and protein biomarkers.

        Clinical / cohort

        ADNI (Alzheimer’s): CSF, imaging, genetics and longitudinal outcomes. A classic example of biomarker validation. Requires an application, which is usually quick for academic use.
        UK Biobank: genomics, proteomics (Olink) and metabolomics at population scale. It is powerful but requires a paid or approved application, so it may be impractical for a course.
        MIMIC-IV: ICU clinical and lab data, good for prognostic markers. Requires free PhysioNet credentialing.
        NHANES: free blood and urine biomarkers with health outcomes. No access barriers.

        Proteomics / metabolomics

        PRIDE / ProteomeXchange: mass-spec proteomics.
        MetaboLights and Metabolomics Workbench: metabolomics case/control studies.

        Small, classroom-friendly (quick to load)

        Golub leukemia (ALL vs. AML), Alon colon cancer and van ‘t Veer breast cancer (MammaPrint). These are classics for showing feature selection, overfitting and the “small n, large p” problem. They are available in R/Bioconductor packages.
        Wisconsin Breast Cancer (UCI / scikit-learn): simple, tabular, good for a first week.

        Suggested course arc: start with Golub or Wisconsin, then do discovery in TCGA with validation in GEO or METABRIC, and finish with a clinical-translation case using ADNI or NHANES.

    ???- question "What did Consensus suggest?"

        # Public **multi-omics cohorts** and repositories serve best for biomarker discovery coursework.

        Selecting datasets for a course on biomarker discovery requires resources with deep clinical annotations, high-dimensional molecular profiling, and sufficient sample sizes to teach quality control, feature selection, and validation (Lin et al., 2019; Ng et al., 2023).

        ## Benchmark Cohorts and Public Repositories

        | Dataset / Repository | Primary Modality & Scope | Pedagogical Value for Courses | Citation |
        | :--- | :--- | :--- | :--- |
        | **TCGA & ICGC** | Multimodal cancer profiling across 33 tumor types (>11,000 patients) | Teaches cross-layer cancer genomics, tumor vs. normal differential expression, and patient survival modeling | (Ng et al., 2023; Majoros et al., 2025) |
        | **ROSMAP Cohort** | Transcriptomic, microRNA, methylation, and clinical data (378 samples) | Benchmark for neurodegenerative disease modeling and multi-omics integration | (Njume et al., 2026) |
        | **MayoRNASeq Cohort** | Transcriptomic, proteomic, and metabolomic profiling (437 samples) | Demonstrates non-cancer phenotypes (PSP) and multi-omics feature stability | (Njume et al., 2026) |
        | **PRIDE & Expression Atlas** | Mass spectrometry proteomics across diverse tissue and biofluid cohorts | Teaches proteomic data reprocessing, missing-value imputation, and hypothesis generation | (Robles et al., 2024) |
        | **Curated Signatures (MSigDB, GeneSigDB)** | Curated gene sets and biological interaction networks (STRING, BioGRID) | Allows validation of candidate gene sets against known pathway biology and interactomes | (Lin et al., 2019; Majoros et al., 2025) |

        **Figure 1:** Widely utilized open-access datasets and repositories for biomarker discovery benchmarking.

        ## Key Analytical Frameworks for Instruction

        Biomarker discovery courses frequently utilize these cohorts because high-throughput omics present distinct dimensionality challenges, where features vastly outnumber samples (Sid et al., 2025; Ng et al., 2023; Zhang et al., 2021). For cancer applications, The Cancer Genome Atlas (TCGA) cohorts, such as TCGA-BRCA, permit students to explore how classical classification models perform across dual- and triple-omics layers compared to single omics (Njume et al., 2026). Students can implement filter, wrapper, and embedded feature selection techniques to identify compact signatures that generalize to external test cohorts (Zhang et al., 2021).

        Neurodegenerative cohorts such as ROSMAP and MayoRNASeq provide real-world postmortem and biofluid data for teaching the identification of subtle effects (Moreira & Jan, 2023; Njume et al., 2026). Working with untargeted metabolomics or mass-spectrometry datasets exposes students to critical preprocessing steps, such as handling correlated clusters, data normalization, and false discovery rate penalties (Lin et al., 2019; Anwardeen et al., 2023; Grissa et al., 2016; Moreira & Jan, 2023). Interactive platforms such as MetaboAnalyst, OmicLearn, and BEST provide accessible environments to demonstrate these pipelines without requiring advanced software engineering skills (Anwardeen et al., 2023; Torun et al., 2021; Liu et al., 2022).

        ## Methodological Lessons for Course Design

        - **Dataset shift and generalization**: Training on single cohorts often leads to overfitting; students should evaluate biomarkers on external validation sets to observe how distribution shifts degrade predictive performance (Lin et al., 2019; Ng et al., 2023; Dockès et al., 2021).
        - **Model complexity versus interpretability**: Benchmarks on cohorts like TCGA and ROSMAP show simpler classifiers often match deep learning while preserving biological interpretability (Ng et al., 2023; Nakayasu et al., 2021; Njume et al., 2026).
        - **Feature sparsity and stability**: Utilizing ensemble methods or sparsity frameworks distills thousands of candidate variables down to minimal panels while mitigating false discoveries (Hédou et al., 2024; Cattelani & Fortino, 2022; Njume et al., 2026).
        - **Rigorous validation metrics**: Performance must be evaluated using receiver-operator characteristic metrics and multi-cohort splits rather than basic training accuracy alone (Ng et al., 2023; Glaab et al., 2021; Ekström et al., 2025).
         
        _These search results were found and analyzed using Consensus, an AI-powered search engine for research. Try it at https://consensus.app. © 2026 Consensus NLP, Inc. Personal, non-commercial use only; redistribution requires copyright holders’ consent._
         
        ## References
         
        Anwardeen, N., Diboun, I., Mokrab, Y., Thani, A. A., & Elrayess, M. A. (2023). Statistical methods and resources for biomarker discovery using metabolomics. *BMC Bioinformatics, 24*. https://doi.org/10.1186/s12859-023-05383-0
         
        Cattelani, L., & Fortino, V. (2022). Improved NSGA-II algorithms for multi-objective biomarker discovery. *Bioinformatics, 38 Supplement_2*, ii20-ii26. https://doi.org/10.1093/bioinformatics/btac463
         
        Dockès, J., Varoquaux, G., & Poline, J. B. (2021). Preventing dataset shift from breaking machine-learning biomarkers. *GigaScience, 10*. https://doi.org/10.1093/gigascience/giab055
         
        Ekström, J., Stoimenov, I., Ögren, J., & Sjöblom, T. (2025). Biomarker discovery study design consistent with the Receiver-Operator Characteristic. *Computer methods and programs in biomedicine, 276*, 109215. https://doi.org/10.1101/2025.04.23.25326188
         
        Glaab, E., Rauschenberger, A., Banzi, R., Gerardi, C., García, P., & Demotes, J. (2021). Biomarker discovery studies for patient stratification using machine learning analysis of omics data: a scoping review. *BMJ Open, 11*. https://doi.org/10.1136/bmjopen-2021-053674
         
        Grissa, D., Pétéra, M., Brandolini, M., Napoli, A., Comte, B., & Pujos-Guillot, E. (2016). Feature Selection Methods for Early Predictive Biomarker Discovery Using Untargeted Metabolomic Data. *Frontiers in Molecular Biosciences, 3*. https://doi.org/10.3389/fmolb.2016.00030
         
        Hédou, J., Marić, I., Bellan, G., Einhaus, J., Gaudillière, D., Ladant, F.-X., Verdonk, F., Stelzer, I., Feyaerts, D., Tsai, A., Ganio, E., Sabayev, M., Gillard, J., Amar, J., Cambriel, A., Oskotsky, T., Roldan, A., Golob, J., Sirota, M., . . . Gaudilliere, B. (2024). Discovery of sparse, reliable omic biomarkers with Stabl. *Nature biotechnology, 42*, 1581 - 1593. https://doi.org/10.1038/s41587-023-02033-x
         
        Lin, Y.-X., Qian, F., Shen, L., Chen, F.-F., Chen, J., & Shen, B.-R. (2019). Computer-aided biomarker discovery for precision medicine: data resources, models and applications. *Briefings in bioinformatics, 20 3*, 952-975. https://doi.org/10.1093/bib/bbx158
         
        Liu, Z.-Q., Liu, L., Weng, S.-Y., Xu, H.-X., Xing, Z., Ren, Y.-Q., Ge, X., Wang, L., Guo, C.-G., Li, L.-F., Cheng, Q., Luo, P., Zhang, J., & Han, X. (2022). BEST: a web application for comprehensive biomarker exploration on large-scale data in solid tumors. *Journal of Big Data, 10*, 1-14. https://doi.org/10.1186/s40537-023-00844-y
         
        Majoros, S., Shiell, M., Wang, J., Richardsson, J., Trinh, Q. M., Marcellus, R., Uehling, D., Al-Awar, R., Pai, S., Courtot, M., & Stein, L. (2025). Abstract A006: Data Curation and Knowledge Integration Pipeline for Biomarker Discovery. *Clinical Cancer Research*. https://doi.org/10.1158/1557-3265.aimachine-a006
         
        Moreira, D. G., & Jan, A. (2023). A beginner’s guide into curated analyses of open access datasets for biomarker discovery in neurodegeneration. *Scientific Data, 10*. https://doi.org/10.1038/s41597-023-02338-1
         
        Nakayasu, E., Gritsenko, M., Piehowski, P., Gao, Y.-Q., Orton, D., Schepmoes, A., Fillmore, T., Frohnert, B., Rewers, M., Krischer, J., Ansong, C., Suchy-Dicey, A. M., Evans-Molina, C., Qian, W., Webb-Robertson, B., & Metz, T. (2021). Tutorial: best practices and considerations for mass-spectrometry-based protein biomarker discovery and validation. *Nature protocols, 16*, 3737 - 3760. https://doi.org/10.1038/s41596-021-00566-6
         
        Ng, S., Masarone, S., Watson, D., & Barnes, M. R. (2023). The benefits and pitfalls of machine learning for biomarker discovery. *Cell and Tissue Research, 394*, 17 - 31. https://doi.org/10.1007/s00441-023-03816-z
         
        Njume, C. M., Petracci, I., Bellini, S., Goljanek‐Whysall, K., Quinlan, L. R., Fiszer, A., Borroni, B., Ghidoni, R., Kumbasar, A., & Çakmak, A. (2026). When complexity does not pay: benchmarking deep learning and ensemble methods for biomarker discovery. *Briefings in Bioinformatics, 27*. https://doi.org/10.1093/bib/bbag211
         
        Robles, J., Prakash, A., Vizcaíno, J., & Casal, J. I. (2024). Integrated meta-analysis of colorectal cancer public proteomic datasets for biomarker discovery and validation. *PLOS Computational Biology, 20*. https://doi.org/10.1371/journal.pcbi.1011828
         
        Sid, K., Zertal, S., Batouche, M., & Zerabi, S. (2025). Efficient Hybrid-Robust Approach for Cancer Biomarker Discovery Using Omics Data. *IEEE Access, 13*, 51130-51149. https://doi.org/10.1109/access.2025.3553078
         
        Torun, F. M., Winter, S. V., Doll, S., Riese, F. M., Vorobyev, A., Mueller-Reif, J. B., Geyer, P., & Strauss, M. T. (2021). Transparent Exploration of Machine Learning for Biomarker Discovery from Proteomics and Omics Data. *Journal of Proteome Research, 22*, 359 - 367. https://doi.org/10.1021/acs.jproteome.2c00473
         
        Zhang, X.-K., Jonassen, I., & Goksøyr, A. (2021). Machine Learning Approaches for Biomarker Discovery Using Gene Expression Data. *Bioinformatics*. https://doi.org/10.36255/exonpublications.bioinformatics.2021.ch4
         

    ???- question "What did Gemini suggest?"

        Here is a summary of the best available open-access datasets for a course on biomarker discovery:
        When structuring coursework, the most effective datasets combine well-defined clinical endpoints (such as disease diagnosis, subtype classification, or survival time) with accessible, multi-omic biological data.
        Key themes across available datasets:
        Classic Benchmark Datasets for Assignments: Compact transcriptomic datasets (such as the Golub Leukemia dataset or Singh Prostate Cancer Microarray dataset) are ideal for introductory exercises in feature selection, classification, and differential expression analysis.
        Multi-Omics & Proteomics Repositories: Resources like cBioPortal / TCGA (for transcriptomics, copy-number variations, and mutations) and CPTAC (for mass spectrometry proteomics paired with genomics) allow students to work with real-world clinical cancer cohorts.
        Multi-Modal & Clinical Datasets: Collections like PhysioNet (MIMIC-IV) for clinical/physiological parameters and ADNI (Alzheimer's Disease Neuroimaging Initiative) for CSF and neuroimaging biomarkers provide practice with longitudinal and clinical data types.
        Tool Integration & Programmatic Access: Pre-curated benchmark collections available through R/Python libraries (such as curatedTCGAData or Therapeutic Data Commons) minimize data-wrangling friction in coding labs.
        📥 The full research report is included as the first source in the import card below — import it to chat with the findings directly.

## 2026-10-29

I've read the three main papers `[Califf, 2018]`
and `[Nakayasu et al., 2021]` and `[Rifai et al., 2006]`.
These are, however, mostly describing lab work.
Let's search for something computational.

???- question "What did you prommpt"

    My prompt to Consensus:

    > Thanks! Now focus only on biomarker discovery that can be done computationally.

    # Best practices for **computational biomarker discovery** prioritize sparse selection and external validation.

    Computational biomarker discovery leverages bioinformatics, machine learning (ML), and artificial intelligence (AI) to prioritize predictive molecular signatures from high-dimensional datasets while mitigating severe overfitting (Njume et al., 2026; Dhillon et al., 2022; Ng et al., 2023). Effectively deriving actionable *in silico* signatures requires strict adherence to dimensionality reduction, stability assessments, multi-omics integration, and independent algorithmic benchmarking (Njume et al., 2026; Hédou et al., 2024; Glaab et al., 2021; Zhang et al., 2021).

    ## Methodological Frameworks and Algorithmic Approaches

    Computational pipelines are designed to handle the "curse of dimensionality," where thousands of molecular variables outnumber small sample sizes (Zenbout et al., 2023). Automated tools like BioDiscML standardize the end-to-end analytical workflow by automating preprocessing, multi-algorithm feature selection, and model evaluation across unbalanced clinical datasets (Leclercq et al., 2019). Furthermore, comprehensive benchmarks show that while deep learning can capture complex interactions, simpler linear models and ensemble methods often match or exceed deep networks in classification accuracy and interpretability at lower computational costs (Njume et al., 2026; Ghaleb et al., 2025).

    | Framework / Tool | Analytical Strategy | Validation and Performance Highlights |
    | :--- | :--- | :--- |
    | **Stabl** (Hédou et al., 2024) | Noise injection and data-driven signal-to-noise thresholding | Distills 1,400–35,000 features down to 4–34 reliable biomarkers across five clinical studies (Hédou et al., 2024). |
    | **sDCFE** (Ghaleb et al., 2025) | Fisher-like variance analysis with MAD regularization and clustering | Intersects with XGBoost to yield 82 candidate genes; achieves 94% accuracy on PCAWG (Ghaleb et al., 2025). |
    | **DIABLO** (Singh et al., 2019) | Multi-omics latent component modeling via mixOmics | Identifies biologically relevant multi-omic drivers discriminating complex phenotype groups (Singh et al., 2019). |
    | **PBMF** (Arango-Argoty et al., 2025) | Neural network architecture leveraging contrastive learning | Retrospectively uncovered predictive biomarkers in trial data yielding a 15% survival benefit (Arango-Argoty et al., 2025). |
    | **ProMS / ProMS_mo** (Shi et al., 2021) | Constrained weighted $k$-medoids clustering | Selects functional representative protein markers with alternative replacement candidates (Shi et al., 2021). |

    **Figure 1:** Comparison of specialized computational frameworks for biomarker discovery and feature selection

    ## Dimensionality Reduction and Multi-Omics Integration

    Reducing model complexity through feature selection improves classification accuracy over full-feature baseline models (MohdFaizal et al., 2023). For instance, in acute myocardial infarction classification, reducing 62 features to a parsimonious five-marker panel improved the mean area under the precision-recall curve to 0.8462 (MohdFaizal et al., 2023). Integrating multiple omics layers—such as transcriptomics, methylation, and proteomics—consistently boosts biomarker recovery over single-layer analysis (Njume et al., 2026; Jiang et al., 2025). Knowledge-guided deep architectures like DeePathNet and DeepKEGG illustrate that incorporating biological pathways and molecular networks achieves superior discovery accuracy (Zenbout et al., 2023; Li et al., 2026).

    Unsupervised exploration techniques provide an essential entry point when underlying disease mechanisms or subtypes are poorly defined (Ng et al., 2023). Techniques such as consensus clustering aggregate repeated subsampling runs to establish stable patient partitions that mitigate random noise fluctuations (Ng et al., 2023). To ensure candidate markers reflect true biological significance rather than statistical artifacts, top-performing pipelines intersect statistical feature importance with biological knowledge databases, functional enrichment, and survival analyses (Ghaleb et al., 2025; Glaab et al., 2021; Zhang et al., 2021).

    ## Evidence-Based Computational Best Practices

    * Apply **multivariate feature selection** and statistical screening to eliminate uninformative noise and minimize classification error in high-content profiling (Papoutsoglou et al., 2023; Dai et al., 2025).
    * Incorporate **prior biological knowledge**, such as protein-protein interaction networks and signaling pathways, to constrain search spaces and boost mechanistic plausibility (Glaab et al., 2021; Zenbout et al., 2023; Li et al., 2026; Zhang et al., 2021).
    * Prioritize **model interpretability** using post hoc explanation tools or linear estimators rather than black-box architectures to verify candidates before clinical translation (Njume et al., 2026; Ng et al., 2023; Papoutsoglou et al., 2023).
    * Enforce **external validation** across independent cohorts and standardized reference databases to confirm predictive stability across diverse patient populations (Njume et al., 2026; Jiang et al., 2025; Díaz-Uriarte et al., 2022).

    Computational biomarker discovery establishes reproducible molecular candidates when investigators pair sparse feature selection with biological priors, rigorous model evaluation, and multi-cohort validation (Njume et al., 2026; Hédou et al., 2024; Glaab et al., 2021; Zhang et al., 2021). Adopting these *in silico* practices ensures that candidate signatures demonstrate true generalizability before entering targeted assay development (Wang et al., 2026; Ng et al., 2023; Shi et al., 2021; Díaz-Uriarte et al., 2022).
     
    _These search results were found and analyzed using Consensus, an AI-powered search engine for research. Try it at https://consensus.app. © 2026 Consensus NLP, Inc. Personal, non-commercial use only; redistribution requires copyright holders’ consent._
     
    ## References
     
    Arango-Argoty, G. A., Bikiel, D. E., Sun, G. J., Kipkogei, E., Smith, K. M., Pro, S. C., Choe, E. Y., & Jacob, E. (2025). AI-driven predictive biomarker discovery with contrastive learning to improve clinical trial outcomes.. *Cancer cell*. https://doi.org/10.1016/j.ccell.2025.03.029
     
    Dai, Y.-F., Wu, D., Carroll, I., Zou, F., & Zou, B.-M. (2025). High-dimensional biomarker identification for interpretable disease prediction via machine learning models. *Bioinformatics, 41*. https://doi.org/10.1093/bioinformatics/btaf266
     
    Dhillon, A., Singh, A., & Bhalla, V. (2022). A Systematic Review on Biomarker Identification for Cancer Diagnosis and Prognosis in Multi-omics: From Computational Needs to Machine Learning and Deep Learning. *Archives of Computational Methods in Engineering, 30*, 917-949. https://doi.org/10.1007/s11831-022-09821-9
     
    Díaz-Uriarte, R., De Lope, E. G., Giugno, R., Fröhlich, H., Nazarov, P., Nepomuceno-Chamorro, I. A., Rauschenberger, A., & Glaab, E. (2022). Ten quick tips for biomarker discovery and validation analyses using machine learning. *PLoS Computational Biology, 18*. https://doi.org/10.1371/journal.pcbi.1010357
     
    Ghaleb, M. S., Al-Berry, M. N., Ebied, H. M., & Tolba, M. F. (2025). A novel statistical feature selection framework for biomarker discovery and cancer classification via multiomics integration. *BMC Medical Research Methodology, 26*. https://doi.org/10.1186/s12874-025-02713-z
     
    Glaab, E., Rauschenberger, A., Banzi, R., Gerardi, C., García, P., & Demotes, J. (2021). Biomarker discovery studies for patient stratification using machine learning analysis of omics data: a scoping review. *BMJ Open, 11*. https://doi.org/10.1136/bmjopen-2021-053674
     
    Hédou, J., Marić, I., Bellan, G., Einhaus, J., Gaudillière, D., Ladant, F.-X., Verdonk, F., Stelzer, I., Feyaerts, D., Tsai, A., Ganio, E., Sabayev, M., Gillard, J., Amar, J., Cambriel, A., Oskotsky, T., Roldan, A., Golob, J., Sirota, M., . . . Gaudilliere, B. (2024). Discovery of sparse, reliable omic biomarkers with Stabl. *Nature biotechnology, 42*, 1581 - 1593. https://doi.org/10.1038/s41587-023-02033-x
     
    Jiang, Z., Zhang, H.-X., Gao, Y., & Sun, Y. (2025). Multi-omics strategies for biomarker discovery and application in personalized oncology. *Molecular Biomedicine, 6*. https://doi.org/10.1186/s43556-025-00340-0
     
    Leclercq, M., Vittrant, B., Martin-Magniette, M., Scott-Boyer, M., Périn, O., Bergeron, A., Fradet, Y., & Droit, A. (2019). Large-Scale Automatic Feature Selection for Biomarker Discovery in High-Dimensional OMICs Data. *Frontiers in Genetics, 10*. https://doi.org/10.3389/fgene.2019.00452
     
    Li, A. Z., Du, Y., Liu, Y., Chen, L., & Liu, R.-S. (2026). Benchmarking computational methods for multi-omics biomarker discovery in cancer. *Briefings in Bioinformatics, 27*. https://doi.org/10.64898/2025.12.18.695266
     
    MohdFaizal, A., Hon, W.-Y., Thevarajah, T., Khor, S. M., & Chang, S.-W. (2023). A biomarker discovery of acute myocardial infarction using feature selection and machine learning. *Medical & Biological Engineering & Computing*, 1 - 15. https://doi.org/10.1007/s11517-023-02841-y
     
    Ng, S., Masarone, S., Watson, D., & Barnes, M. R. (2023). The benefits and pitfalls of machine learning for biomarker discovery. *Cell and Tissue Research, 394*, 17 - 31. https://doi.org/10.1007/s00441-023-03816-z
     
    Njume, C. M., Petracci, I., Bellini, S., Goljanek‐Whysall, K., Quinlan, L. R., Fiszer, A., Borroni, B., Ghidoni, R., Kumbasar, A., & Çakmak, A. (2026). When complexity does not pay: benchmarking deep learning and ensemble methods for biomarker discovery. *Briefings in Bioinformatics, 27*. https://doi.org/10.1093/bib/bbag211
     
    Papoutsoglou, G., Tarazona, S., Lopes, M. B., Klammsteiner, T., Ibrahimi, E., Eckenberger, J., Novielli, P., Tonda, A., Simeon, A., Shigdel, R., Béreux, S., Vitali, G., Tangaro, S., Lahti, L., Temko, A., Claesson, M., & Berland, M. (2023). Machine learning approaches in microbiome research: challenges and best practices. *Frontiers in Microbiology, 14*. https://doi.org/10.3389/fmicb.2023.1261889
     
    Shi, Z., Wen, B., Gao, Q., & Zhang, B. (2021). Feature Selection Methods for Protein Biomarker Discovery from Proteomics or Multiomics Data. *Molecular & Cellular Proteomics : MCP, 20*. https://doi.org/10.1016/j.mcpro.2021.100083
     
    Singh, A., Shannon, C., Gautier, B., Rohart, F., Vacher, M., Tebbutt, S., & Cao, K.-A. L. (2019). DIABLO: an integrative approach for identifying key molecular drivers from multi-omics assays. *Bioinformatics*. https://doi.org/10.1093/bioinformatics/bty1054
     
    Wang, X., Nguyen, J., Nader, K., Miihkinen, M., Wall, P., Singhal, A., Bedard, P., Ideker, T., Aittokallio, T., & Haibe-Kains, B. (2026). Discovery of predictive biomarkers for cancer therapy through computational approaches. *Nature Reviews Clinical Oncology, 23*, 180 - 200. https://doi.org/10.1038/s41571-025-01109-8
     
    Zenbout, I., Bouramoul, A., Meshoul, S., & Amrane, M. (2023). Efficient Bioinspired Feature Selection and Machine Learning Based Framework Using Omics Data and Biological Knowledge Data Bases in Cancer Clinical Endpoint Prediction. *IEEE Access, 11*, 2674-2699. https://doi.org/10.1109/access.2023.3234294
     
    Zhang, X.-K., Jonassen, I., & Goksøyr, A. (2021). Machine Learning Approaches for Biomarker Discovery Using Gene Expression Data. *Bioinformatics*. https://doi.org/10.36255/exonpublications.bioinformatics.2021.ch4
 

Good, I will read, in this order:

- `[Njume et al., 2026]`: tests the many different possible pipelines:
    - 'deep learning models did not outperform simpler classifiers'
    - 'Triple-omics yielded the highest validation'
- `[Ng et al., 2023]`
- `[Dhillon et al., 2022]`

## References

