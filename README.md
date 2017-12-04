# CEL2Mtx
Prepare CEL to expression set

For Affymetrix data, this R script can be used to convert raw CEL files into a
custom CDF normalized expression dataset that is compatible with CIBERSORT.


* customCDF should be downloaded from BrainArray(http://brainarray.mbni.med.umich.edu/Brainarray/Database/CustomCDF/CDF_download.asp)
(Entrez Gene Identifiers Only). Entrez v12.1.0 for HGU133A, along with 
v18 for HGU133A and HGU133Plus2.0 are provided above.
* To install, do not gunzip. Use following command 
(using hgu133plus2.0 v18 as an example, in a Linux environment):
```sudo R CMD INSTALL hgu133plus2hsentrezgcdf_18.0.0.tar.gz```
* Change cdfname in the provided R script if chipset is different
Choose mas5 or rma normalization 
(mas5 is default and rma is commented out). 一般来说用rma
