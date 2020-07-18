

## File descriptions:

- `__ms.tex`: The main LaTeX document, mostly containing formatting.
  The only manuscript content in this file are the title, authors, and keywords.
- `##-<Description>.tex` files: These files are for the various sections of 
  the paper. Most of the paper content should be contained in these files.
- `ecology.bst`: This tells LaTeX how we want to format citations.
- `ref.bib`: This contains the reference information.


## Adding citations:

> Thanks to Daijiang for these!

1. Go to Google Scholar; click the top left, and select Settings; then in the
   Bibliography manager section, check show links to import citations into BibTeX, 
   then Save it. This step only need to be done once.
2. Back to the Google Scholar homepage and search the paper you want to cite 
  (e.g., "Generalized linear mixed models for phylogenetic analyses of community structure"). 
  Under the item, click the quotation marks, then click `BibTeX`.
  Then copy the whole new page (`Cmd + A` then `Cmd + C`).
  It should look something like this:

```
@article{Ives2011,
  title={Generalized linear mixed models for phylogenetic analyses of community structure},
  author={Ives, Anthony R and Helmus, Matthew R},
  journal={Ecological Monographs},
  volume={81},
  number={3},
  pages={511--525},
  year={2011},
  publisher={Wiley Online Library}
}
```

3. Open the `refs.bib` in this folder, and paste the citation information there.

4. To cite the paper in the manuscript, copy its key (e.g. `Ives2011` here),
   and the LaTeX cite command (`\citep{Ives2011}` here) to where you
   want to cite it. For multiple papers, use `\citep{key1,key2}`.
   To add prefixes or suffixes, use `\citep[e.g.,][, see?]{Ives2011}` to
   generate "(e.g., Ives & Helmus 2011, see?)".

