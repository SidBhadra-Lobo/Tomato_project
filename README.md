#Tomato Project

*So far I have downloaded and assembled the tomato reference genome,  `S_lycopersicum_build_2.50_chr1-12.fa`. 

*Wrote a script that concatenates all sequences associated with probes of idenitcal ids, `make_probe_fasta.fa`

*Wrote a script that then uses blastn to align the concatenated probe fastas against the tomato reference genome, `S_lycopersicum_build_2.50_chr1-12.fa`
 
**Currently**

Right now I'm making 5937 fastas from the 65535 probes from `Tomato.probe_tab_1.txt`, then aligning those fastas.
