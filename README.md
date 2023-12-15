The three data files provide the trimmed data used in each analysis. These SNPs have been selected for having a significance value below p = 10^(-5), which have then been transformed.

Significance Data.xlsx contains the SNPs used in the significance analysis, which looked at differences in p-value of each SNP per trait category. This also represents the entirety of the dataset - all studies were included in this analysis.

Effect Data.xlsx contains the SNPs used in the effect size analysis. This is a subset of the previous data, using data from studies that provided effect sizes of every significant SNP.

Proportion Data.xlsx contains the SNPs used in the proportion of significant SNPs analysis. This was calculated by dividing the number of significant SNPs per trait by the total SNPs included in the original GWA analysis. This proportion then underwent a logit transformation, ln(p/1-p), where p is the raw proportion.

Within the data files, the columns contain the following information:
  Study - name of the study SNPs derived from. See "Study Citations and Information.xlsx" file for link to the study.
  Trait - the trait within that study that was tested.
  AbsEffect - the absolute value of effect size for that SNP.
  transformed_pvalue - the negative log of the p-value.
  Category - the trait category assigned to that SNP - Behavioral, Morphological, or Physiological.
  Data.Type - the type of data that was collected, continuous or binary.
  DGRP.lines - the number of lines of flies included in that study.
  tranformed_proportion - within the proportion data file, this column contains the logit-transformed proportion as described above.

Study Citations and Information.xlsx - this file contains information on every trait and study, including total SNPs in that study and a link to the paper.

Analysis Code.txt - note that the Excel files listed above have been transformed to .csv files, that were then analyzed in R.
