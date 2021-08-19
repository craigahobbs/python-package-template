# python-package-template

**python-package-template** is a Python package template for use with
[template-specialize](https://pypi.org/project/template-specialize/).

All generated projects have the following functionality:

- use [Python Build](https://github.com/craigahobbs/python-build#readme) for build and development experience

- contain setup.py ready to upload to [PyPI](https://pypi.org/)

- setup installs command-line script and [package main](https://docs.python.org/3/library/__main__.html) (optional)

- generates package documentation with [Sphinx](https://pypi.org/project/Sphinx/) (optional)

- publishes package documentation to [GitHub Pages](https://pages.github.com/) (optional)

- 100% unit-test code coverage ("make cover" fails if coverage is less than configurable minimum)


## Usage

To generate a new Python package project, clone this repository and render the template directory using template-specialize:

```
template-specialize python-package-template/template/ my-package/ \
    -k package "my-package" \
    -k name "John Doe" \
    -k email "johndoe@gmail.com" \
    -k github "johndoe"
```


## Template Variables

The following template variables are defined:

- **package** - the Python package name (e.g. "my-package")

- **name** - the package author's full name (e.g. "John Doe")

- **email** - the package author's email address

- **github** - the package author's GitHub account name (e.g. "johndoe")

- **nodoc** (optional) - if true, the package documentation is omitted

- **nomain** (optional) - if true, the command-line script and package main are omitted
