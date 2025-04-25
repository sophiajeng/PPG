# PPG

scRNA-Seq tools for identifying HCMV transcripts involved in latency and reactivation of HCMV

1. Need to identify putative 3 prime UTR prior to alignment as 10X Genomics has a three prime bias
    1. To do this, we identify a stop codon and the closest polyA signal.  If no polyA signal can be found within 500 bp, we cut it off at 500 bp.
2. Once aligned reads have been filtered for Quality Control, and normalized using Harmony, cells were clustered using Monocle.
3. For each cluster, we provide a heatmap of HCMV transcript expression for each sample type.
