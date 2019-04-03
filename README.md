# Cookiecutter Python

[Cookiecutter](https://github.com/audreyr/cookiecutter) template for Python packages.

* GitHub repo: https://github.com/tomtom-international/cookiecutter-python/
* Free software: Apache Software License 2.0

## Features

* Supports projects hosted in GitHub and BitBucket Server.
* Ready for [Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/) for GitHub projects and [Jenkins Declarative Pipelines](https://jenkins.io/doc/book/pipeline/syntax/#declarative-pipeline) for internally hosted projects in BitBucket Server.
* Testing setup with ``py.test`` only.
* Tox testing: Setup to easily test for Python (currently only for 3.6)
* Sphinx docs: Documentation ready for generation with, for example, ReadTheDocs
* Bumpversion: Pre-configured version bumping with a single command
* Auto-release to PyPI when PR gets merged into master via Azure Pipelines or Jenkins Pipelines.

## Quickstart

Install the latest Cookiecutter if you haven't installed it yet (this requires Cookiecutter 1.4.0 or higher):

```bash
pip install cookiecutter
```

Generate the Python package project:

```bash
cookiecutter gh:tomtom-international/cookiecutter-python
```

Then:

* Create a repo and push the generated project to master.
* Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``) and start coding.
* If you chose to use Azure for the CI contact the @nav-pipeline team to request a build pipeline in the [TomTom Azure DevOps account](https://dev.azure.com/tomtomweb/GitHub-TomTom-International/_build) (@nav-pipeline: detailed instructions on how to set up a project can be found [here](https://github.com/tomtom-international/azure-pipeline-templates/blob/master/README.md)).
* If you chose to use Jenkins it depends on your internal Jenkins setup.
  * For internal TomTom projects: Trigger **Scan Organization Folder Now** on the BitBucket Team Project folder. In case of problems contact the @nav-pipeline team.
* Contact the @nav-pipeline team to activate your project on `pyup.io`.

## Credits

This package is inspired by [Cookiecutter PyPackage](https://github.com/audreyr/cookiecutter-pypackage/) project template.
