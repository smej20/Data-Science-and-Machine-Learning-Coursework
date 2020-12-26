COVID-19 Analysis 

Use this file to explain purpose of what I am doing and how the code works.
This Jupyter Notebook can be adapted to use for any fasta sequence which requires investigation i.e. if another world pandemic was to strike once again. 
Primer functionality, can be used for any supplied sequence.
Blast functionality, can be used for any supplied sequence.

Primer design could also be used for mulitple sequences?
Interpret and analyse 

fasta_string = open(i+".fasta").read()

result_handle = NCBIWWW.qblast(
"blastp",
"nr",
fasta_string,
)
save_file = open("out.xml", "w")

save_file.write(result_handle.read())

save_file.close()

result_handle.close()

add alignment???