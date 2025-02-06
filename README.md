# Malawi Course repo

Repository to hold notes, files and links for the Malawi training.

Currently private but we will make this public so participants can download files,
find links, reread instructions, etc.

Home: <https://github.com/seqafrica/malawi-course>


## Programme

 * Google doc: <https://docs.google.com/document/d/1oN3s6jiw1a7ccOcbP2N_ZHP_qV_GEZgAjZKRn4Mt56M/edit?tab=t.0>




## Enterobase

Explore any dataset (for the nine species that Enterobase covers) that is publicly
available in the SRA and/or your own uploaded isolates.  Illumina short reads only.

Enterobase has GrapeTree built in, but you can also use it standalone.

#### Links:

 * Site: <https://enterobase.warwick.ac.uk/>
 * Documentation: <https://enterobase.readthedocs.io/en/latest/>


## Grapetree

Software to produce a "grape tree" from

 - A newick file (the standard format for phylogenetic trees), or
 - A list of MLST profiles (of any kind: classic, cgMLST, wgMLST, rMLST, ...), or
 - A multiple sequence alignment (FASTA), or
 - Indeed _any table with samples down the rows and attributes across the columns_

A GrapeTree visualises the distances between samples as measured quite simply by
the number of columns on which they differ (i.e. do not have identical values).

It collapses samples into "grapes" when the samples are identical across the columns,
or within some chose threshold distance.  The size of each grape represent the number
of samples in it.

The graph becomes interesting when you colour the grapes with a metadata attribute,
such as location, collection date, or some predicted phenotype (AMR, serotype, etc).

#### Links:

 * Documentation: <https://enterobase.readthedocs.io/en/latest/grapetree/>
 * Repository: <https://github.com/achtman-lab/GrapeTree>

#### Installation:

 * Linux: use conda: `conda create -n grapetree -c bioconda grapetree`
 * Windows/Mac: download is available [here](https://github.com/achtman-lab/GrapeTree/releases)

#### Usage:

See the [documentation](https://enterobase.readthedocs.io/en/latest/grapetree/),
or dive straight in:

@TODO@: add cgMLST and metadata sample here
@TODO@: add an MSA as well?

 1. Upload a newick tree, MLST profile, or multiple sequence alignment
   - MLST profile must be TSV, have a header, must start with `#`

 2. Upload a metadata table
   - Must be TSV, header must _not_ start with `#`

Use the various controls to format it.  Tutorials and tips are available in the
Enterobase and GrapeTree on-line documentation.

Your work will be stored in a Workspace that you can later reload.
