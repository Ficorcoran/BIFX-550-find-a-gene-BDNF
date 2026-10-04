# scripts/

Commands, notebooks, and scripts used in the analysis, plus the analysis log below. 

Carcharhinus cautus whole genome tBLASTn linux script for step 2 in `carcharhinus_cautus_genome_tBLASTn_script.txt`

## Analysis log

| Step | Tool and version or access date | Input | Key parameters | Output |
|---|---|---|---|---|
| 2 | NCBI tBLASTn, linux, 2026-10-02 | `data/query_human_BDNF_NP_001700.2.fasta` | database: Carcharhinus cautus assembly GCA_988281185.1; matrix: BLOSUM62; E-value threshold: 1e-5 | `results/blast/tblastn_carcharhinus_cautus_assembly_hits.txt` |
| 2 | NCBI tBLASTn, web, 2026-10-02 | `data/query_human_BDNF_NP_001700.2.fasta` | database: wgs; organism: Zearaja maugeana (taxid:496415); matrix: BLOSUM62; E-value threshold: 1e-5 | `results/blast/tblastn_wgs_zearaja_maugeana_hits.csv` |
| 4 | NCBI BLASTp, web, 2026-10-02 | `data/novel_carcharhinus_cautus_OZ558480.1-122450059-122450808.faa` | database: nr; matrix: BLOSUM62; E-value threshold: 1e-5 | `results/blast/blastp_nr_hits_carcharhinus_cautus.csv` |
| 4 | NCBI BLASTp, web, 2026-10-02 | `data/novel_zearaja_maugeana_JCCJZE010001961.1-1890706-1891428.faa` | database: nr; matrix: BLOSUM62; E-value threshold: 1e-5 | `results/blast/blastp_nr_hits_zearaja_maugeana.csv` |
| 5 | [tool, version] | `data/msa_input.fasta` | [settings] | `results/msa/...` |
| 6 | [tool, version] | `results/msa/...` | [method; model; bootstrap replicates] | `results/tree/...` |
| 7 | [tool, version] | `data/novel_...fasta` | [settings; PDB ID compared] | `results/structure/...` |
