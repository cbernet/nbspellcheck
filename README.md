# npspellcheck : 

**spell checking jupyter notebooks**

Writing correctly should be a priority, even for programmers and scientists. 

But this is not easy in jupyter notebooks. 

In english, a good solution is to make use of the spellchecker notebook extension, which highlights incorrect text: 

```
pip install jupyter_contrib_nbextensions
jupyter contrib nbextension install --user
jupyter nbextension enable spellchecker/main
```

However, this extension is currently not able to suggest corrections, and is only available for English. 

Since I write blog posts based on jupyter notebooks in French, I came up with a small script for spell checking. 

Example of use:

```
nbspellcheck.py my_jupyter_notebook.ipynb -l fr
```

## Installation

This script requires:

* python 3
* [nltk](http://www.nltk.org/)
* [pyspellchecker](https://pypi.org/project/pyspellchecker/)
* termcolor

All of that can be installed easily with Anaconda and pip.

Maybe I'll make a pip package when I have some time.

## Thanks & disclaimer

A big thank you to all people behind:

* [nltk](http://www.nltk.org/)
* [pyspellchecker](https://pypi.org/project/pyspellchecker/)

I made this real fast, and the script is not perfect yet. Please don't hesitate to send a PR. 

