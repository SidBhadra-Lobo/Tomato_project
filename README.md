#Tomato Project

**So far**
 
* I have downloaded and assembled tomato reference genome <ftp://ftp.solgenomics.net/tomato_genome/assembly/build_2.50/>,  `S_lycopersicum_build_2.50_chr1-12.fa`, script is [`tomato_wget_assemble.sh`](scripts/tomato_wget_assemble.sh) 

* Wrote a script that concatenates all sequences associated with probes of idenitcal ids, [`make_probe_fasta.fa`](scripts/make_probe_fasta.sh)

* Wrote a script that then uses blastn to align the concatenated probe fastas against the tomato reference genome, [`blastn_tomato.sh`](scripts/blastn_tomato.sh).
 
Done - Right now I'm making 5937 fastas from the 65535 probes from [`Tomato.probe_tab_1.txt`](./Tomato.probe_tab_1.txt), then aligning those fastas.

Done - Made blast table of all probes against tomato refgen [`full_blastn.table`](./full_blastn.table) , out format 7, default threshold, culling limit 1.

**Currently**

Done - Wrote [`gene_match.sh`](scripts/gene_match.sh) to match up the GeneIDs from [`Gene_ID_tabdelim.txt`](Gene_ID_tabdelim.txt) to the concatenated fasta probes. And matched them up to the already generated respective BLAST outputs, to generate the final complete [table](Gene_ID_fulltable.txt).
