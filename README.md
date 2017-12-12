# IronYeasts

[![Build Status](https://travis-ci.org/thomasdenecker/IronYeasts.svg?branch=master)](https://travis-ci.org/thomasdenecker/IronYeasts)
[![Coverage Status](https://coveralls.io/repos/github/thomasdenecker/IronYeasts/badge.svg?branch=master)](https://coveralls.io/github/thomasdenecker/IronYeasts?branch=master)

**IronYeasts** is a project that aims to find the genes involved in iron homeostasis in pathogenic yeasts. This project is divided into 2 main parts :
- tools developed in python :
  - [GRYCotation](./GRYCotation) : tool to get GRYC annotation of Yeast
  - [MESH_link](./MESH_link) : tool to find link between MESH terms
  - [GO_DEF](./GO_DEF) : tool to get the last GO definition for each GO term.
- tools developed in R :
  - Ytools : a package with various functions to assist in the analysis of multi-omics yeast data
  - Main code : the code that performs the analysis using Ytools


## Requirements

### Python part

We use Pipenv to develop and run Python programs in IronYeast. We invite you to ensure you have
installed the following requirements before trying to use different programs:

* [pipenv](https://github.com/kennethreitz/pipenv)

This project use `flake8` to ensure coding style consistency (PEP8). To test python codes locally,
you must install the following modules:

* [flake8](http://flake8.pycqa.org/en/latest/)
* [Pylint](https://www.pylint.org/#install)
* [Biopython](http://biopython.org/)

The command lines to install them are :

```bash
python3 -m pip install flake8
python3 -m pip install pylint
python3 -m pip install biopython
```

## Quick start

Have you read the "Requirements" section above?

```bash
# Clone the project
$ git clone https://github.com/thomasdenecker/IronYeasts.git
$ cd IronYeasts
```
Then, we invite you to read the different READMEs proposed for each program.

## Continuous integration
> Continuous Integration (CI) is the process of automating the build and testing of code at each commit changes.

In this project, we use [Travis CI](https://travis-ci.org). A documentation is available [here](./docs/TRAVIS_CI.md).

### Python part
#### 1) Lint the code
> `flake8` and `lint` are tools to ensure coding style consistency (PEP8).

To run locally them with python codes

```bash
$ flake8 CODE_NAME.py
$ pylint CODE_NAME.py
```
#### 2) Test code
> The pytest framework makes it easy to write small tests, yet scales to support complex functional testing for applications and libraries.

In coming

#### 3) Coveralls
> Coveralls is a web service to help you track your code coverage over time, and ensure that all your new code is fully covered.

A documentation is available [here](./docs/coveralls.md)

In coming


## Contributing

Please, see the [CONTRIBUTING](CONTRIBUTING.md) file.

## Contributor Code of Conduct

Please note that this project is released with a [Contributor Code of
Conduct](http://contributor-covenant.org/). By participating in this project you
agree to abide by its terms. See [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) file.

## License

Pixel is released under the BSD-3 License. See the bundled [LICENSE](LICENSE)
file for details.
