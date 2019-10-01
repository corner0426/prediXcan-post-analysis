# PrediXcan post analysis



## Define gwas loci from plink output

### Use plink to identify independent loci (index snps)

```shell
cd /data/myl/WGS_Data_for_analysis
plink --noweb --bfile chrALL_1329_samples_MAF_0.01_new_beagle --clump-p1 5e-8 --clump-kb 500 --clump-r2 0.05 --clump 1_chrALL_1329_samples_MAF_0.01_MDS_Smoking_additive.assoc.logistic --out /data1/yaoyh/prediXcan/prediXcan_post_analysis/indep_loci/Smoking_indep
```



 ### Define loci
We defined an associated locus as the physical region containing all SNPs correlated at r2 > 0.6 with each of the 128 index SNPs. .[PMID: 25056061].(https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4112379/)

