# Malawi Course repo

Repository to hold notes, files and links for the Malawi training.

Currently private but we will make this public so participants can download files,
find links, reread instructions, etc.

Home: <https://github.com/seqafrica/malawi-course>


## Programme

 * Document: [Malawi_training_agenda_final.docx](Malawi_training_agenda_final.docx) (copied below)


## Day 1

### WGS Overview

Overview of whole genome sequencing (WGS) technologies and their laboratory roles.

 * Presentation: [???]

TODO: <https://nanoporetech.com/blog/how-oxford-nanopore-sequencing-works> has very nice animation <https://youtu.be/RcP85JHLmnI>.

Review basic bioinformatics concepts: file formats and sequence data types.

 * Talk: bioinformatics 101

Hands-on exercise:

 * See the [mystery/README.md](mystery/README.md)

### Introduction to Online Tools

Demonstrations

 * BLAST
 * Galaxy, Epi2me, PathogenWatch, CGE, “Assembly Server”, Illumina Dragen, Terra Bio, etc.

Hands-on work

 * 

## Day 2

### Quality Control (QC) and Assembly

Presentation:

Demonstration:

Hands-on:

### Assembly Theory, Exercises, and QC

        ◦ Presentation:
            ▪ Assembly Approaches:
                • Reference-based vs. de‑novo assembly (including de Bruijn graphs).
                • Issues such as contamination and high contig counts.
            ▪ Assembly Types:
                • Long, short, and hybrid assemblies.
            ▪ Tools like BV‑BRC for assembly.
            ▪ Quality Assessment:
                • QC tools such as QUAST, MultiQC, CheckM, and BUCO.
        ◦ Hands-On Exercises:
            ▪ Generate assemblies (ideally using participants’ own data) via the BV‑BRC Assembly Service.
            ▪ Evaluate assembly quality using QC reports (reference QC reports from NICD as examples).
            ▪ Run assemblies through BLAST to further assess their quality.


## Day 3

### Typing and AMR Analysis using Online Platforms

    • Presentation:
        ◦ Compare traditional lab-based typing methods with bioinformatics approaches.
        ◦ Typing Methods:
            ▪ KmerFinder (including kmer theory), MLST (using tools like KMA), serotyping, PlasmidFinder, VirulenceFinder.
            ▪ Additional tools: VirulenceFinder and PlasmidFinder.
    • Hands-On Exercise:
            ▪ Review Marco’s slides on building a ResFinder/PlasmidFinder workflow.
            ▪ Build your own Resfinder/PlasmidFinder with MyDBFinder (upload section from a 16S reference database, download from NCBI).

Instructions in [mydbfinder](mydbfinder).

            ▪ AMR package for R - determining MDR 


### Hands on AMR exercises

    • Review & Discussion:
        ◦ Revisit CGE results and discuss findings.
    • AMR Overview Presentation:
        ◦ Clinical significance and mechanisms of resistance (briefly).
        ◦ Importance of surveillance and the genotype‑to‑phenotype correlation in AMR reporting (include Marco’s story on cholera).
    • Hands-On Exercises:
        ◦ Use web‑based tools for AMR gene detection (e.g., ResFinder, PathogenWatch, MEFinder, PlasmidFinder).
        ◦ Discuss interpretation of results and the importance of consensus among tools (e.g., comparing ResFinder, AMRFinderPlus, CARD; demo Harmonize if possible).
        ◦ Examine HTML reports generated from assemblies.


## Day 4

### Bacterial Typing and Phylogenetic Analysis via Online Tools

Focus: Leveraging online platforms for bacterial typing and exploring phylogenetic relationships.
Morning Session 9:00-12:00: Bacterial Typing Overview
    • Presentation - Overview of Typing Methods:
        ◦ Introduction to methods such as MLST and cgMLST and their applications in tracking AMR epidemiologically.
        ◦ Discussion on SNP and cgMLST analysis (kmer distance vs. SNPs vs genes/alles).
    • Additional Topics:
        ◦ Use of multiple sequence alignment (MSA) and tree-building tools.
        ◦ Overview of tools such as CSI Phylogeny, MinTyper, and BEAST (including rooted trees, bootstrapping, and clock/time analysis).
    • Demonstration:
        ◦ Live demo using Enterobase.

### Afternoon Session 13:00-17:00: Hands-On Phylogenetic Analysis & Simulated Outbreak Scenario
    • Hands-On Exercise:
        ◦ Participants work with sample datasets to generate and visualize phylogenetic trees using online tools such as GrapeTree, Microreact, and iTOL.
    • Theory & Discussion:
        ◦ Interpreting tree topology and understanding outbreak clusters.
        ◦ Discuss practical implications for AMR surveillance.
    • Simulated Outbreak Scenario
        ◦ Tasks:
            ▪ Identify AMR genes using a web‑based tool.
            ▪ Perform bacterial typing and generate a phylogenetic tree.
            ▪ Interpret the integrated results to propose potential clinical and epidemiological actions.
    • Wrap-Up:
        ◦ Q&A session and final discussion


## TODO: InterpretAMR / AMRgen, AMRrules

<https://github.com/interpretAMR>

**AMRgen**:

AMRgen is an open-source R package designed to bridge the gap between genotypic and phenotypic antimicrobial resistance (AMR) data. Developed as an extension to the AMR R package, it provides tools to interpret AMR genes, integrate these findings with antimicrobial susceptibility test (AST) data, and calculate genotype-phenotype associations.

This package is developed in collaboration with the ESGEM-AMR Working Group and is tailored for researchers and healthcare professionals tackling AMR globally.

Also:

From their github page:

We are partnering with ESGEM, the ESCMID Study Group on Epidemiological Markers, to form an ESGEM-AMR Working Group to curate organism-specific rule sets. Membership of the working group is open to anyone with relevant expertise, you do not have to be an ESGEM member.

If you would like to get involved, please:

    Consider registering to attend one of the intro sessions to find out if this is the group for you:

    Tues 14 May 17:00 UK / 9:00 Seattle / 12:00 Boston
    Weds 15 May 9:00 UK / 15:00 Hanoi / 18:00 Melbourne

    If you decide you want to join the ESGEM-AMR working group please register your interest, and let us know what organism/s you have expertise in, using this form.

 
## Enterobase

Explore any dataset (for the nine species that Enterobase covers) that is publicly
available in the SRA and/or your own uploaded isolates.  Illumina short reads only.

Enterobase has GrapeTree built in, but you can also use it standalone.

#### Links:

 * Site: <https://enterobase.warwick.ac.uk/>
 * Documentation: <https://enterobase.readthedocs.io/en/latest/>


## Grapetree

See [grapetree/README.md](grapetree/README.md)

