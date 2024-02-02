# CIViC Frontend Documentation

This repository houses the [documentation](https://civic.readthedocs.io/) for [CIViC](https://civicdb.org), a knowledgebase of clinical interpretations of variants in cancer. The documentation is compiled and hosted by the [ReadTheDocs](https://readthedocs.org/) service at [civic.readthedocs.io](https://civic.readthedocs.io/).

## Contributing

We welcome contributions to the documentation. If you wish to contribute a clarification, correction, or addition to the docs, please fork this repository, make your contribution, and submit a pull request.

## Getting Started

After you've forked and cloned the repository, install [Sphinx](https://www.sphinx-doc.org/en/master/), a [reStructuredText](http://docutils.sourceforge.net/rst.html) documentation generator, and [sphinx-autobuild](https://pypi.org/project/sphinx-autobuild/), a utility that will host and update the documentation as you work:

```
pip install sphinx sphinx-autobuild sphinx-fontawesome sphinxcontrib-images sphinx-rtd-theme
```

These docs also depend on a custom fork of the `sphinxcontrib-programoutput` extension. It can be installed by running:

```
pip install git+git://github.com/griffithlab/sphinxcontrib-programoutput.git#egg=sphinxcontrib-programoutput
```

If you get a timeout you can try changing "git+git..." to "git+https..."

Then start the sphinx-autobuild process:

```
cd ./civic-docs/docs
sphinx-autobuild ./ ./_build/html
```

Sphinx-autobuild will start a server at http://127.0.0.1:8000. View the compiled docs in your web browser at that URL, and edit the documentation to create your contribution. Sphinx-autobuild will recompile the docs when you save updates and reload the page in your browser.

Occasionally, especially after adding or moving a page or modifying the configuration, autobuild doesn't properly compile the new pages or changes. If this happens try these commands to delete cached files and rebuild the docs:

```
rm -rf ./_build/*
make html
```

Then restart sphinx-autobuild:

```
sphinx-autobuild ./ ./_build/html
```

## Updating the Docs with Pull Requests

If you'd like to contribute to the documentation or correct an error, clone the repository and create a new branch with your updates (if you do not have authorship permissions on the civic-docs repository, fork the repository first, before cloning, using the Fork button at the top right corner of the github interface):

```
git checkout -b doc-update
```

Make your updates, then push a new branch to the repository:

```
git push origin doc-update
```

Then visit the [civic-docs pull requests page](https://github.com/griffithlab/civic-docs/pulls). Github should display a message asking you if you'd like to create a pull request from the new branch you just pushed. Create the pull request with a short description of your contribution. A CIViC maintainer will evaluate your contribution and will likely merge it with the master branch, which will then be published. Thanks for your contributions!

## Setting up Sphinx to work in Docker

If you wind up in Python dependency hell getting Sphinx to work, you may want to try working in a Docker image by doing something like the following:

```
docker pull griffithlab/pvactools:latest
docker run -p 8000:8000 -v ~/git/civic/civic-docs/:/opt/git/civic/civic-docs/ -it griffithlab/pvactools:latest
pip install sphinx sphinx-autobuild sphinx-fontawesome sphinxcontrib-images
pip install git+https://github.com/griffithlab/sphinxcontrib-programoutput.git#egg=sphinxcontrib-programoutput
cd /opt/git/civic/civic-docs/docs
sphinx-autobuild --host 0.0.0.0 --port 8000 ./ ./_build/html
```

To view the updated docs site in your web browser go to: http://0.0.0.0:8000/. Once you are satisfied, submit a pull request as described above.
