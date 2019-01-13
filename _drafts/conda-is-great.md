---
layout: post
title: "Conda is great"
date: YYYY-MM-DD
tags: conda python depenencies dev-ops c++
---

# Overwhelmed by all your python dependencies? Conda to the rescue!

## Why Conda?

The *classical* way (at least on Linux or MAC, I don't know what Windows is) to manage python dependencies
is to use `pip` as package manager and `virualenv` for enviroments. But this approach has some short-comings,
most importantly pip is restricted to python dependencies.

Fortunately conda

## How to use it

### Install conda

Conda comes in two flavors: there is [miniconda](), which provides the conda dev-kit and [anaconda]() that in addition provides a full python distribution.
For development purposes, you should go with `miniconda`. You can install all python packages of ``anaconda` on demand anyways.
To install it, ... 

### Create and manage environments

```bash
$ conda create -n my-env scikit-image scikit-learn pandas matplotlib
$ conda activate my-env
```

`environment.yaml`

```yaml
name: myenv
dependencies:
- scikit-image
- scikit-learn
- pandas
- matplotlib
```

```bash
$ conda env create -f environment.yaml
```

### Install packages

```bash
$ conda install h5py=2.7.0
```

### Anaconda Cloud & Channels

### Recipes & Conda Forge
