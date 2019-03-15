# CIViC Frontend Documentation

This repository houses the [documentation](https://civic.readthedocs.io/) for [CIViC](https://civicdb.org), a knowledgebase of clinical interpretations of variants in cancer. The documentation is compiled and hosted by the [ReadTheDocs](https://readthedocs.org/) service at [civic.readthedocs.io](https://civic.readthedocs.io/).

## Contributing

We welcome contributions to the documentation. If you wish to contribute a clarification, correction, or addition to the docs, please fork this repository, make your contribution, and submit a pull request.

## Getting Started

After you've forked and cloned the repository, install [https://www.sphinx-doc.org/en/master/](Sphinx), a [reStructuredText](http://docutils.sourceforge.net/rst.html) documentation generator, and [https://pypi.org/project/sphinx-autobuild/](sphinx-autobuild), a utility that will host and update the documentation as you work:

```
pip install sphinx sphinx-autobuild sphinx_rtd_theme 
```

Then start the sphinx-autobuild process:

```
cd ./civic-docs/docs
sphinx-autobuild ./ ./_build/html
```

Sphinx-autobuild will start a server at http://127.0.0.1:8000. View the compiled docs in your web browser at that URL, and edit the documentation to create your contribution. Sphinx-autobuild will recompile the docs when you save updates and reload the page in your browser.
