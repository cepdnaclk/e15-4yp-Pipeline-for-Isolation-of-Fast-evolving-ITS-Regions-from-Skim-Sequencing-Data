---
layout: home
permalink: index.html

# Please update this with your repository name and title
repository-name: e15-4yp-Pipeline-for-Isolation-of-Fast-evolving-ITS-Regions-from-Skim-Sequencing-Data
title: A User-friendly Pipeline for Isolation of Fast-evolving Internal Transcribed Spacer(ITS) Regions from Skim Sequencing Data
---

[comment]: # "This is the standard layout for the project, but you can clean this and use your own template"

# Project Title

#### Team

- E/15/016, Anojan S., [email](mailto:anojans1996@gmail.com)
- E/15/171, Kapilrajh R., [email](mailto:svkapilvs@gmail.com)
- E/15/351, Thakshajini S., [email](mailto:tsuhumar8@gmail.com)

#### Supervisors

- Dr. Asitha Bandaranayake, [email](mailto:asithab@eng.pdn.ac.lk)
- Prof. Pradeepa Bandaranayake, [email](mailto:pradeepag@agri.pdn.ac.lk)

#### Table of content

1. [Abstract](#abstract)
2. [Related works](#related-works)
3. [Methodology](#methodology)
4. [Experiment Setup and Implementation](#experiment-setup-and-implementation)
5. [Results and Analysis](#results-and-analysis)
6. [Conclusion](#conclusion)
7. [Publications](#publications)
8. [Links](#links)

---

## Abstract
DNA that resides within the nucleus of a cell is the primary genetic material that is responsible for genetic behaviours of various eukaryotic organisms such as plants, humans, animals, algae and fungi as well as prokaryotic organisms such as archaea and bacteria. Genome or DNA of an organism has several complex genomic regions. Specific genomic regions consist of several complex proteins. RNA is the replica of DNA involved in protein synthesis using these complex proteins and instructions carried from DNA. Ribosomes are small particles having these RNA molecules. Ribosomal DNAs are repeating units having fast-evolving as well as conserved subregions. Isolation of fast-evolving regions of rDNA is necessary for a more accurate and successful analysis of variation within and between species. ITS1 and ITS2 are the fast-evolving regions of rDNA that are widely preferred to differentiate various species including humans, plants and fungi. These regions have the highest probability of correct identification and ITS is the most frequently used molecular marker in species variation analysis. There are several computational tools and pipelines available in the literature to isolate ITS regions from different sequence datasets and to analyze the inter-species as well as intra-species variation using these fast-evolving genomic regions. Biologists don’t have a clear understanding on which is the most efficient and suitable computational tool or pipeline to extract and analyze the fast-evolving nuclear ribosomal ITS regions associated with various organisms since they don’t have sufficient computer knowledge. Hence, they find it difficult to select the best tool or technology required for the isolation and analysis process. Therefore, the purpose of our project is to compare the pros and cons of existing computational tools and pipelines based on various parameters such as the CPU time taken to run the software, CPU performance, accuracy, required computer memory and disk space and depending on other specifications to come up with an efficient procedure or pipeline to extract and analyze fast-evolving genomic regions from low coverage skim sequence data at a low cost. Hence, the primary objective of this project is to come up with a simple,user-friendly and efficient workflow or pipeline for the biologists to isolate fast-evolving genomic regions from skim sequencing data for phylogenetic studies.

## Related works
According to our literature review, previous several researches related to ITS regions, prove that ITS is a standard accepted metabarcode marker for several species including plants, fungi and human fungal pathogens. These researches also emphasize that ITS subregions ITS1 and ITS2 have the highest probability of correct identification within and between above mentioned species.

### 2.1 Justifications on ITS Regions

- One of the researches shows that it is possible to use the ITS2 region of rDNA to distinguish five different Cinnamomum species.
- Another review paper indicates that the ITS1 region is very useful for reliable identification of medicinal plants and phylogenetic analysis of Gambhari.
- One of the other articles related to DNA barcoding asserts  ITS1 and ITS2 regions as the standard metabarcoding markers to identify fungi species such as Basidiomycota.
- One of ther papers shows the use of Inter Simple Sequence Repeat (ISSR) markers together with nrDNA ITS sequences incorporated with leaf morphological characteristics to describe cladistic relationships between twelve different Cinnamomum species in Taiwan.
- In another research paper, highly repeated units of ITS showed distinguishable variation between individual Cerastoderma species in the phylogenetic analysis.
- Another group of researchers proved a more close phylogenetic relationship between polypoid Elymus plant species and other organisms using ITS sequences.
- One of the researches approved that utilizing ITS regions as molecular targets provided the higher potential for the characterization of human fungal pathogens.

### 2.2 Justifications on Software Tools and Pipelines

According to our literature review, there are various computational tools and pipelines used in several previous researches over the last one and a half-decade to extract and analyze ITS regions from different fungal sequencing datasets. Here, we have provided justifications based on those tools and pipelines.
     
- One of the researches shows that ITSx is a software tool to isolate ITS1, 5.8S and ITS2 and also full-length ITS sequences from both Sanger and NGS sequencing datasets.
- One of the researches of Professor H. Kauserud shows that extracting ITS1 sequences from 12 486 raw pyrosequencing ITS1 dataset using ITSx detected 12 410 ITS1 fungal sequences and he found the low quality or short length reads when examining the rest of the 76 sequences.
- Research related to ITSxpress shows that it is an improved software tool from ITSx that extends its capability from marker gene studies which use Operational Taxonomic Units (OTUs) to studies that use Exact Sequence Variants (ESVs).
- This research further justifies that using 4 cores, ITSxpress trimmed ITS1 region samples by a median of 23 times speeder than ITSx. ITSxpress trimmed the ITS2 region 14 times speeder  than ITSx. Clustering at 99.5 percent identity minimized the number of reads used for Hmmsearch by a median of 71 times for ITS1 region and 36 times for ITS2 region.
- Some researchers used  ITScan as an automated software pipeline to identify and analyze the variation of fungal species using ITS sequences.
- Another research related to PIPITS shows that it is also an automated pipeline to analyze fungal ITS sequences. It uses ITSx to isolate ITS subregions and utilizes the RDP classifier for the classification of sequences with the UNITE fungal sequencing dataset.
- One of the literature uses CloVR-ITS as a portable pipeline to utilize the analysis of fungal communities using ITS amplicon pyrosequencing data.
- A review paper related to Illumina Metabarcoding Pipeline describes it as a flexible software pipeline to extract and analyze ITS rDNA from Illumina Miseq sequencing data having paired-end reads.
- One of the other review papers on PlutoF justifies it as a web-based tool that includes the software tool to isolate and classify ITS sequences obtained from high-throughput sequencing datasets.
- Research associated with CLOTU indicates that it is a software pipeline which helps to speed up the process of analyzing fungal ITS sequences by providing high performance.
- One of the other review papers emphasizes that another Perl-based software pipeline is also available to automate the BLAST process and to extract ITS subregions from various ITS sequence datasets to speed up the analysis process.

Considering the above literature review justifications, these researches have focused on the importance of using ITS regions as a molecular marker for accurate fungal species variation analysis and the articles related to the software tool and pipelines to extract and analyze ITS regions mostly focusing on Fungal ITS sequences. Hence, these papers could not utilize these tools and pipelines to isolate ITS regions from plant and human skim sequence data. We have not found a review paper comparing the pros and cons of all the tools and pipelines. Therefore, through our research, we are going to do a comparative analysis between these software tools and pipelines to identify the best tool or technology or pipeline. Then, we are going to find whether they are applicable for plant and human skim sequence data and how much data is enough for the analysis.

## Methodology
First, we analyzed the software and hardware requirements of the software tools and pipelines that we identified from our literature review such as  ITSx, ITSxpress and PIPITS about how much RAM and disk space is needed to install each tool and what kind of input data is needed for each tool. Then, we identified whether we need to input skim data or contigs or scaffolds for these tools. After that, we installed these tools ITSx, ITSxpress and PIPITS with all the other required tools in our department aiken server using the anaconda environment. 

Next, we have collected the data that separately contains forward and reverse raw reads of different Cinnamomum species such as Cinnamomum Capparu Coronde, Cinnamomum Verum and Cinnamomum Zeylanicum. Then, we tested these tools using the given cinnamomum capparu coronde data containing the forward raw reads around 19 GB and reverse raw reads around 19 GB. We recorded the output and the CPU time for each tool.We earlier got empty files as output for the tools earlier and it took a very long time to obtain the output in akien server.

As a result, we got some ITS regions and we verified those output ITS regions by blasting agianst NCBI nr/nt database to make sure we exactly got the ITS regions of cinnamomum species. We did a comparative analysis of the tools based on the CPU time and the similarity of the ITS regions to identify the better tool which is much efficient and accurate. Further, we analyzed the steps of the existing pipeline PIPITS to come up with a similar pipeline by improving it.

We used the tool seqtk to partition different sizes of the collected data such as 1GB, 2GB,3GB and 5GB for both forward and reverse raw reads in order to test our pipeline. Earlier, We ran our pipeline in our department aiken server for 1GB and 2GB data of cinnamomum capparu coronde and recorded the respective run times of each tool that performs the relevant step. Then, we shifted to agbc server later because the aiken server was responding too slow. As a result, we have experienced much improved performance for each tool of our pipeline in agbc server compared to aiken server. Hence, we tested the same 1GB and 2GB data in agbc server and recorded the improved run times with respect to each tools of the pipeline.

In the first step of our pipeline, we have done the quality checking of the reads to find the GC content, no of low quality reads and other relevant characteristics of the reads.Then, we filtered out the low quality reads using fastqc. However, we couldn't filter out both forward and reverse reads simultaneously using that tool. Therefore, we found another tool afterqc to filter out both forward and reverse reads at the same time and tested it successfully.

After quality filtering, we ran ITSx by directly using the good quality forward and reverse raw reads as input to extract ITS regions. However, we failed in the process and we found that the read length 150bp is not sufficient to extract ITS regions using ITSx. Therefore, we needed to assemble the forward and reverse reads to get contigs in order to maximize the read length. Hence, we used the assembler Spades to obtain the contigs in fasta format. In the next step, we ran ITSx using the resultant contigs in fasta format for the aforementioned different sizes of data separately. 

Meanwhile, we also converted the obtained contigs from fasta format to fastq format using the tool seqtk since ITSxpress only accepts fastq format input files. Then, we used the resultant contigs in fastq format as input to ITSxpress to extract ITS regions. Here, we looked for more tools associated with fasta to fastq conversion and found the tool bbmap(reformat.sh) in addition to seqtk. Then, we compared the performance between seqtk and bbmap(reformat.sh) for 3GB and 5GB cinnamomum capparu coronde data and observed the difference in the recorded run times. Thereafter, we input the resultant fastq files obtained form both seqtk and bbmap(reformat.sh) to ITSxpress and compared the run times taken to get the output.

Earlier, when we ran ITSx using contigs as input for 1GB data, we got empty output file. Then, we merged the forward and reverse reads using the tool vsearch and ran ITSx again using the obtained merged reads as input. As a result, we got some ITS sequences as output. Then, we have checked the quality of the output and blasted to ensure that we got the exact ITS regions of cinnamomum species. However, we identified multiple sequences in the output. 

Further, we found that some of the sequences in contigs which are greater than 100kbp in read length is the reason behind getting these multiple sequences in the output. Therefore, we filtered out those sequences that are greater than 100kbp from the contigs file using the tool bbmap(reformat.sh). After that, we ran ITSx using the filtered contigs to extract ITS regions and we ended up getting some ITS sequences as output for cinnamomum capparu coronde 1GB data. When we checked the quality of the output this time, we found that there were no multiple sequences. 

Earlier, we ran ITS using the default mumber of threads which is only one CPU thread and later we increased the number of CPU threads from one to sixteen to run the ITSx. As a result, we found much improvement in the performance of ITSx. After that, we tried with different thread sizes for 1GB cinnamomum capparu coronde data and observed the deviation in the performance of ITSX with respect the increasing or decreasing thread sizes. 

Meanwhile, we faced no problem when directly using contigs obtained from spades as input to run ITSxpress and we got an ITS sequence as the output from ITSxpress for the same data. Then, we checked the quality of the ITSxpress output and blasted it to verify that the obtained ITS sequence belongs to cinnamomum species. Next, we compared the ITSxpress output with the ITSx output by doing multiple alignment to find whether both of them are same. 

Further, we tested our pipeline for 1GB cinnamomum verum and cinnamomum zeylanicum data as well using the same process and compared all the results of both ITSx and ITSxpress for the three cinnamomum species based on the performance and quality of the output obtained by blasting the output sequences and doing multiple alignment to obtain the distance matrix.

## Experiment Setup and Implementation

## Results and Analysis

## Conclusion

## Publications
1. [Semester 7 report](./)
2. [Semester 7 slides](./)
3. [Semester 8 report](./)
4. [Semester 8 slides](./)
5. Author 1, Author 2 and Author 3 "Research paper title" (2021). [PDF](./).


## Links

[//]: # ( NOTE: EDIT THIS LINKS WITH YOUR REPO DETAILS )

- [Project Repository](https://github.com/cepdnaclk/e15-4yp-Pipeline-for-Isolation-of-Fast-evolving-ITS-Regions-from-Skim-Sequencing-Data)
- [Project Page](https://cepdnaclk.github.io/e15-4yp-Pipeline-for-Isolation-of-Fast-evolving-ITS-Regions-from-Skim-Sequencing-Data)
- [Department of Computer Engineering](http://www.ce.pdn.ac.lk/)
- [University of Peradeniya](https://eng.pdn.ac.lk/)

[//]: # "Please refer this to learn more about Markdown syntax"
[//]: # "https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet"
