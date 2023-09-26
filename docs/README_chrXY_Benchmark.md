The chrXY Benchmark README was generated 2023-09-26 by Jennifer McDaniel, NIST.

GENERAL INFORMATION
--------------------------------------------------------------------------------

### Title of Dataset
HG002 chromosome X and Y small variant benchmark


###  Principal Investigator(s)
Name: Justin M. Zook  
Institution: National Institute of Standards and Technology (NIST)  
Email: jzook@nist.gov

### Dataset Contact(s)
Name: Justin Wagner  
Institution: National Institute of Standards and Technology (NIST)  
Email: justin.wagner@nist.gov

Name: Jennifer McDaniel   
Institution: National Institute of Standards and Technology (NIST)  
Email: jennifer.mcdaniel@nist.gov

### Dates of Data Collection
[MM-DD-YYYY to MM-DD-YYYY]

### Background
The chrXY small variant benchmark for SNV's and small indels less than 50bp in size
was created using the T2T HG002 complete assembly of chromosomes X and Y. This benchmark 
includes more challenging regions, like segmental duplications, that were excluded 
from previous GIAB benchmarks. The benchmark includes 94.48892% of X and 63.28961% of Y 
in GRCh38, of 294 medically relevant genes on these chromosomes, 270 are >90% included 
and 251 are >99% included in the XY small variant benchmark regions, as well as some 
challenging regions like 68.23813% of segmental duplications, 0.1549578 of satellite DNA, 
99% of XTR. A higher fraction - 4.8723613% - of indels are large indels 15 to 49 bp in 
size compared to the v4.2.1 benchmark - 2.6117621%. Also, a higher fraction - 30.3060056% - 
of indels are in tandem repeats compared to the v4.2.1 benchmark - 20.895619%.

### Data Usage

### Limitations
Significant fractions of GRCh38 X and Y are excluded from the small variant benchmark,in addition to the 0.73% of X and 53% of Y missing from GRCh38, such as the large human satellites in the X centromere and Y heterochromatin.

SHARING/ACCESS INFORMATION
--------------------------------------------------------------------------------

### Licenses/restrictions placed on the data, or limitations of reuse: 
See NIST license and data use policy at the end of the document.

### Recommended citation for the data:
**Benchmark Manuscript**

	Small variant benchmark from complete assembly of X and Y chromosomes of HG002 - Pending

**Assembly Manuscripts** 

	Rhie, A. et al. The complete sequence of a human Y chromosome. Nature 621, 344–354 (2023).
	Nurk, S. et al. The complete sequence of a human genome. Science 376, 44–53 (2022).

### Links to publicly accessible locations of the data:
- [HG002 chrXY small variant benchmark files](https://ftp-trace.ncbi.nlm.nih.gov/ReferenceSamples/giab/release/AshkenazimTrio/HG002_NA24385_son/chrXY/GRCh38/SmallVariant)


DATA & FILE OVERVIEW
--------------------------------------------------------------------------------

HG002_GRCh38_chrXY_smallvar_v1.0.bed : bed file with small variant benchmark regions.
HG002_GRCh38_chrXY_smallvar_v1.0.vcf.gz : bgzipped vcf file with benchmark small variants.

### File List with md5s:
96e20f3a7c74ff71c2d96c1fe9c91d5f	HG002_GRCh38_chrXY_smallvar_v1.0.bed  
881bcfc624506871f0537575cf1badbc	HG002_GRCh38_chrXY_smallvar_v1.0.vcf.gz  
efacd65872b081095b5ae2bb8b53b78a	HG002_GRCh38_chrXY_smallvar_v1.0.vcf.gz.tbi  


METHODOLOGICAL INFORMATION
--------------------------------------------------------------------------------

To create a small variant benchmark for SNVs and small indels less than 50 bp in size, 
we align the T2T assembly of HG002’s X and Y to GRCh38 and call variants with 
[dipcall](https://github.com/lh3/dipcall) that was developed during the course of 
the syndip effort.8 We then exclude regions where assembly-based small variant calling 
is unreliable and/or benchmarking tools are unreliable

NIST Data Use Policy
--------------------------------------------------------------------------------

This data/work was created by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 17 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States.  This data/work may be subject to foreign copyright.

The data/work is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the world.

You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data:  Data citation recommendations are provided at https://www.nist.gov/open/license.

Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data/work.
