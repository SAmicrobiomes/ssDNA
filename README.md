## The detection of Marine associated ssDNA viruses using HMM profiles
### The following are steps we followed to build HMM profiles used in the search for ssDNA viruses in our metagenomes
1. Download Cressdnaviricota and Phixvirota protein sequences from GenBank;
2. Cluster these at ```95%``` amino acid identity over ```90%```of the shortest sequence using CD-HIT;
3. Compare representative sequences using all-vs-all blastp with evalue ```1e-5```;
4. 


