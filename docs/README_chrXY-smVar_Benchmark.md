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
[2022 to 2023-09-25]

### Background
The chrXY small variant benchmark for SNV's and small indels less than 50bp in size
was created using the T2T HG002 complete assembly of chromosomes X and Y. This benchmark 
includes more challenging regions, like segmental duplications, that were excluded 
from previous GIAB benchmarks. The benchmark includes 94.5% of X and 63.3% of Y 
in GRCh38, of 294 medically relevant genes on these chromosomes, 270 are >90% included 
and 251 are >99% included in the XY small variant benchmark regions, as well as some 
challenging regions like 68.2% of segmental duplications, 0.2% of satellite DNA, 
99% of XTR. A higher fraction (4.9%) of indels are large indels 15 to 49 bp in 
size compared to the v4.2.1 benchmark (2.6%). Also, a higher fraction (30.3%) 
of indels are in tandem repeats compared to the v4.2.1 benchmark (20.9%).

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

*.bed : bed file with small variant benchmark regions.  
*vcf.gz : bgzipped vcf file with benchmark small variants.

### File List with md5s:
**SmallVariant/**  
96e20f3a7c74ff71c2d96c1fe9c91d5f	HG002_GRCh38_chrXY_smallvar_v1.0.bed    
881bcfc624506871f0537575cf1badbc	HG002_GRCh38_chrXY_smallvar_v1.0.vcf.gz    
efacd65872b081095b5ae2bb8b53b78a	HG002_GRCh38_chrXY_smallvar_v1.0.vcf.gz.tbi   

**SmallVariant/SupplementaryFiles/T2T-XY-v2.7-align2-GRCh38/**     
5d038e758ec4a8180317ef950a0cb99f	GRCh38_T2T-XY-v2.7_dipcall-z2k.dip.bed  
99b98c697b161343088ef54b0d62c9aa	GRCh38_T2T-XY-v2.7_dipcall-z2k.dip.vcf.gz  
90954d3042e0cac2d39bc1483b8caf86	GRCh38_T2T-XY-v2.7_dipcall-z2k.hap1.bam  
d157c2ac9ccd6c78a1795e45f8b23a82	GRCh38_T2T-XY-v2.7_dipcall-z2k.hap1.bam.bai  
3bfa03087f53eeb342d8107f88aef7eb	GRCh38_T2T-XY-v2.7_dipcall-z2k.hap2.bam  
0014483d2e5b97812f82535c8373f127	GRCh38_T2T-XY-v2.7_dipcall-z2k.hap2.bam.bai


METHODOLOGICAL INFORMATION
--------------------------------------------------------------------------------

To create a small variant benchmark for SNVs and small indels less than 50 bp in size, we align the T2T assembly (v2.7) of HG002’s X and Y to GRCh38 and call variants with [dipcall](https://github.com/lh3/dipcall) that was developed during the course of the syndip effort. Files in `SmallVariant/SupplementaryFiles/T2T-XY-v2.7-align2-GRCh38/` are the alignment files produced by dipcall. 

We then exclude regions where assembly-based small variant calling is unreliable and/or benchmarking tools are unreliable. Examples include loci with more than one contig aligning (except in the X PAR), structural variants at least 50 bp in size (and the entire tandem repeat for SVs in tandem repeats), large repeats (segmental duplications, tandem repeats, and satellites) that have any breaks in the assembly-assembly alignment, regions around gaps in GRCh38, homopolymers longer than 30 bp, tandem repeats discordant with a different assembly, and homopolymers discordant with Element avidity-based sequencing variant calls. 


NIST Data Use Policy
--------------------------------------------------------------------------------

This data/work was created by employees of the National Institute of Standards and Technology (NIST), an agency of the Federal Government. Pursuant to title 17 United States Code Section 105, works of NIST employees are not subject to copyright protection in the United States.  This data/work may be subject to foreign copyright.

The data/work is provided by NIST as a public service and is expressly provided “AS IS.” NIST MAKES NO WARRANTY OF ANY KIND, EXPRESS, IMPLIED OR STATUTORY, INCLUDING, WITHOUT LIMITATION, THE IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT AND DATA ACCURACY. NIST does not warrant or make any representations regarding the use of the data or the results thereof, including but not limited to the correctness, accuracy, reliability or usefulness of the data. NIST SHALL NOT BE LIABLE AND YOU HEREBY RELEASE NIST FROM LIABILITY FOR ANY INDIRECT, CONSEQUENTIAL, SPECIAL, OR INCIDENTAL DAMAGES (INCLUDING DAMAGES FOR LOSS OF BUSINESS PROFITS, BUSINESS INTERRUPTION, LOSS OF BUSINESS INFORMATION, AND THE LIKE), WHETHER ARISING IN TORT, CONTRACT, OR OTHERWISE, ARISING FROM OR RELATING TO THE DATA (OR THE USE OF OR INABILITY TO USE THIS DATA), EVEN IF NIST HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

To the extent that NIST may hold copyright in countries other than the United States, you are hereby granted the non-exclusive irrevocable and unconditional right to print, publish, prepare derivative works and distribute the NIST data, in any medium, or authorize others to do so on your behalf, on a royalty-free basis throughout the world.

You may improve, modify, and create derivative works of the data or any portion of the data, and you may copy and distribute such modifications or works. Modified works should carry a notice stating that you changed the data and should note the date and nature of any such change. Please explicitly acknowledge the National Institute of Standards and Technology as the source of the data:  Data citation recommendations are provided at https://www.nist.gov/open/license.

Permission to use this data is contingent upon your acceptance of the terms of this agreement and upon your providing appropriate acknowledgments of NIST’s creation of the data/work.
