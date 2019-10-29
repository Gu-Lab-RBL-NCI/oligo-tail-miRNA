# miRNA trimming and oligo-tailing analysis
R scripts used to analyze miRNA isoforms trimming and tailing (as well as nucleotide composition of non-templated tails).

* **Analysis of TCGA mutants:**
  * [AGO2](https://github.com/Gu-Lab-RBL-NCI/oligo-tail-miRNA/tree/master/AGO2%20mutants)
    * [GDC Portal AGO2 missense mutations](https://portal.gdc.cancer.gov/exploration?facetTab=mutations&filters=%7B%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22genes.gene_id%22%2C%22value%22%3A%5B%22ENSG00000123908%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22ssms.consequence.transcript.consequence_type%22%2C%22value%22%3A%5B%22missense_variant%22%5D%7D%7D%5D%2C%22op%22%3A%22and%22%7D&searchTableTab=mutations)
  * [AGO1](https://github.com/Gu-Lab-RBL-NCI/oligo-tail-miRNA/tree/master/AGO1%20mutants)
    * [GDC Portal AGO1 missense mutations](https://portal.gdc.cancer.gov/exploration?facetTab=mutations&filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22genes.gene_id%22%2C%22value%22%3A%5B%22ENSG00000092847%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22ssms.consequence.transcript.consequence_type%22%2C%22value%22%3A%5B%22missense_variant%22%5D%7D%7D%5D%7D&searchTableTab=mutations)
* **Analysis of long tail composition:**
  * [Long tail composition](https://github.com/Gu-Lab-RBL-NCI/oligo-tail-miRNA/tree/master/Long%20Tail%20Composition)
  * [Descriptive example of the analysis performed](https://github.com/Gu-Lab-RBL-NCI/oligo-tail-miRNA#minimum-number-of-n-nucleotide-in-tail)

### Minimum number of "N" nucleotide in tail

**miRBase reference**
```
>hsa-miR-7-5p MIMAT0000252
UGGAAGACUAGUGAUUUUGUUGUU
```

**Example long tailed read**
```
<--templated-----------><--non-templated-->
UGGAAGACUAGUGAUUUUGUUGUUUUUUUUUAAUUUUGUCUUU
........................UUUUUUUAAUUUUGUCUUU

Number of U in tail: 15
Number of A in tail: 2
Number of G in tail: 1
Number of C in tail: 1
```

### References:
* [QuagmiR: A Cloud-based Application for IsomiR Big Data Analytics.](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/bty843/5123434)
Bofill-De Ros X, Chen K, Chen S, Tesic N, Randjelovic D, Skundric N, Nesic S, Varjacic V, Williams EH, Malhotra R, Jiang M, Gu S. Bioinformatics. 2018 Oct 8. doi: 10.1093/bioinformatics/bty843.([Pubmed link](https://www.ncbi.nlm.nih.gov/pubmed/30295744))
