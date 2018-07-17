[asm_release] Arachis hypogea, version 2.0 (NOTE: renamed to gnm1 for release)

Assembly Stats:
---------------
Main genome scaffold total: 384
Main genome contig total:   4037
Main genome scaffold sequence total: 2556.9 MB
Main genome contig sequence total:   2553.0 MB (->  0.2% gap)
Main genome scaffold N/L50: 9/135.2 MB
Main genome contig N/L50:   461/1.5 MB
Number of scaffolds > 50 KB: 68
% main genome in scaffolds > 50 KB: 99.8%

 Minimum    Number    Number     Total        Total     Scaffold
Scaffold      of        of      Scaffold      Contig     Contig
 Length   Scaffolds  Contigs     Length       Length    Coverage
--------  ---------  -------  -----------  -----------  --------
    All       384      4,037  2,556,916,893  2,553,021,585    99.85%
   1 kb       384      4,037  2,556,916,893  2,553,021,585    99.85%
 2.5 kb       363      4,016  2,556,885,768  2,552,990,460    99.85%
   5 kb       341      3,994  2,556,802,470  2,552,907,162    99.85%
  10 kb       302      3,955  2,556,517,501  2,552,622,193    99.85%
  25 kb       133      3,785  2,553,855,160  2,549,969,160    99.85%
  50 kb        68      3,717  2,551,589,080  2,547,706,080    99.85%
 100 kb        42      3,688  2,549,925,018  2,546,045,018    99.85%
 250 kb        31      3,657  2,548,188,878  2,544,328,878    99.85%
 500 kb        28      3,631  2,547,178,637  2,543,341,637    99.85%
   1 mb        23      3,556  2,543,355,212  2,539,588,212    99.85%
 2.5 mb        20      3,462  2,538,283,725  2,534,607,725    99.86%
   5 mb        20      3,462  2,538,283,725  2,534,607,725    99.86%

Assembly Notes:
---------------

A total of 48.25x of PACBIO sequence (avg. read length of 11,525) was used to 
generate the initial MECAT assembly, which was subsequently polished using ARROW.
Synteny with the diploid A. duranensis and A. ipaensis, along with 1 genetic map and
2 synthetic maps (provided by David Bertioli) were used to identify misjoins in 
the raw assembly.  A total of 856 breaks were identified.  The broken assembly was
then scaffolded using HiC data by Rajeev Varshney.  Post scaffolding, 6 additional
breaks were made to resolve misjoins introduced during the scaffolding procedure.

A total of 7 tetrasomic regions were identified and duplicated in the following
chromosomes:

Chr01  No tetrasomic regions identified.
Chr02  2,322,927 bases were duplicated from the   end of B02 and added to the   end of A02
Chr03    342,613 bases were duplicated from the   end of A03 and added to the   end of B03
Chr04  2,767,012 bases were duplicated from the   end of B04 and added to the   end of A04
Chr05  6,264,747 bases were duplicated from the front of A05 and added to the front of B05
Chr06  2,501,280 bases were duplicated from the   end of A06 and added to the   end of B06
Chr07  1,099,346 bases were duplicated from the   end of A07 and added to the front of B08
Chr08  1,099,346 bases were duplicated from the   end of A07 and added to the front of B08
Chr09    193,833 bases were duplicated from the front of A09 and added to the front of B09
Chr10  No tetrasomic regions identified.

The original sequences were combined with the duplicated tetrasomic regions and joined 
together using 26 joins to create the 20 A. hypogaea chromosomes. During the construction of 
the chromosomes, all 500bp scaffolded gaps were converted to 1,000 bp gaps, and the map joins 
that were added consisted of 10,000 bp gaps.  Chromosomes were numbered as Arahy.01-Arahy.20, 
where the A genome is represented as Arahy.01-Arahy.10 and the B genome is represented as 
Arahy.11-Arahy.20.  99.3% of the assembled sequence is contained in the chromosomes.

Additionally, homozygous SNPs and INDELs were corrected in the release sequence using 
~40x of illumina reads (2x250, 800bp insert, library ID ICIH and ICID).  The table below provides 
the summary statistics of this correction:

Case                    Het_SNPs  Hom_SNPs  Het_INDELs  Hom_INDELs  Callable Bases (includes altHaps)
----                    --------  --------  ----------  ----------  --------------
Pre  SNP/INDEL fixing     39,908       762       5,098     136,607   2,285,156,312
Post SNP/INDEL fixing     44,300       199       4,875         735   2,300,218,064

Chromosome Stats:
-----------------

   Scaffold  Contigs   Scaffold Size    Basepairs     GC%
   --------  -------   -------------   -----------    ---
   Arahy.01    157      112,420,854    112,264,854   35.90%
   Arahy.02    195      102,981,163    102,751,163   35.91%
   Arahy.03    180      143,813,506    143,589,506   35.94%
   Arahy.04    238      128,801,742    128,555,742   36.54%
   Arahy.05    173      115,930,344    115,758,344   36.06%
   Arahy.06    213      115,504,342    115,283,342   36.48%
   Arahy.07    113       81,119,488     81,007,488   35.79%
   Arahy.08     45       51,897,010     51,844,010   33.47%
   Arahy.09    130      120,519,698    120,390,698   36.32%
   Arahy.10    236      117,088,237    116,853,237   36.15%

   Arahy.11    163      149,299,306    149,137,306   36.90%
   Arahy.12    136      120,579,088    120,444,088   36.10%
   Arahy.13    174      146,725,006    146,525,006   36.24%
   Arahy.14    152      143,237,272    143,086,272   36.49%
   Arahy.15    150      160,879,708    160,694,708   36.59%
   Arahy.16    222      154,808,347    154,560,347   36.61%
   Arahy.17    163      134,922,436    134,751,436   36.72%
   Arahy.18    206      135,150,084    134,927,084   36.65%
   Arahy.19    233      158,625,764    158,384,764   36.59%
   Arahy.20    183      143,980,330    143,798,330   36.75%

  Remaining	   575       18,633,168     18,633,168

