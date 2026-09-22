# data/

Sequences in FASTA format, the inputs for every later step.

| File | Contents |
|---|---|
| `query_[GENE]_[accession].fasta` | Starting protein (Step 1) |
| `novel_[species]_[nucleotide-accession].fasta` | Translated novel candidate (Step 3) |
| `msa_input.fasta` | All sequences used in the alignment (Step 5) |

List the sequences in `msa_input.fasta` with their accessions:

| Name | Species | Accession |
|---|---|---|
| [name] | [species] | [accession] |
