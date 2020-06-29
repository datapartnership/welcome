# Welcome to the Development Data Partnership!

<p align="center">
  <img width="250" height="250" src="images/logo.png">
</p>


 > A partnership between international organizations and companies, created to facilitate the use of third-party data in research and international development.

As part of the Development Data Partnership, members have access to:

- Tools and snippets to get your data analysis up and running.
- A Python package that includes both partner-specific and general facilitators.
- A command-line toolbox that includes both partner-specific and general facilitators.

## Get Started

Probably you are looking where to start, so if:

- You have an [account](https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2Fjoin&source=header) on GitHub.
- You are a member of the Partnership's [organization](https://github.com/orgs/datapartnership/people) on GitHub. If not, [drop us a line](https://forms.office.com/Pages/ResponsePage.aspx?id=wP6iMWsmZ0y1bieW2PWcNhuvidJGUV9CkFxv6crNd1NUMjdRVVcyTzFJSjBWT0s4NDZCMDdKRlU2TC4u).

You're done! Go ahead explore the [documentation](#documentation) or [install](#installation) and [contribute](#contributing)!

## Resources

### [Awesome Development Data Partnership](https://datapartnership.github.io/awesome-ddp/)

> A curated list of the Development Data Partnership data goods and derivative works.

### Documentation

> Data documentation repositories curated for each Development Partner, based on their signed license agreements. 

Links to All Data Documentation:

| Development Partner | Documentation   | Package       | Repository    |
|:-------------------:|:---------------:|:-------------:|:-------------:|
| IDB                 | [Docs](https://devdatapartnership-idb.herokuapp.com/) | [v0.2](https://github.com/datapartnership/devdatapartnership-idb/releases/tag/v0.2) | [GitHub](https://github.com/datapartnership/devdatapartnership-idb) |
| IMF                 | [Docs](https://devdatapartnership-imf.herokuapp.com/) | [v0.2](https://github.com/datapartnership/devdatapartnership-imf/releases/tag/v0.2) | [GitHub](https://github.com/datapartnership/devdatapartnership-imf) |
| WBG                 | [Docs](https://docs.datapartnership.org) | [v0.2](https://github.com/datapartnership/devdatapartnership/releases/tag/v0.2) | [GitHub](https://github.com/datapartnership/devdatapartnership)

### Data Partners

| Data Partner       |       | WBG        | IDB        | IMF        |
|:------------------:|:-----:|:----------:|:----------:|:----------:|
| Carto              |       |:white_check_mark:|||
| ClimaCell          |       |:white_check_mark:|||
| Cuebiq             |       |:white_check_mark:|||
| ESA                |       |:white_check_mark:|||
| ESRI               |       |:white_check_mark:|:white_check_mark:|:white_check_mark:|
| Facebook           |       |:white_check_mark:|:white_check_mark:|:white_check_mark:|
| Google             |       |:white_check_mark:|||
| Grab               |       |:white_check_mark:|||
| GSMA               |       |:white_check_mark:|||
| Indigo             |       |:white_check_mark:|||
| InLoco             |       ||:white_check_mark:||
| LinkedIn           |       |:white_check_mark:|||
| Mapbox             |       |:white_check_mark:|||
| Mapillary          |       |:white_check_mark:|||
| Mobike             |       |:white_check_mark:|||
| Orbital Insight    |       |:white_check_mark:|||
| Premise            |       |:white_check_mark:|:white_check_mark:||
| SafeGraph          |       |:white_check_mark:||:white_check_mark:|
| Twitter            |       |:white_check_mark:|||
| Uber               |       |:white_check_mark:|||
| Unacast            |       |:white_check_mark:|:white_check_mark:|:white_check_mark:|
| Veraset            |       |:white_check_mark:|:white_check_mark:||
| Waze               |       |:white_check_mark:|||
| WhereIsMyTransport |       |:white_check_mark:|||
| X-Mode             |       |:white_check_mark:|||

## Installation

The Partnership maintains a Python package that offers partner-specific and general helper functions.

Before installing the package, you will have to:

1. Install **Python 3.6+**
1. Set up [GitHub with ssh](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh). Alternatively, see [username/password](#can-i-use-https-instead).

**Unfortunately, the package not public, so you will have to be authenticated via GitHub.**

Now you are ready to `pip install`! It is strongly recommended that you create a [virtual environment](https://docs.python-guide.org/dev/virtualenvs/).

### Development Data Partner

Now choose the organization you belong to. You will have visilibity to all data partners and documentation your organization have agreements with.

#### IDB 

If you are from the Inter-American Development Bank, install:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-idb.git@v0.2
```

#### IMF

If you are from the International Monetary Fund, install:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-imf.git@v0.2
```

#### WBG

If you are from the World Bank Group, install:

```
pip install git+ssh://git@github.com/datapartnership/devdatapartnership.git@v0.2
```

### Verifying 

Now you should have **datapartnership** installed on your environment.

```python
>> import datapartnership
>> datapartnership.__version__
0.2.0
```

See examples on the [documentation](#documentation).

### Can I use *https* instead?

We recommend `ssh`. Alternatively, you can change your global settings to use `https` instead.

That way, you will be able to login with your `username` and `password`. If you are using two-factor authentication on GitHUb, you will have to create a [personal token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line).

Now change your global settings,

```
git config --global url."https://github.com/".insteadOf "git@github.com:"
git config --global credential.helper cache
```

Finally, while installing, use `git+https://github.com/` instead of `git+ssh://git@github.com/`. For example,

```
pip install git+https://github.com/datapartnership/devdatapartnership.git
```

## Contributing

Our documentation follows the [literate programming](https://en.wikipedia.org/wiki/Literate_programming) paradigm.

> Literate programming is a programming paradigm introduced by Donald Knuth in which a computer program is given an explanation of its logic in a natural language, such as English, interspersed with snippets of macros and traditional source code, from which compilable source code can be generated. [Wikipedia](https://en.wikipedia.org/wiki/Literate_programming) 

It requires [nbdev](https://github.com/fastai/nbdev). Check [CONTRIBUTING](CONTRIBUTING.md).

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
