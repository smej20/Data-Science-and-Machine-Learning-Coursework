# SARS-CoV-2 (COVID-19) Analysis 

This Jupyter Notebook was written to provide a working example of how computer languages such as Python and packages such as Biopython can be utilised to analyse and interpret a genomic sequence using the example of the SARS-CoV-2 (COVID-19) genomic sequence. This type of analysis allows scientists to gleam further information which can be utilised in conjunction with experimental analyses'. It should be noted that this Jupyter Notebook can be adapted for any genomic sequences supplied in a fasta style format. 


To run this Jupyter Notebook:
    
    1. Ensure that all the packages and functions are downloaded and imported onto your system. These are provided in the first section of the SARS-CoV-2 (COVID-19) Analysis Jupyter Notebook.
    
    2. Example data should be downloaded within the same directory, this includes the SARS-CoV-2 (COVID-19) sequence (MN908947.fna), as well as the fasta sequences for SARS (SARS.fasta.txt) and MERS(MERS.fasta.txt). Note: If using different sequences files, ensure to change the file names within the code to match the new files.
    
    3. For the code to run, it is important that each cell is run in the order it was written within the Jupyter Notebook otherwise error messages are likely to occur.
    
    
In this analysis, the SARS-CoV-2 (COVID-19) sequence was interrogated. The number of each respective nucleotide base is counted, this produced the results: {'A': 8954, 'T': 9594, 'G': 5863, 'C': 5492}. The GC% was then calculated producing as result of 38%. The sequence was then translated and transcribed into its amino acids and specific protein chains were identified where stop codons were present.

Protein sequences less than 20 amino acids were removed and collated into a dataframe. Individual files were also created for each protein sequence identified. This Jupyter Notebook also provides code for calculating certain properties of each suggested protein sequence, including: Amino Acids Percent, Molecular Weight, Aromaticity, Flexibility, Isoelectric Point and Secondary Structure Fraction.

The longest protein sequence identified was chosen for further investigation, Peptide_49.fasta, as it was considerably larger than the remaining discovered protein sequences.

Peptide_49.fasta was then searched against NCBI's Protein Blast database within Python. Other sequences could also be searched for using this code. This matched to the ORF1ab polyprotein in SARS-CoV-2 (COVID-19) which plays an important role in RNA synthesis.

This Jupyter Notebook also provides code for primer design using Primer3. Here, primers were designed for the ORF1ab polyprotein identified. Three separate regions within this protein was designated for primer design, with five separate primer pairs being designed for each specificed region. The code used here can also be modified to include a number of different sequences or different regions of a particular sequence for primer design. 

Finally, this Jupyter Notebook also provides code to align and compare the similarity in sequence between SARS-CoV-2 (COVID-19) and both Severe Acute Respiratory Syndrome (SARS-CoV-1 ) and 
Middle East Respiratory Syndrome (MERS-CoV). This found that SARS-CoV-1 is most similar to the COVID-19 sequence sharing a shared sequence similarity of 83.3%, whilst MERS-CoV shared a sequence similarity of 69.4%. The code here can also be modifed and used to compare other sequences of interest.

In conclusion, this Jupyter Notebook has been developed to interpret and analyse the SARS-CoV-2 (COVID-19) sequence. However, any fasta sequence could be interrogated here. The information gathered here can be utilised, in conjunction with experimental data, to gain further understanding about a virus which has swept across the world. 
 
    
   