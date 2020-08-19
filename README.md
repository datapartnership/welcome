# Welcome to the Development Data Partnership!

<p align="center">
  <img width="250" height="250" src="https://raw.githubusercontent.com/datapartnership/welcome/master/images/logo.png">
</p>

 > A partnership between international organizations and companies, created to facilitate the use of third-party data in research and international development.

## Get Started

Probably you are looking where to start, so if:

- You have an [account](https://github.com/join?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2Fjoin&source=header) on GitHub.
- You are a member of the Partnership's [organization](https://github.com/orgs/datapartnership/people) on GitHub. If not, [drop us a line](https://forms.office.com/Pages/ResponsePage.aspx?id=wP6iMWsmZ0y1bieW2PWcNhuvidJGUV9CkFxv6crNd1NUMjdRVVcyTzFJSjBWT0s4NDZCMDdKRlU2TC4u).

You're done! Go ahead explore the [documentation](#documentation) or [install](#installation) and [contribute](#contributing)!

## Resources

### [Awesome Data Partnership](https://datapartnership.github.io/awesome-ddp/)

> A curated list of the Development Data Partnership public data goods and derivative works.

### Documentation

> Data documentation repositories curated for each Development Partner, based on their signed license agreements.

Links to each Data Partner's Documentation:

> **Important: The documentation may **NOT** be shared with persons outside of your organization.**

| Data Partner       | Repository   | WBG        | IDB        | IMF        |
|:------------------:|:------------:|:----------:|:----------:|:----------:|
| Carto              | [Examples](https://github.com/datapartnership/ddp-docs-carto)      |✅|||
| ClimaCell          | [Examples](https://github.com/datapartnership/ddp-docs-climacell)      |✅|||
| Cuebiq             | [Examples](https://github.com/datapartnership/ddp-docs-cuebiq)      |✅|||
| ESA                | [Examples](https://github.com/datapartnership/ddp-docs-esa)      |✅|||
| ESRI               | [Examples](https://github.com/datapartnership/ddp-docs-esri)      |✅|✅|✅|
| Facebook           | [Examples](https://github.com/datapartnership/ddp-docs-facebook)      |✅|✅|✅|
| Google             | [Examples](https://github.com/datapartnership/ddp-docs-google)      |✅|||
| Grab               | [Examples](https://github.com/datapartnership/ddp-docs-grab)      |✅|||
| GSMA               | [Examples](https://github.com/datapartnership/ddp-docs-gsma)      |✅|||
| Indigo             | [Examples](https://github.com/datapartnership/ddp-docs-indigo)      |✅|||
| InLoco             | Examples      ||✅||
| LinkedIn           | [Examples](https://github.com/datapartnership/ddp-docs-linkedin)      |✅|||
| Mapbox             | [Examples](https://github.com/datapartnership/ddp-docs-mapbox)      |✅|||
| Mapillary          | [Examples](https://github.com/datapartnership/ddp-docs-mapillary)      |✅|||
| Mobike             | [Examples](https://github.com/datapartnership/ddp-docs-mobike)      |✅|||
| Orbital Insight    | [Examples](https://github.com/datapartnership/ddp-docs-orbitalinsight)      |✅|||
| Premise            | [Examples](https://github.com/datapartnership/ddp-docs-premise)      |✅|✅|✅|
| SafeGraph          | [Examples](https://github.com/datapartnership/ddp-docs-safegraph)      |✅||✅|
| Twitter            | [Examples](https://github.com/datapartnership/ddp-docs-twitter)      |✅|||
| Uber               | [Examples](https://github.com/datapartnership/ddp-docs-uber)      |✅|||
| Unacast            | [Examples](https://github.com/datapartnership/ddp-docs-unacast)      |✅|✅|✅|
| Veraset            | [Examples](https://github.com/datapartnership/ddp-docs-veraset)      |✅|✅||
| Waze               | [Examples](https://github.com/datapartnership/ddp-docs-waze)      |✅|||
| WhereIsMyTransport | [Examples](https://github.com/datapartnership/ddp-docs-whereismytransport)      |✅|||
| X-Mode             | [Examples](https://github.com/datapartnership/ddp-docs-xmode)      |✅|||

## Installation

The Partnership maintains a Python package that offers partner-specific and general helper functions.

Before installing the package, you will have to:

1. Install **Python 3.6+**
1. Set up [GitHub with ssh](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh). Alternatively, see [username/password](#can-i-use-https-instead).

**Unfortunately, the package not public, so you will have to be authenticated via GitHub.**

Now you are ready to `pip install`! It is strongly recommended that you create a [virtual environment](https://docs.python-guide.org/dev/virtualenvs/).

```
pip install git+ssh://git@github.com/datapartnership/datapartnership.git@v0.2
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
pip install git+https://github.com/datapartnership/datapartnership.git
```

## Contributing

Our documentation follows the [literate programming](https://en.wikipedia.org/wiki/Literate_programming) paradigm.

> Literate programming is a programming paradigm introduced by Donald Knuth in which a computer program is given an explanation of its logic in a natural language, such as English, interspersed with snippets of macros and traditional source code, from which compilable source code can be generated. [Wikipedia](https://en.wikipedia.org/wiki/Literate_programming) 

It requires [nbdev](https://github.com/fastai/nbdev). Check [CONTRIBUTING](CONTRIBUTING.md).