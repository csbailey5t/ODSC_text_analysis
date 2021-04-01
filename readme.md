# Exploratory Text Analysis in Python Using spaCy and textacy

Scott Bailey <br/>
Digital Research and Scholarship Librarian <br/>
Copyright and Digital Scholarship Center (CDSC) <br/>
NC State University Libraries

_Workshop for the Open Data Science Conference East 2021_

The Python ecosystem has many libraries for natural language processing (NLP), which can make it confusing to get started analyzing text as data. This workshop will introduce spaCy as a powerful, opinionated library for NLP that facilitates analysis of text data, along with textacy, a library that adds information retrieval and corpus analysis features.

By completing this workshop, you will develop core skills in asking questions of text and identifying interesting features through spaCy's tokenization, part-of-speech tagging, and named entity recognition. You will also learn to expand that analysis and scale it to many documents through textacy.

## Running the workshop code

All of the code in this workshop exists in Jupyter Notebooks (`.ipynb` files). The workshop code can be run in multiple ways.

If you already have a local Python installation and are comfortable working with virtual environments, you can clone this repository, create a virtual environment, and install the libraries listed in `requirements.txt` in your preferred way. This workshop was developed with Python 3.9 (by way of `pyenv`) with `virtualenv` and `pip` for simplicity, but you could use `conda`, `pipenv`, `poetry`, or other environment and package managers.

If you are just getting started with Python or simply prefer to work in the browser (I recommend this for the live workshop if you're at all unsure), use Colab through one of the links below and you'll be able to run all of the code in your browser without extra setup. You will need a Google account for Colab.

If you don't have a Google account or prefer not to use Google products, you can click on the Binder link below. Running the code with Binder will require an extra step when we work with a corpus in the workshop.

During the workshop, if you'd like to code along, you can open the `exploratory-clean.ipynb` notebook and write code there, where I've left the structure and some cells of code. If you'd prefer not to write code, but want to run it as we go, you can open the `exploratory-text-analysis.ipynb` file, and run each cell as the workshop progresses. This file will also serve as a reference for those coding along.

Clean Colab notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/csbailey5t/ODSC_text_analysis/blob/master/exploratory-clean.ipynb)

Filled in Colab notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/csbailey5t/ODSC_text_analysis/blob/master/exploratory-text-analysis.ipynb)

Binder (has both notebooks): [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/csbailey5t/ODSC_text_analysis/HEAD)

There are activities sprinkled throughout as ways to practice some techniques. Given time limits, we won't do activities during the workshop, but they are there as a way to practice after.

## Our Corpus: _State of the Union speeches_

Our corpus today will be the [State of the Union (1790-2018)](https://www.kaggle.com/rtatman/state-of-the-union-corpus-1989-2017) corpus released on Kaggle by Rachel Tatman. The corpus consists of the President of the United States' annual address from the designated years.

I've included the data, which is [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) licensed, in this repo for ease of use.
