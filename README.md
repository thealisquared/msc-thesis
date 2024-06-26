# msc-thesis

**Characterising Therapeutic Vulnerabilities in Colorectal Cancer, University of Glasgow (2020)**

This master's research was a transcriptomics project aiming to investigate the transcription-level effects of combination tyrosine kinase inhibitors in mouse models of aggressive colorectal cancer (CRC) and to identify the human populations which may benefit from these treatments. To achieve the second aim, the R-package CMSCaller was used, which provide Consensus Molecular Subtype (CMS) and Colorectal Cancer Intrinsic Subtype (CRIS) classifications of CRC pre-clinical models. 

CMS and CRIS are robust transcriptomic analyses of large scale CRC patient data sets characterising genomic, mutational, stromal, and immune profiles of whole CRC tumours and cancer cell-specific traits excluding the stroma respectively. Additionally, each CMS and  CRIS signature has unique gene expression traits and clinical outcomes. In the pre-clinical setting of this project, subtyping mouse CRC can cross-compare biological characterisation and clinical outcomes to human CRC. Therefore, CMSCaller not only allowed to identify the drug-induced change in biological characterisation of the cancers but also determined the prognostic value offered by the combination treatments. In this way, a shift from a poor prognostic subtype to a better prognostic subtype will signify response to treatment.

In CMSCaller, the raw gene expression data and the human Entrez IDs were inputted into R to replace the ENSEMBLE gene IDs in the expression data with the equivalent human Entrez IDs since CMSCaller recognises the latter. The script then performs the CMS and CRIS calls to subtype each of the four replicates in the treated and control by calculating a distance value to each subtype classification. Finally, a heat map was created using the average CMS and CRIS subtyping distance value for each treatment and control group.

**Acknowedgement:**

The project was supervised by Andrew Campbell at CRUK Scotland Institute. The R-script was written with the training and support of Kathryn Gilroy at CRUK Scotland Institute.

**References:**

Eide, P.W., Bruun, J., Lothe, R.A. et al. CMScaller: an R package for consensus molecular subtyping of colorectal cancer pre-clinical models. Sci Rep 7, 16618 (2017). https://www.nature.com/articles/s41598-017-16747-x

Guinney, J., Dienstmann, R., Wang, X. et al. The consensus molecular subtypes of colorectal cancer. Nat Med 21, 1350–1356 (2015). https://www.nature.com/articles/nm.3967

Isella, C., Brundu, F., Bellomo, S. et al. Selective analysis of cancer-cell intrinsic transcriptional traits defines novel clinically relevant subtypes of colorectal cancer. Nat Commun 8, 15107 (2017). https://www.nature.com/articles/ncomms15107
