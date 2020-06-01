
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

You're done! Go ahead explore the documentation, [install](#installation), and [contribute](#contributing)!

## Resources

### [Awesome Development Data Partnership](https://datapartnership.github.io/awesome-ddp/)

> A curated list of the Development Data Partnership data goods and derivative works.

### Documentation

| Development Partner | Documentation   | Package       | Repository    |
|:-------------------:|:---------------:|:-------------:|:-------------:|
| IDB                 | [Docs](https://devdatapartnership-idb.herokuapp.com/) | [v0.1](https://github.com/datapartnership/devdatapartnership-idb/releases/tag/v0.1) | [GitHub](https://github.com/datapartnership/devdatapartnership-idb) |
| IMF                 | [Docs](https://devdatapartnership-imf.herokuapp.com/) | [v0.1](https://github.com/datapartnership/devdatapartnership-imf/releases/tag/v0.1) | [GitHub](https://github.com/datapartnership/devdatapartnership-imf) |
| WBG                 | [Docs](https://devdatapartnership.herokuapp.com/) | -- | [GitHub](https://github.com/datapartnership/devdatapartnership)

## Installation

The Partnership maintains a Python package that offers partner-specific and general helper functions.

Before installing the package, you will have to:

1. Install **Python 3.6+**
1. Set up [GitHub with ssh](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh). Alternatively, see [https](#Can-I-Use-HTTPS-Instead?).

Now you are ready to `pip install`! It is strongly recommended that you create a [virtual environment](https://docs.python-guide.org/dev/virtualenvs/).

### IDB 

If you are from Inter-American Development Bank, install running:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-idb.git
```

### IMF

If you are from International Monetary Fund, running using:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-imf.git
```

### WBG

If you are from the World Bank Group, running using:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership.git
```

### Can I use HTTPS instead?

We recommend `ssh`. Alternatively, you can change your global settings to use `https` instead.

```
git config --global url."https://github.com/".insteadOf "git@github.com:"
git config --global credential.helper cache
```

Use `git+https://github.com/` instead of `git+ssh://git@github.com/`. For example,

```
pip install git+https://github.com/datapartnership/devdatapartnership.git
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
