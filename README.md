## The detection of Marine associated ssDNA viruses using HMM profiles


<img src="https://user-images.githubusercontent.com/63568880/197710916-c9a1d903-e215-4b29-8c2f-4d3512628b79.png" width="370">

### The following are steps we followed to build HMM profiles used in the search for putative ssDNA viruses in our metagenomes
1. Retrieved Cressdnaviricota and Phixvirota protein sequences from [GenBank](https://www.ncbi.nlm.nih.gov/protein/?term=single+stranded+DNA+viruses);
2. Clustered these at ```95%``` amino acid identity over ```90%```of the shortest sequence using [CD-HIT](https://www.bioinformatics.org/cd-hit/);
3. Compared representative sequences using all-vs-all blastp with evalue ```1e-5```;
4. The blastp results were further clustered using [MCL - Markov Clustering Algorithm](https://micans.org/mcl/) with the inflation ```1.5```;
5. Clusters with proteins >= 10 representing replication initiator (Rep) and major capsid (VP1) were aligned using [mafft](https://mafft.cbrc.jp/alignment/software/) with the ```--auto``` parameter;
6. Alignments were then used to create HMM profiles using [hmmer](http://hmmer.org/) 




