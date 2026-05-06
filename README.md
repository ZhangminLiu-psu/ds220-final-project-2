# Who Gets to Speak on Screen? — DS 220 Project II

A 44-year analysis of women's representation in Hollywood films, using the Bechdel Test as the lens.

**Live site:** https://YOUR-GITHUB-USERNAME.github.io/REPO-NAME/

## What's in this repo

| File | What it is |
|---|---|
| [`index.html`](index.html) | The rendered analysis (this is what GitHub Pages serves). |
| [`analysis.ipynb`](analysis.ipynb) | The Jupyter notebook source. Open it in Codespaces, Colab, or local Jupyter. |
| [`data/movies.csv`](data/movies.csv) | 1,794 films from 1970–2013 with Bechdel result, budget, gross. From FiveThirtyEight. |
| [`data/SOURCE_README.md`](data/SOURCE_README.md) | The original FiveThirtyEight description of the dataset. |
| [`build_notebook.py`](build_notebook.py) | Programmatic notebook builder — re-run to regenerate `analysis.ipynb` from scratch. |

## How the analysis is structured

Following the DS 220 Project II rubric, the notebook is organized into:

1. **Problem space** — what, why, who, where, when.
2. **Eight questions** to address with data.
3. **Dataset description** and connection to the problem.
4. **Setup** and data loading into a pandas DataFrame.
5. **Exploratory data analysis** (sample sizes, distributions, financial summaries).
6. **Eight separate analyses**, each visualized and explained.
7. **Insights** that synthesize the answers and call out limitations.

## Running it locally

```bash
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME
pip install -r requirements.txt   # or: pip install pandas matplotlib seaborn jupyter
jupyter notebook analysis.ipynb
```

To regenerate `index.html` after editing the notebook:

```bash
jupyter nbconvert --to html analysis.ipynb --output index.html --template lab
```

## Acknowledgments

- **Data:** [FiveThirtyEight Bechdel Test dataset](https://github.com/fivethirtyeight/data/tree/master/bechdel), originally from [bechdeltest.com](https://bechdeltest.com/) and [The Numbers](https://www.the-numbers.com/).
- **Inspiration:** Walt Hickey's 2014 FiveThirtyEight article *"The Dollar-and-Cents Case Against Hollywood's Exclusion of Women."*
