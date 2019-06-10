### Description

The **genome** is the complete genetic sequence of a living organism, i.e. the list of the nucleotides containing all the genetic instructions used for its growth, development, functioning and reproduction.

A genome basically consists of two parts:

* the *genes*, which are the coding regions of the DNA influencing a particular phenotype by encoding the information necessary to transcript a protein;

* the *non-coding DNA*, which is mostly involved in the transcriptional and translational regu- lation of protein-coding sequences.

The set of all the proteins that can be transcripted by a genome is called *proteome*. Proteins may be classified according to their function (metabolism, transcription, ...) or their structure ($\alpha$-helix, $\beta$-sheets, ...). In this last case, it is possible to divide them into the so-called *protein domains* or *families*.

We collected the nucleotidic sequence of 10 PFAMs which results to be present in the over- whelming majority of the known proteomes, thus suggesting they may play fundamental roles within them.

The aim of the project is to apply the PCA clustering algorithm to the sequences associated to each PFAM to see whether they are connected to a taxonomic level (order, family or genus) of the proteome to which they belong or not.

### Assignments

* define a proper distance between strings of possibly different lengths (e.g. maximum overlap)
* calculate the distance between each pair of nucleotidic sequence thus building the distance matrix
* apply the PCA to this matrix
* colour the points in the first two principal components according to a fixed taxonomic level (TaxaTab).

### Datasets

The file *SequencesCorePFAM_PF0053.txt* contains the aminoacid sequences with which the PFAM PF0053 appears in the different proteomes of the databases. In particular, the file is organized as follows:
* in odd lines you will find the information on the proteome to which the PFAM belongs and the protein in which it has been found.

Example: ">1000565.tsv/F5REM1" means that the PFAM is contained in the proteome with ID code 1000565 and that it has been found in its protein named F5REM1.

* in even lines you will found the amino-acid sequences associated to that PFAM in such a proteome.

Example: *RVKRGVTARARHKKVLDQAKGYRGRRKSVYRIAKEAVMKAGQYAYRDRRQRKRQFRSLWIVRINAAARELGMTYSALINGLNKASIQVDRKVLADLAVFDKAAFAAI*

The file *TaxaTab_proteomes_bacteria.csv* contains the taxonomy of all the proteomes appearing in odd lines of the file *SequencesCorePFAM_PF0053.txt*. For example, for proteome 1000565, you will find the scientific name, (second column) together with the super kingdom, class, order, family, genus and species to which it belongs.

### Contacts

* Anna Tovo <anna.tovo@unipd.it>
* Samir Suweis <samir.suweis@unipd.it>
