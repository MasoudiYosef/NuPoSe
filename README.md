# NuPoSe: Nucleosome positioning prediction

<p align='justify'> 
NuPoSe is a deep-learning framework that predicts nucleosome positioning and identifies related features. Figure 1 illustrates NuPoSe's framework, which comprises four main steps.
</p>

![NuPoSe](https://github.com/MasoudiYosef/NuPoSe/assets/83264279/73dd3cd5-7a70-4d45-8b58-1047fb2c4296)
<p align='center'>The framework of NuPoSe</p>

<p align='justify'>
In the first step (Figure 1a), high-coverage data of paired-end 147 bp length MNase-seq fragments from seven human lymphoblastoid cell lines (GSE36979) were aligned to the human reference genome (GRCh37). Subsequently, the alignment scores were smoothed, and the dyad positions were determined. The file named <i>DyadMNase.zip</i> contains all the necessary files and bash-format commands, which can be executed on the Ubuntu operating system. Using the determined dyad positions, two groups of DNAs were generated: the positive group representing 201-bases nucleosomal DNA and the negative group representing 201-bases non-nucleosomal DNA.
</p>


<p align='justify'>
In the second step (Figure 1b), a total of 336 di-nucleotide, tri-nucleotide, and tetra-nucleotide sequence patterns were defined for each DNA strand in the positive and negative datasets. Subsequently, five groups of features were extracted for each sequence pattern. The python-format file named FeatureExtraction.py contains the source code for extracting these features. To execute this source code, the following commands were used:
  <br><br>
<b>python3 FeatureExtraction.py PG<br>
python3 FeatureExtraction.py NG</b>
  <br><br>
Here, 'PG' and 'NG' refer to two text files containing 201-base nucleosomal and non-nucleosomal DNAs, respectively. Running these source codes converts every 201-base DNA sequence into a set of over 32,000 features.
</p>
