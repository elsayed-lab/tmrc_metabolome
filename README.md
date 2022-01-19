# TMRC3 Metabolomics analyses

This directory is intended to contain some shared analyses of the
TMRC3 data in combination with some MS/MS metabolomics data.

# Requisites

In its current iteration, this requires a couple of rda files from the
TMRC3 analyses.  They reside in the 'rda' directory therein as
'visit_monocyte_gluc_table-v202011.rda' and
'visit_biopsy_gluc_table-v202011.rda'.

These files contain the differential expression results when comparing
the three visits against each other (v2/v1, v3/v1, v3/v2) for only the
biopsy or monocyte samples from people who were treated with
glucantime (Meglumine antimoniate).

The analyses in their current form were performed in the section:
'Comparing visits without regard to cure/fail' in the tmrc3 worksheet
'tmrc3_reorganized_202111.Rmd'.

# Tasks

In our last conversation, Najib and Maria Adelaida suggested that we
do the following:

1.  Extract the significant genes from the v3/v1 monocytes.
2.  Extract the significant genes from the v3/v1 biopsies.
3.  Perform a set of GSEA on these results.
4.  Potentially perform a set of GSVA on their source datasets.
5.  Compare these results to the results from MetaboAnalyst.
6.  Create pathway diagrams of the genes and metabolites, on the same image.
  a.  Perform this for a specific set of pathways.

# Shift of focus

It appears we will also try to compare the KEGG results from the two
separate directions: from the metabolites and from the genes.  To that
end, we will attempt to color KEGG pathway diagrams with the human
genes and metabolites simultaneously.
