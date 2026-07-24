# Central Kurdish Treebank (CKTB)

The **first constituency treebank for Central Kurdish (Sorani)** — a manually annotated
corpus with part-of-speech tagging and phrase-structure (constituency) bracketing,
developed to support syntactic parsing and NLP research for a low-resource language.

## Overview

| Attribute | Value |
|---|---|
| Language | Central Kurdish (Sorani), Arabic script |
| Sentences | 3,000 |
| Words | 18,230 |
| POS tagset | 74 fine-grained tags (custom, designed for Central Kurdish morphology) |
| Grammar | 249-rule Context-Free Grammar (CFG) |
| Annotation | Two-pass manual POS annotation; parser-assisted, expert-validated constituency bracketing |
| Genres | Academic, news (politics, sport, economy), literature, culture, health, history |
| Empty categories | Pro-drop subjects annotated as empty nodes |

## Repository contents

```
data/        treebank sentences with gold constituency trees + train/val/test splits
guidelines/  annotation guideline (POS tagset and bracketing conventions)
eval/        EVALB parameter file used for all parsing evaluation in the paper
```

> **Data release status:** the treebank file will be added here after final
> validation checks are completed. Watch/star the repository for updates.

## Evaluation

All parsing results in the accompanying paper were computed with
[EVALB](https://nlp.cs.nyu.edu/evalb/) using the parameter file in
[`eval/kurdish.prm`](eval/kurdish.prm) (punctuation labels and empty categories
excluded from bracket scoring, following Penn Treebank conventions).

## Citation

If you use this treebank, please cite:

```bibtex
@article{ahmad_cktb,
  title   = {Designing and Collecting a Corpus and Syntactic Parser for Central Kurdish Language},
  author  = {Ahmad, Omed Sedeeq and Veisi, Hadi and Daneshfar, Fatemeh},
  note    = {Under review},
  year    = {2026}
}
```

## License

This dataset is released under the
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
license — you may use, share, and adapt it for any purpose, provided you give
appropriate credit.

## Contact

- Omed Sedeeq Ahmad — Soran University — omed.ahmed@soran.edu.iq
