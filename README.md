# SARS-CoV-2 (COVID-19) Analysis 

This Jupyter Notebook was written to provide a working example of how computer languages such as Python and packages such as Biopython can be utilised to analyse and interpret a genomic sequence using the example of the SARS-CoV-2 (COVID-19) genomic sequence. This type of analysis allows scientists to gleam further information which can be utilised in conjunction with experimental analyses'. It should be noted that this Jupyter Notebook can be adapted for any genomic sequences supplied in a fasta style format. 


To run this Jupyter Notebook:
    
    1. Ensure that all the packages and fucntion are downloaded and imported onto your system. These are provided in the first section of        the SARS-CoV-2 (COVID-19) Analysis Jupyter Notebook.
    
    2. Example data should be downloaded within the same directory, this includes the SARS-CoV-2 (COVID-19) sequence (MN908947.fna), as well as the fasta sequences for SARS (SARS.fasta.txt) and MERS(MERS.fasta.txt). Note: If using different sequences, ensure to change the file names within the code to match the new files.
    
    
In this analysis, the SARS-CoV-2 (COVID-19) sequence was interrogated. The number of each respective nucleotide base is counted, this produced the results: {'A': 8954, 'T': 9594, 'G': 5863, 'C': 5492}. The GC% was then calculated producing as result of 38%. The sequence was then translated and transcribed into its amino acids and specific protein chains were identified where stop codons were present.

Protein sequences less than 20 amino acids were removed and collated into a dataframe. Individual files were also created for each protein sequence identified. This Jupyter Notebook also provides code for calculating the 
Here, the longest protein sequence identified was chosen for further investigation as it was considerably larger than the remianing discovered protein sequences.




Primer functionality, can be used for any supplied sequence.
Blast functionality, can be used for any supplied sequence.

Primer design could also be used for mulitple sequences?
Interpret and analyse 

ORF1ab polyprotein in the SARS-CoV-2
~200bp difference between the different sequences. <i> SARS
    SARS/COVID19 Similarity (%):  83.33837518066619
MERS/COVID19 Similarity (%):  69.39141405757164
MERS/COV Similarity (%):  69.93714496991697