# Supplementary-Repository-S1
All bioinformatics reports mentioned in the Results section are available here. To open the documents from this link, you must first download them. Once downloaded, several .html files will appear that can be opened with any web browser.

The reports are as follows:

  -	1.B. Differences between Tenebrio molitor larvae and adults – Bacteria
  -	1.F. Differences between Tenebrio molitor larvae and adults – Fungi
  -	2.B. Differences between T. molitor colonies in the larval stage – Bacteria
  -	2.F. Differences between T. molitor colonies in the larval stage – Fungi
  -	3.B. Differences between T. molitor colonies in the adult stage – Bacteria
  -	3.F. Differences between T. molitor colonies in the adult stage – Fungi
  -	4.B. Differences between treatments in T. molitor larvae – Bacteria
  -	4.F. Differences between treatments in T. molitor larvae – Fungi
  -	5.B. Differences between treatments in T. molitor adults – Bacteria
  -	5.F. Differences between treatments in T. molitor adults – Fungi

Each report includes results and figures for the following sections:

  1.	Introduction
  2.	Rarefaction curves of pooled samples
  3.	Taxonomic composition of pooled samples
  4.	Taxonomic composition by groups
  5.	Overall alpha diversity
  6.	Evenness index
  7.	Dominance
  8.	Beta diversity
  9.	Gamma diversity
  10.	Differential abundance
  11.	Krona plots

The differential abundance analysis using the DESeq2 package in R includes the following parameters:

  •	baseMean: the average abundance across all samples in the analysis.
  •	log2FoldChange: the log base 2 of the ratio between one group and another. A negative value indicates higher abundance in the reference (denominator) group, while a positive value indicates the opposite. For example, a log2FC of 1 (2¹) indicates twice the abundance, and a value of 2 (2²) indicates four times the abundance.
  •	lfcSE: the standard error of the log2FoldChange.
  •	stat: the value of the test statistic used in the comparison.
  •	pvalue: the p-value from the test under the null hypothesis of no significant difference between group means.
  •	padj: the adjusted p-value. When performing multiple comparisons, p-values are adjusted to reduce the number of false positives. The most commonly used method is FDR (False Discovery Rate), also known as the Benjamini-Hochberg correction.
  •	comp: the specific comparison being analysed.
  •	ref: the reference group, which serves as the denominator in the ratio.