PACBIO Coverage Stats:
------------------------

Cutoff      Reads       Basepairs Median Read Size Coverage
------ ---------- --------------- ---------------- --------
     0 10,089,743 130,266,939,667           11,525   48.25x
 1,000 10,089,743 130,266,939,667           11,525   48.25x
 2,000 10,089,743 130,266,939,667           11,525   48.25x
 3,000 10,089,743 130,266,939,667           11,525   48.25x
 4,000 10,088,907 130,263,676,016           11,525   48.25x
 5,000  9,840,623 129,083,983,051           11,734   47.81x
 6,000  9,041,368 124,685,043,428           12,433   46.18x
 7,000  8,243,303 119,499,596,383           13,168   44.26x
 8,000  7,465,522 113,668,991,396           13,914   42.10x
 9,000  6,721,099 107,345,617,458           14,652   39.76x
10,000  6,017,605 100,667,142,175           15,392   37.28x
11,000  5,365,727  93,827,183,866           16,133   34.75x
12,000  4,765,579  86,929,718,241           16,869   32.20x
13,000  4,211,417  80,006,254,436           17,606   29.63x
14,000  3,688,770  72,952,513,170           18,367   27.02x
15,000  3,192,321  65,757,429,239           19,172   24.35x
16,000  2,739,700  58,746,195,489           19,996   21.76x
17,000  2,331,934  52,021,933,439           20,842   19.27x
18,000  1,967,115  45,641,186,029           21,716   16.90x
19,000  1,647,049  39,723,897,425           22,614   14.71x
20,000  1,368,980  34,304,901,294           23,539   12.71x
21,000  1,130,944  29,428,363,245           24,500   10.90x
22,000    929,742  25,105,412,319           25,487    9.30x
23,000    762,774  21,351,263,767           26,490    7.91x
24,000    624,668  18,108,340,640           27,507    6.71x
25,000    512,072  15,351,684,079           28,524    5.69x
26,000    420,109  13,008,198,879           29,532    4.82x
27,000    344,925  11,017,169,186           30,532    4.08x
28,000    283,774   9,336,509,106           31,528    3.46x
29,000    233,119   7,893,669,201           32,531    2.92x
30,000    191,549   6,668,024,675           33,520    2.47x
31,000    157,308   5,624,257,583           34,494    2.08x
32,000    129,423   4,746,364,759           35,457    1.76x
33,000    106,160   3,990,632,913           36,416    1.48x
34,000     86,944   3,347,176,070           37,363    1.24x
35,000     71,068   2,799,739,503           38,287    1.04x
36,000     57,933   2,333,635,066           39,209    0.86x
37,000     46,852   1,929,339,804           40,157    0.71x
38,000     37,889   1,593,343,169           41,062    0.59x
39,000     30,384   1,304,557,901           41,977    0.48x
40,000     24,268   1,063,119,945           42,870    0.39x
41,000     19,235     859,374,791           43,782    0.32x
42,000     15,112     688,338,128           44,697    0.25x
43,000     11,727     544,559,333           45,639    0.20x
44,000      9,078     429,367,910           46,545    0.16x
45,000      6,972     335,695,736           47,392    0.12x
46,000      5,274     258,451,745           48,273    0.10x
47,000      3,953     197,039,744           49,200    0.07x
48,000      2,881     146,151,439           50,065    0.05x
49,000      2,103     108,437,767           51,015    0.04x
50,000      1,476      77,409,781           51,930    0.03x
51,000      1,058      56,309,917           52,720    0.02x
52,000        710      38,401,319           53,565    0.01x
53,000        469      25,758,022           54,415    0.01x
54,000        284      15,870,257           55,382    0.01x
55,000        173       9,820,902           56,133    0.00x
56,000         95       5,492,665           57,349    0.00x
57,000         54       3,181,679           58,119    0.00x
58,000         30       1,799,943           59,115    0.00x
59,000         16         983,084           60,734    0.00x

Completeness Notes:
-------------------
Completeness of the euchromatic portion of the genome assembly was assessed by
aligning the A. duranensis and A. ipaensis.  This is a routine test to determine 
whether we are missing significant portions of the genome.

36,732 out of 36,734 (99.99%) of the A. duranensis genes were found
41,838 out of 41,840 (99.99%) of the A. ipaensis genes were found


The scaffolds are divided into the following sets:
--------------------------------------------------
1) Main genome         (  384 scaffolds, 2,556.9 Mb )
2) Repeat scaffolds    (  406 scaffolds,     6.3 Mb )  ( < 150kb scaffolds composed of >=95% 24mers >4x in >=150kb scaffolds )
3) Unanchored rDNA     (    4 scaffolds,     1.5 Mb )
4) Alt. Haplotype      (    7 scaffolds,   186.1 Kb )  ( Scaffolds representing an alternative copy of an anchored allele )

