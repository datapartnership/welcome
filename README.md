
<p align="center">
  <img width="250" height="250" src="images/logo.png">
</p>

# Welcome to the Development Data Partnership!

 > A partnership between international organizations and companies, created to facilitate the use of third-party data in research and international development.

As part of the Development Data Partnership, you are going to have access to:

- code snippets and general tools to get your data analysis up and running
- a curated list of code examples and data explorations for each data provider
- a Python package that includes both partner-specific and general helper functions

## Get Started

Probably you are looking where to start, so if:

- You have an [account](https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2Fjoin&source=header) on GitHub.
- You are a member of the Partnership's [organization](https://github.com/orgs/datapartnership/people) on GitHub. If not, [drop us a line](mailto:datapartnership@worldbank.org).

You're done! Explore our documentation, [install](#installation) or [contribute](#contributing),

| Development Partner | Documentation   | Package       | Repository    |
|:-------------------:|:---------------:|:-------------:|:-------------:|
| IDB                 | [Docs](https://devdatapartnership-idb.herokuapp.com/) | [v0.1](#idb) | [GitHub](https://github.com/datapartnership/devdatapartnership-idb) |
| IMF                 | [Docs](https://devdatapartnership-imf.herokuapp.com/) | [v0.1](#imf) | [GitHub](https://github.com/datapartnership/devdatapartnership-imf) |
| WBG                 | [Docs](https://devdatapartnership.herokuapp.com/) | -- | [GitHub](https://github.com/datapartnership/devdatapartnership) 

## [Awesome Development Data Partnership](https://datapartnership.github.io/awesome-ddp/)

> A curated list of the Development Data Partnership data goods and derivative works.

## Installation

The Partnership maintains a Python package that offers partner-specific and general helper functions.

### Pre-installation

Before installing the package, you will have to:

- be a member of the [Partnership's team](https://github.com/orgs/datapartnership/people)
- set up [GitHub with ssh](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)

**HTTPS**

We recommend `ssh`. Alternatively, you can change your global settings to use `https` instead.

```
git config --global url."https://github.com/".insteadOf "git@github.com:"
git config --global credential.helper cache
```

Now you are ready to `pip install`! Make sure that you are running **Python 3.6+** and it strongly recommendeded that you create a [virtual environment](https://docs.python-guide.org/dev/virtualenvs/).

Check for the [latest stable version](https://github.com/datapartnership/welcome#get-started). Alternatively, you can install the latest version.

### IDB 

If you are from IDB, choose a version, e.g. `export VERSION=v0.1`, and install using:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-idb.git@${VERSION}#egg=ddp
```

or, install the latest version,

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-idb.git#egg=ddp
```

### IMF

If you are from IMF, choose a version, e.g. `export VERSION=v0.1`, and install using:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-imf.git@${VERSION}#egg=ddp
```

or, install the latest version,

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-imf.git#egg=ddp
```

### WBG

If you are from WBG, choose a version, e.g. `export VERSION=v0.1`, and install using:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership.git@${VERSION}#egg=ddp
```

or, install the latest version,

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership.git#egg=ddp
```

## Contributing

Our documentation follows the [literate programming](https://en.wikipedia.org/wiki/Literate_programming) paradigm.

> Literate programming is a programming paradigm introduced by Donald Knuth in which a computer program is given an explanation of its logic in a natural language, such as English, interspersed with snippets of macros and traditional source code, from which compilable source code can be generated. [Wikipedia](https://en.wikipedia.org/wiki/Literate_programming) 

It requires [nbdev](https://github.com/fastai/nbdev).

### Cloning

- IDB 

    ```sh
    git clone --recurse-submodules git@github.com:datapartnership/devdatapartnership-idb.git
    ```

- IMF 

    ```sh
    git clone --recurse-submodules git@github.com:datapartnership/devdatapartnership-imf.git
    ```

- WBG

    ```sh
    git clone --recurse-submodules git@github.com:datapartnership/devdatapartnership.git
    ```

### Pulling

```sh
git pull --recurse-submodules
```

### Pushing

As a member of the Development Data Partnership, you will be able to share and contribute to a common code base. 

For that we use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). Basically, each data partner has a home of its own

```sh
.
└── notebooks
    ├── core
    └── facebook
```

You can contribute as you would normally do by going to any subfolder/submodule,

```sh
# contribute to facebook
cd notebooks/facebook

# create your feature branch
git checkout -b <my-awesome-branch>
```

Make your contributions, adding and commiting and whenever you are ready,

```sh
# push your contributions
git push
```

As a final step, open a pull request on corresponding data partner repository (e.g., [Facebook](https://github.com/datapartnership/ddp-docs-facebook/pulls)).
