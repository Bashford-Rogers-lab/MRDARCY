**This code will perform network clustering of BCRs from multiple samples.** This was named "MRD Assessment and Retrieval Code in pYthon" (MRDARCY), and was originally developed to identify leukaemic clones in follow-up samples for the early and sensitivity detection of MRD. However, this can be applied to any sets of samples for a comparison of clones. 


MRDARCY developed by Rachael Bashford-Rogers (2018) at the University of Oxford and Univeristy of Cambridge
**E-mail:** rbr1@well.ox.ac.uk

If you find the methods in MRDARCY, please cite the following reference: Bashford-Rogers, R. J., et al. (2016). "Eye on the B-ALL: B-cell receptor repertoires reveal persistence of numerous B-lymphoblastic leukemia subclones from diagnosis to relapse." Leukemia 30(12): 2312-2321.

**Installation**
Pre-requisites: CD-hit (installed from https://github.com/weizhongli/cdhit)

Edit line 1152 to point to your cd-hit location

This can be run straight from download (not compilation needed)


**Usage:**
python3 MRDARCY_2.2.py <input sample id file>  <sample number from input file> <command number>

<input sample id file> should be a tab delimited file with the following columns:
	Column 1: Group name
	Column 2: Sample name
	Column 3: Annotation file location (the corresponding IMGT "3_Nt-sequences.txt" file)
	Column 4: Fasta file location
	Column 5: Output directory
	Column 6: Annotation file type (IMGT or ImmuneReceptorAnnotator or Single_Cell)

<command number>:
	1: Merge files
	2: Align sequences from largest clones

e.g.
python3 MRDARCY_2.0.py Sample_example.txt 1 1



