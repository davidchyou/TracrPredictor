# TracrPredictor
**What it does**

This application predicts tracrRNA genes in a genome with previously annotated CDS. It does this by utilizing the fact that the anti-repeat part if a tracrRNA is approximately, but in almost all cases not exactly, the reverse complement of a CRISPR repeat starting with a conserved GYY motif, and the tail part of the tracrRNA (i.e. after the anti-repeat) often start with a conserved AR motif. Furthermore, known tracrRNAs often located within 500 bases from a cas9 gene, although there are exceptions. The application uses a support-vector machine to calculate the probability of a true-positive tracrRNA prediction based on the above-mentioned features, without requiring a full match.

**The Galaxy server for TracrPredictor**

The TracrPredictor is currently available as a web application [under our galaxy server](http://139.80.3.3:8080/) under the tab "CRISPR: TracrRNA Finder". However, source codes are available here in the zipped directory for downloading. Users will need to upload an “annotated” genome sequence file in GenBank format (gbk or gbff). Detailed usages are documened under the web interface.

Flat files showing the coordinates of tracrRNA on the genome, the structures of the repeat-anti-repeat hybrid and the tail-folding, and the prediction statistics are available in GFF and CSV formats, as well as reader-friendly TXT file.

**References**

Chyou D. T. and Brown C. M. (2018): Prediction and diversity of tracrRNAs from type II CRISPR-Cas systems. RNA Biology. [Link](https://pubmed.ncbi.nlm.nih.gov/29995560/)
