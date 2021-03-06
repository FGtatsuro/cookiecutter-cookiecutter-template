{{ cookiecutter.template_project_name }}
==================================================
<!-- First 'cookiecutter-'(used in almost cases) is removed. -->
Cookiecutter template for {{ cookiecutter.template_project_name|replace('cookiecutter-', '', 1)|replace('-', ' ')|replace('_', ' ') }}.

[![Build Status](https://travis-ci.org/FGtatsuro/{{ cookiecutter.template_project_name }}.svg?branch=master)](https://travis-ci.org/FGtatsuro/{{ cookiecutter.template_project_name }})

Requirements
------------

Cookiecutter (>=1.4.x) (<https://github.com/audreyr/cookiecutter>)

How to
------

You can create new project of Cookiecutter template as follows.

```bash
$ cookiecutter gh:FGtatsuro/{{ cookiecutter.template_project_name }}
...
project_name [Name of generated project]: test-project
project_description [Description of generated project]: Test Project
year [2018]:
author [FGtatsuro]:
...
$ cd test-project
$ ls -1a
.
..
LICENSE
README.rst
```

You can overwrite default value of the field prompt asks with
~/.cookiecutterrc. It's better to overwrite 'author' field with your
Github username.

```bash
$ cat ~/.cookiecutterrc
default_context:
    author: "FGtatsuro"

$ cookiecutter gh:FGtatsuro/{{ cookiecutter.template_project_name }}
...
author [FGtatsuro]:
...
```
