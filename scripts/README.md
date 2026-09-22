# scripts/

Commands, notebooks, and scripts used in the analysis, plus the analysis log below. For web tools, the log is the method: record enough that someone else could repeat the step and get the same result.

## Analysis log

| Step | Tool and version or access date | Input | Key parameters | Output |
|---|---|---|---|---|
| 2 | [NCBI tBLASTn, web, YYYY-MM-DD] | `data/query_...fasta` | [database: wgs; organism: taxon; matrix; E-value threshold] | `results/blast/tblastn_...` |
| 4 | [NCBI BLASTp, web, YYYY-MM-DD] | `data/novel_...fasta` | [database: nr] | `results/blast/blastp_...` |
| 5 | [tool, version] | `data/msa_input.fasta` | [settings] | `results/msa/...` |
| 6 | [tool, version] | `results/msa/...` | [method; model; bootstrap replicates] | `results/tree/...` |
| 7 | [tool, version] | `data/novel_...fasta` | [settings; PDB ID compared] | `results/structure/...` |
