# Getting started

This file explains how to set up and maintain your Find-a-Gene repository. Delete it before the final submission on Dec 1.

## 1. Create your repository from this template

1. Open https://github.com/ravichas/bifx550-find-a-gene-template/generate, or go to the template page and click **Use this template**, then **Create a new repository**.
2. Set **Owner** to your own GitHub account.
3. Name the repository `bifx550-find-a-gene-<lastname>`, all lowercase, for example `bifx550-find-a-gene-smith`.
4. Choose **Public**, then click **Create repository**.

Your repository starts with this folder structure and the README placeholders. It does not share history with the template.

## 2. Fill in the README

Open `README.md`, click the pencil icon, and replace the items in angle brackets as your results come in. Commit each edit with a short message that says what changed.

## 3. Add files

Each folder has its own `README.md` listing the files that belong there and how to name them.

### Option A: upload in the browser

1. Open the folder the file belongs in, for example `results/blast/`.
2. Click **Add file**, then **Upload files**, and drag the files in.
3. Write a commit message, for example `Add tBLASTn results`, and click **Commit changes**.

To create a new folder, click **Add file**, then **Create new file**, and type the folder name followed by `/`.

### Option B: push from Google Colab or a terminal

Use the course GitDemo notebook for the one-time setup (token, Colab Secrets, configuration, clone). After that, each update follows the same pattern:

```
cp /content/novel_candidate.fasta data/
git add data/novel_candidate.fasta
git commit -m "Add translated novel candidate sequence"
git pull --rebase origin main
```

then push with `push_to_github()` in Colab, or `git push origin main` in a terminal where you are signed in to GitHub.

## 4. Commit at each milestone

The commit history is graded, so commit as you work rather than once at the end.

| Milestone | Due | Commit at least |
|---|---|---|
| bifx550a | Oct 6 | Query and novel sequences in `data/`; BLAST output in `results/blast/` |
| bifx550b | Nov 17 | Alignment in `results/msa/`; tree file and image in `results/tree/` |
| bifx550c and Final | Dec 1 | Structure files in `results/structure/`; report in `report/`; completed README and analysis log |

## 5. Check against the rubric (15 points)

| Criterion | Points | Where it lives |
|---|---|---|
| Repository organization | 4 | Folder structure; completed root `README.md` |
| Reproducibility | 5 | Analysis log in `scripts/README.md`; inputs in `data/` |
| Results files | 3 | Report in `report/`; FASTA, alignment, tree file, structure images or model |
| Professionalism | 3 | Public repository; commits across the term; no junk files |

## 6. Keep the repository clean

- `.gitignore` already excludes notebook checkpoints, system files, and Word lock files.
- GitHub rejects files over 100 MB. From ColabFold or AlphaFold output, commit the top-ranked model and the confidence images, not the full zip archive.
- Before Dec 1, remove leftover placeholders and delete this file.

## About this Template

Prepared by Sarangan Ravichandran, PhD, PMP, for BIFX-550 Computational Functional Genomics, Hood College, Fall 2026. 

Use of AI tools: this template was drafted in collaboration with Claude (Anthropic). The instructor reviewed and edited all content. 
