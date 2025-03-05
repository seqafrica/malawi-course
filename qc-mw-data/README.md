# Malawi data QC

Here are the MultiQC reports for the first NICD run of CG isolates:

 - [Reads QC _before_ trimming](https://zwets.it/course/malawi/qc-mw-data/01-pre/index.html)
 - [Reads QC _after_ trimming](https://zwets.it/course/malawi/qc-mw-data/02-post/index.html)
 - [Assembly QC](https://zwets.it/course/malawi/qc-mw-data/03-asm/index.html)

> MultiQC integrates the output of other QC tools, such as FastQC
> and Quast in an "interactive" HTML document.

The run was overall high quality, but there were issues with a few
isolates.

### Read Quality

Take a look at the _pre-trimming_ report.  One thing to notice is the high
percentages of duplicate reads.  This may indicate an issue during library
prep or with the input DNA.

However this is not the most notable issue in the data.  Scroll through
to find this issue, which necessitates trimming.  Then check in the
post-trimming report that trimming has indeed solved the issue.

### Assembly Quality

Examine the Assembly QC report.  There is one assembly that has amazing
quality, one with very good quality, and four of good quality.  Which are
these and why do we rate them good quality?

One of the good quality assemblies has one suspicious feature.  Which one
do we mean?

Inversely, one assembly has terrible quality.  Which one is this and what
is so bad about it?  What is a likely cause?

The five remaining assemblies are quite poor.  What metric is indicative
of this?

