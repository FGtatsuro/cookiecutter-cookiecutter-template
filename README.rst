cookiecutter-cookiecutter-template
==================================

Cookiecutter template for Cookiecutter template.

Requirements
------------

Cookiecutter (>=1.3.0) (https://github.com/audreyr/cookiecutter)

How to
------

You can create new project of Cookiecutter template as follows.

.. code:: bash

    $ cookiecutter gh:FGtatsuro/cookiecutter-cookiecutter-template
    TODO:

You can overwrite default value of the field prompt asks with `~/.cookiecutterrc`.
It's better to overwrite 'author' field with your Github username.

.. code:: bash

    $ cat ~/.cookiecutterrc
    default_context:
        author: "FGtatsuro"
    
    $ cookiecutter gh:FGtatsuro/cookiecutter-cookiecutter-template
    ...
    author [FGtatsuro]: 
    ...
