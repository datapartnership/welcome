
<p align="center">
  <img width="250" height="250" src="https://raw.githubusercontent.com/datapartnership/datapartnership.org/master/static/logo.png?token=AA65TKBV3GEVINUD5ABCHHK6Y7Y4M">
</p>

# Welcome to the Development Data Partnership!

 > A partnership between international organizations and companies, created to facilitate the use of third-party data in research and international development.


As part of the Development Data Partnership, you are going to have access to:

- common tools and code snippets to ease your data analysis
- curated list of exploratory notebooks for each data provider

## Get Started

Probably you are looking where to get started, so if:

- You have an [account](https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2Fjoin&source=header) on GitHub.
- You are a member of the Partnership's [organization](https://github.com/orgs/datapartnership/people) on GitHub. If not, drop us a line at datapartership@worldbank.org.

Go ahead, explore our documentation, [install](#install) or [clone](#cloning),

| Development Partner | Documentation   | Package       | Repository    |
|:-------------------:|:---------------:|:-------------:|:-------------:|
| IDB                 | [Docs](https://devdatapartnership-idb.herokuapp.com/) | [v0.1](#idb) | [GitHub](https://github.com/datapartnership/devdatapartnership-idb) |
| IMF                 | [Docs](https://devdatapartnership-imf.herokuapp.com/) | [v0.1](#imf) | [GitHub](https://github.com/datapartnership/devdatapartnership-imf) |
| WBG                 | [Docs](https://devdatapartnership.herokuapp.com/) | -- | [GitHub](https://github.com/datapartnership/devdatapartnership) |

and start contributing!

## Install

### IDB 

```sh
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-idb.git@v0.1#egg=ddp
```

### IMF 

```sh
pip install git+ssh://git@github.com/datapartnership/devdatapartnership-imf.git@v0.1#egg=ddp
```

### WBG 

```sh
pip install git+ssh://git@github.com/datapartnership/devdatapartnership.git#egg=ddp
```

###

## Contribute

Our documentation follows the [literate programming](https://en.wikipedia.org/wiki/Literate_programming) paradigm.

> Literate programming is a programming paradigm introduced by Donald Knuth in which a computer program is given an explanation of its logic in a natural language, such as English, interspersed with snippets of macros and traditional source code, from which compilable source code can be generated. [Wikipedia](https://en.wikipedia.org/wiki/Literate_programming) 

It requires [nbdev](https://github.com/fastai/nbdev).

### Cloning

- IDB 

    ```sh
    git clone --recurse-submodules git@git@github.com:datapartnership/devdatapartnership-idb.git
    ```

- IMF 

    ```sh
    git clone --recurse-submodules git@git@github.com:datapartnership/devdatapartnership-imf.git
    ```

- WBG

    ```sh
    git clone --recurse-submodules git@git@github.com:datapartnership/devdatapartnership.git
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
