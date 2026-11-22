# Axiomatch Labs

Research papers by Axiomatch Labs on order book data structures.

## Papers

| Paper | Date | PDF | Source |
|---|---|---|---|
| Sublinear market order sweep in order book implies a plane tree structure | 31 Aug 2026 | [PDF](papers/orderbook-plane-tree/orderbook-plane-tree.pdf) | [LaTeX](papers/orderbook-plane-tree/) |
| Resolution of staleness in order book with sublinear market order sweep | 4 Sep 2026 | [PDF](papers/resolution-of-staleness/resolution-of-staleness.pdf) | [LaTeX](papers/resolution-of-staleness/) |

### Sublinear market order sweep in order book implies a plane tree structure

An order book supports limit order placement and market order sweep. We show that if the sweep is sublinear and the operation count of a sweep is minimized, the order book will necessarily support a plane tree structure.

### Resolution of staleness in order book with sublinear market order sweep

Builds on the paper above. We propose a resolution of staleness algorithm for order books supporting sublinear market order sweep and prove its correctness. The algorithm needs $N+1$ storage, where $N$ is the number of price ticks, and we prove this is optimal by showing that $N$ storage cannot resolve staleness.

## Building from source

Each paper is a standard LaTeX project using `biblatex` with `biber`. With TeX Live installed:

```bash
cd papers/resolution-of-staleness
latexmk -pdf -jobname=resolution-of-staleness main.tex
```

## How to cite

```bibtex
@misc{axiomatch2026planetree,
  author = {{Axiomatch Labs}},
  title  = {Sublinear market order sweep in order book implies a plane tree structure},
  year   = {2026},
  month  = aug,
  url    = {https://github.com/axiomatch-labs/papers}
}

@misc{axiomatch2026staleness,
  author = {{Axiomatch Labs}},
  title  = {Resolution of staleness in order book with sublinear market order sweep},
  year   = {2026},
  month  = sep,
  url    = {https://github.com/axiomatch-labs/papers}
}
```

## License

The papers in this repository (text, figures, LaTeX sources and PDFs) are licensed under
[Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/).
You may share them unchanged, with attribution, for non-commercial purposes. See [LICENSE](LICENSE).

© 2026 Axiomatch Labs
