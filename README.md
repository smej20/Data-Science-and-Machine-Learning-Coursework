# SARS-CoV-2 (COVID-19) Analysis 

This Jupyter Notebook was written to provide a working example of how computer languages such as Python and packages such as Biopython can be utilised to analyse and interpret a genomic sequence using the example of the SARS-CoV-2 (COVID-19) genomic sequence. This has been further developed from work discussed during the Presentation Workshop. This type of analysis allows scientists to gleam further information which can be utilised in conjunction with experimental analyses'. It should be noted that this Jupyter Notebook can be adapted for any genomic sequence supplied in a fasta style format. 


To run this Jupyter Notebook:
    
    1. Ensure that all the packages and functions are downloaded and imported onto your system. These are provided in the first section of the SARS-CoV-2 (COVID-19) Analysis Jupyter Notebook.
    
    2. Example data should be downloaded within the same directory, this includes the SARS-CoV-2 (COVID-19) sequence (MN908947.fna), as well as the fasta sequences for SARS (SARS.fasta.txt) and MERS(MERS.fasta.txt). The sequence for COVID-19 was obtained from  https://www.nature.com/articles/s41586-020-2008-3 but can also be found on NCBI GenBank using the accession number MN908947. The sequences for SARS and MERS can also be found on GenBank using the NCBI Reference Sequences NC_004718.3 and NC_019843.3 respectively. All of which can also be found on the associated GITHUB page. If using different sequence files, ensure to change the file names within the code to match the new files.
    
    3. For the code to run, it is important that each cell is run in the order it was written within the Jupyter Notebook otherwise error messages will be likely to occur.
    
    
In this analysis, the SARS-CoV-2 (COVID-19) sequence was interrogated. The number of each respective nucleotide base was counted and the GC content % calculated. These were then printed to observe the results.The sequence was then translated and transcribed into its amino acids and specific protein chains were identified where stop codons (*) were present.

Protein sequences less than 20 amino acids were removed and collated into a dataframe which can be exported into an excel xlsx file. Individual fasta files were also created for each protein sequence identified. This Jupyter Notebook also provides code for calculating certain properties of each suggested protein sequence, including: Amino Acids Percent, Molecular Weight, Aromaticity, Flexibility, Isoelectric Point and Secondary Structure Fraction. Again, code is provided to write these observations into an xlsx file. Code is provided to further interrogate the Molecular Weight property through the visual aid of a bar chart. This can be done with any of the potential protein sequences identified by changing the index number from the poi_list. The longest protein sequence identified was chosen for further investigation, Peptide_49.fasta, as it was considerably larger than the remaining discovered protein sequences.

Peptide_49.fasta was then searched against NCBI's Protein Blast Non-redundant database within Python. Other sequences could also be searched for using this code with this specific database or the code could be edited to utilise other databases including the nucleotide database. Peptide_49.fasta matched to the ORF1ab polyprotein in SARS-CoV-2 (COVID-19) which plays an important role in RNA synthesis, providing a potential therapeutic target for the disease. 

This Jupyter Notebook also provides code for primer design using Primer3. Here, primers were designed for the ORF1ab polyprotein identified. Three separate regions within this protein was designated for primer design, with five separate primer pairs being designed for each specificed region. The code for primer design also includes some parameters which can be changed based upon user preference, including maximum/minimum TM, GC% and size allowed. Code is also provided to write the results into an excel file. The code used here can also be modified to include a number of different sequences or different regions of a particular sequence for primer design. 

Finally, this Jupyter Notebook also provides code to align and compare the similarity in sequence between SARS-CoV-2 (COVID-19) and both Severe Acute Respiratory Syndrome (SARS-CoV-1 ) and Middle East Respiratory Syndrome (MERS-CoV). This found that SARS-CoV-1 is most similar to the COVID-19 sequence. Different sequences may also be compared using this code by modifying the names of the files used to match the new file names and editing the names of the comparisons. 



    
   
