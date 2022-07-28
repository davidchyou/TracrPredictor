# TracrPredictor
**What it does**

This application finds tracrRNA genes in a genome with previously annotated CDS. It does this by utilizing the fact that the anti-repeat part if a tracrRNA is approximately, but in almost all cases not exactly, the reverse complement of a CRISPR repeat starting with a conserved GYY motif, and the tail part of the tracrRNA (i.e. after the anti-repeat) often start with a conserved AR motif. Furthermore, known tracrRNAs often located within 500 bases from a cas9 gene, although there are exceptions. The application uses a support-vector machine to calculate the probability of a true-positive tracrRNA prediction based on the above-mentioned features, without requiring a full match.

**The Galaxy server for TracrPredictor**

The TracrPredictor is currently available as a web application [under our galaxy server](http://139.80.3.3:8080/). However, source codes are available here in the zipped directory for downloading. Users will need to upload an “annotated” genome sequence file in GenBank format (gbk or gbff). Detailed usages are documened under the web interface.  
