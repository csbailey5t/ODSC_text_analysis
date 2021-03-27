# Exploratory Text Analysis in Python Using spaCy and textacy

Scott Bailey <br/>
Digital Research and Scholarship Librarian <br/>
Copyright and Digital Scholarship Center (CDSC) <br/>
NC State University Libraries

_Workshop for the Open Data Science Conference East 2021_

The Python ecosystem has many libraries for natural language processing (NLP), which can make it confusing to get started analyzing text as data. This workshop will introduce spaCy as a powerful, opinionated library for NLP that facilitates analysis of text data, along with textacy, a library that adds information retrieval and corpus analysis features.

By completing this workshop, you will develop core skills in asking questions of text and identifying interesting features through spaCy's tokenization, part-of-speech tagging, and named entity recognition. You will also learn to expand that analysis and scale it to many documents through textacy.

## Running the workshop code

All of the code in this workshop exists in a Jupyter Notebooks (`.ipynb` files). The workshop code can be run in multiple ways.

If you already have a local Python installation and are comfortable working with virtual environments, go ahead and create a virtual environment and install the libraries listed in `requirements.txt` in your preferred way. This workshop was developed with Python 3.9 (by way of `pyenv`) with `virtualenv` and `pip` for simplicity, but you could use `conda`, `pipenv`, `poetry`, or other environment and package managers.

If you are just getting started with Python or simply prefer to work in the browser (I recommend this for the live workshop), click on the Google Colab button below to open the workshop notebook in Google Colab, Google's hosted Jupyter Notebook environment. You'll be able to run all of the code in your browser.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/csbailey5t/ODSC_text_analysis/blob/master/exploratory-text-analysis.ipynb)

You can also run the full notebook in Binder. To run in Binder, click the button below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/csbailey5t/ODSC_text_analysis/master)

## Our Corpus: _State of the Union speeches_

Our corpus today will be the [State of the Union (1790-2018)](https://www.kaggle.com/rtatman/state-of-the-union-corpus-1989-2017) corpus released on Kaggle by Rachel Tatman. The corpus consists of the President of the United States' annual address from the designated years.