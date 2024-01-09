# NuPoSe: Nucleosome positioning prediction

<p align='justify'> 
NuPoSe is a deep-learning framework that predicts nucleosome positioning and identifies related features. The figure below illustrates NuPoSe's framework, which comprises four main steps.
</p>

![NuPoSe](https://github.com/MasoudiYosef/NuPoSe/assets/83264279/73dd3cd5-7a70-4d45-8b58-1047fb2c4296)

<p align='justify'>
In the first step, high-coverage data of paired-end 147 bp length MNase-seq fragments from seven human lymphoblastoid cell lines (GSE36979) were aligned to the human reference genome (GRCh37). Subsequently, the alignment scores were smoothed, and the dyad positions were determined. The file named <i>DyadMNase.zip</i> contains all the necessary files and bash-format commands, which can be executed on the Ubuntu operating system. 
</p>
