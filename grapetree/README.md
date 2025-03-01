# GrapeTree

Software to produce a "grape tree" from

 - A newick file (the standard format for phylogenetic trees), or
 - A list of MLST profiles (of any kind: classic, cgMLST, wgMLST, rMLST, ...), or
 - A multiple sequence alignment (FASTA), or
 - Indeed _any table with samples down the rows and attributes across the columns_

A GrapeTree visualises the distances between samples as measured quite simply by
the number of columns on which they differ (i.e. do not have identical values).

It collapses samples into "grapes" when the samples are identical across the columns,
or within some chosen threshold distance.  The size of each grape represent the number
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

Run without arguments to start an interactive browser session, with arguments
to generate a Newick tree from the data using one of several methods.

See the [documentation](https://enterobase.readthedocs.io/en/latest/grapetree/),
or dive straight in:

 1. Upload a newick tree, MLST profile, or multiple sequence alignment
   - MLST profile must be TSV, have a header, must start with `#`

 2. Upload a metadata table
   - Must be TSV, header must _not_ start with `#`

@TODO@: add cgMLST and metadata sample here
@TODO@: add an MSA as well?

Use the various controls to format it.  Tutorials and tips are available in the
Enterobase and GrapeTree on-line documentation.

