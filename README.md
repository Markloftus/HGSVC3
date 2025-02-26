# HGSVC3
Code written for a subset of analyses found in the HGSVC3 manuscript (https://www.biorxiv.org/content/10.1101/2024.09.24.614721v1). 

You will see four folders. Each folder contains jupyter notebooks of the code written for those sections (in no particular order). 
  - __IsoSeq__: This contains the underlying code for how we were phasing long reads to the assemblies.
    -   PhasingReads_HGSVC3_WorkingVersion.ipynb - proto read phaser which was later put together onto the Clemson HPC.
  - __MEI__: This contains scripts for analyzing the MEI (Mobile Element Insertions) call sets.
    -   CleanDataset_DeduplicateCalls.ipynb - code for additional callset refinement (deduplicating PAV calls (e.g., two SVAs at same site with variable VNTRs but same element become one call) etc.).
    -   CompareOrthogonalCallset.ipynb - comparing against MELT LRA callset for concordance.
    -   HGSVC3_Centromere_MEIs_Chr2.ipynb - MEIs on the chr2 centromere/initial visualization of insertion locations. 
    -   HGSVC3_Centromere_MEIs_Chr20-New.ipynb - MEIs on the chr20 centromere/initial visualization of insertion locations. 
    -   HGSVC3_Filter_PALMER_and_Konkel_Unique_Calls.ipynb - run proto-L1ME-AID on PALMER only calls to check for sequence quality. Filter out calls missing tails, older elements, etc. 
    -   Part1_HGSVC3_Filter_Calls_06_17-2024.ipynb - initial filtering of PAV MEI calls. 
    -   Part2_HGSVC3_MERGE_MEI_Callsets-T2T_Merge.ipynb - Merge PALMER T2T-CHM13 calls with L1ME-AID+PAV T2T-CHM13 calls.
    -   Part2_HGSVC3_MERGE_MEI_Callsets-hg38Merge.ipynb - Merge PALMER GRCh38 calls with L1ME-AID+PAV GRCh38 calls.
    -   Total_T2T_INS_and_REF_INS_Calls_Heatmap-Copy1.ipynb - visualize with a heatmap the T2T-CHM13 reference and sample specific MEI calls. 
    -   Total_hg38_INS_and_REF_INS_Calls_Heatmap.ipynb  - visualize with a heatmap the GRCh38 reference and sample specific MEI calls. 
  - __MHC__: Code for analyzing the Major Histocompatibility Complex (HLA-DRB, and RCCX analyses specifically).
    - DR1_Haplotype_Recombination.ipynb
    - DR8_Recombination.ipynb
    - DRA_Check.ipynb
    - DRB_Pull_Sequence_Code.ipynb
    - HGSVC3_DR_Haplotype_Alignment_SNVs.ipynb
    - Par1_Clean_HLA_HeaderNames-Copy1.ipynb
    - Part1_Clean_HLA_HeaderNames.ipynb
    - Part2_a_Primate_Human_C4_CYP21A2_RepeatMaskerRuns_Jan2024.ipynb
    - Part2_allGeneLocations_MHCLocus_December122023-DRB_Specific-Final_BuildsDataframes_Important.ipynb
    - Part3_BuildTrainingData_Allchr6Gene_RepeatMasker_ReadIn-Copy1.ipynb
    - Part3_PullC4_CYP21A2_Sequences.ipynb
    - Part4.1_EDITED_Human_Visualizations-gene_simplified-Copy1.ipynb
    - Part4.1_Human_Visualizations-gene_simplified.ipynb
    - Part4_Human_Primate_C4_CYP21A2_Visualizations-withAllRepeats.ipynb
    - Part4_Human_RCCX_Visualizations-withAllRepeats.ipynb
    - Part5_Human_Primate_C4_CYP21A2_Visualizations-Nucleotide.ipynb
    - Part6_Human_Primate_C4_CYP21A2_Visualizations-AminoAcid.ipynb
    - Part7_HLA-C4_Network_Nucleotide_Master.ipynb
    - Part8_HLA-C4_VariantTable-November-VariantProblem.ipynb
  - __SMN__: Code to analyze SMN (also NAIP, SERF1, GTF2H2)  gene copy numbers.
    - SMN_CopyNumbers.ipynb

