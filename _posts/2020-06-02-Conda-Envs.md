---
layout: post
title: "Working with Conda Envs"
categories: conda
---
* TOC
{:toc}

## activating an environment

`conda activate name`

## Creating an Env file
[docs](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)

`conda env create -f environment.yml`

example of an environment file

```
name: stats2
channels:
  - javascript
dependencies:
  - python=3.6   # or 2.7
  - bokeh=0.9.2
  - numpy=1.9.*
  - nodejs=0.10.*
  - flask
  - pip:
    - Flask-Testing
```
