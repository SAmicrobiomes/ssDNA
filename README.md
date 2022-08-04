## The detection of Marine associated ssDNA viruses using HMM profiles
![Alt text](?[CRESS Kazlauskas Matthew Figure 3.pdf](https://github.com/SAmicrobiomes/skulminatore/files/9258121/CRESS.Kazlauskas.Matthew.Figure.3.pdf)
raw=true "")
### The following are steps we followed to build HMM profiles used in the search for putatuve ssDNA viruses in our metagenomes
1. Download Cressdnaviricota and Phixvirota protein sequences from GenBank;
2. Cluster these at ```95%``` amino acid identity over ```90%```of the shortest sequence using CD-HIT;
3. Compare representative sequences using all-vs-all blastp with evalue ```1e-5```;
4. The blastp results were further clustered using MCL - Markov Clustering Algorithm with the inflation ```1.5```;
5. Clusters with proteins >= 10 annotated as replication initiator (Rep) and major capsid (VP1) were aligned using mafft with the ```--auto``` parameter;
6. 




