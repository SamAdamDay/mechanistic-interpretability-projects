Mechanistic Interpretability Projects
=====================================

This repository houses research projects in mechanistic interpretability: [reverse engineering neural networks](https://transformer-circuits.pub/2022/mech-interp-essay/index.html).


## [Understanding bracket closing in GPT-Neo](/bracket-closing.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SamAdamDay/mechanistic-interpretability-projects/blob/main/bracket-closing.ipynb)

The goal of this notebook is to explore the phenomenon of bracket closing in the [GPT-Neo 125M model](https://www.eleuther.ai/artifacts/gpt-neo), whereby it can correctly match open parentheses `([{<` with their corresponding closing versions `)]}>`.

This is [Problem 2.13](https://www.alignmentforum.org/s/yivyHaCAmMJ3CqSyj/p/XNjRwEX9kxbpzWFWd#block71) in Neel Nanda's [200 Concrete Open Problems in Mechanistic Interpretability](https://www.alignmentforum.org/posts/LbrPTJ4fmABEdEnLf/200-concrete-open-problems-in-mechanistic-interpretability). The first goal is to figure out how the model determines whether an opening or closing bracket is more appropriate, and the second is to figure out how it knows the correct kind: `(`, `[`, `{` or `<`.


## [Playground](/playground/)

Some notebooks messing around with models.
- [Reducing transformer embedding dimensionality](/playground/token-embed-dim.ipynb)
- [Regressing on transformer embeddings](/playground/token-embed-regression.ipynb)
- [Doing SVD on positional embeddings](/playground/pos-embed-svd.ipynb)