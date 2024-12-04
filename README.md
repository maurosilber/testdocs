# testdocs

[![Copier Badge][copier-badge]][copier-url]
[![Pixi Badge][pixi-badge]][pixi-url]
![License][license-badge]
[![CI Badge][ci-badge]][ci-url]
[![conda-forge Badge][conda-forge-badge]][conda-forge-url]
[![PyPI Badge][pypi-badge]][pypi-url]
[![Python version Badge][pypi-version-badge]][pypi-version-url]

testing mkdocs

## Install

Using [pixi](pixi-url),
install from PyPI with:

```sh
pixi add --pypi testdocs
```

or install the latest development version from GitHub with:

```sh
pixi add --pypi testdocs@https://github.com/maurosilber/testdocs.git
```

Otherwise,
use `pip` or your `pip`-compatible package manager:

```sh
pip install testdocs  # from PyPI
pip install git+https://github.com/maurosilber/testdocs.git  # from GitHub
```

## Development

This project is managed by [pixi](https://pixi.sh).
You can install it for development using:

```sh
git clone https://github.com/maurosilber/testdocs
cd testdocs
pixi run pre-commit-install
```

Pre-commit hooks are used to lint and format the project.

### Testing

Run tests using:

```sh
pixi run test
```

### Publishing to PyPI

When a tagged commit is pushed to GitHub,
the GitHub Action defined in `.github/workflows/ci.yml`
builds and publishes the package to PyPI.

Tag a commit and push the tags with:

```sh
git tag <my-tag>
git push --tags
```

Trusted publishing must be enabled once in [PyPI Publishing](https://pypi.org/manage/account/publishing/).
Fill the following values in the form:

```
PyPI Project Name: testdocs
            Owner: maurosilber
  Repository name: testdocs
    Workflow name: ci.yml
 Environment name: pypi
```

[ci-badge]: https://img.shields.io/github/actions/workflow/status/maurosilber/testdocs/ci.yml
[ci-url]: https://github.com/maurosilber/testdocs/actions/workflows/ci.yml
[conda-forge-badge]: https://img.shields.io/conda/vn/conda-forge/testdocs?logoColor=white&logo=conda-forge
[conda-forge-url]: https://prefix.dev/channels/conda-forge/packages/testdocs
[copier-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/copier-org/copier/master/img/badge/badge-black.json
[copier-url]: https://github.com/copier-org/copier
[license-badge]: https://img.shields.io/badge/license-MIT-blue
[pixi-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json
[pixi-url]: https://pixi.sh
[pypi-badge]: https://img.shields.io/pypi/v/testdocs.svg?logo=pypi&logoColor=white
[pypi-url]: https://pypi.org/project/testdocs
[pypi-version-badge]: https://img.shields.io/pypi/pyversions/testdocs?logoColor=white&logo=python
[pypi-version-url]: https://pypi.org/project/testdocs
