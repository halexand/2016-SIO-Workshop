======================================
Gene Abundance Estimation with Salmon
======================================

Salmon is one of a breed of new, very fast RNAseq counting packages. Like Kallisto and Sailfish, Salmon counts fragments without doing up-front read mapping. Salmon can be used with edgeR and others to do differential expression analysis.

The goals of this tutorial are to:

*  Install salmon
*  Use prokka to annotate our genomes

Installing prokka
==================================================

Download and extract the latest version of salmon:
::
    wget https://github.com/COMBINE-lab/salmon/releases/download/v0.7.2/Salmon-0.7.2_linux_x86_64.tar.gz
    tar -xvzf Salmon-0.7.2_linux_x86_64.tar.gz
    cd Salmon-0.7.2_linux_x86_64

    
Running Salmon
==============

Make a new directory for the quantification of data with Salmon:
::
    mkdir quant
    cd quant

Grab the nucleotide (``*ffn``) predicted protein regions from Prokka and link them here. Also grab the trimmed sequence data (``*fq``)
::
    ln -fs annotation/prokka_annotation *ffn .
    ln -fs data/*.abundtrim.subset.pe.fq.gz .

Create the
References
===========
* http://www.vicbioinformatics.com/software.prokka.shtml
* https://www.ncbi.nlm.nih.gov/pubmed/24642063
* https://github.com/tseemann/prokka/blob/master/README.md
