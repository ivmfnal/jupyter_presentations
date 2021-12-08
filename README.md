# jupyter_presentations
Templates and other pieces I used to make IPython/Jupyter - based presentations

## reveal1 template

This template is based to the ``reveal`` template with some modifications

To install it:

```sh
$ jupyter --paths
config:
    /Users/ivm/.jupyter
    /Users/ivm/.local/etc/jupyter
    /Users/ivm/miniconda3/etc/jupyter
    /usr/local/etc/jupyter
    /etc/jupyter
data:
    /Users/ivm/Library/Jupyter
    /Users/ivm/.local/share/jupyter
    /Users/ivm/miniconda3/share/jupyter
    /usr/local/share/jupyter
    /usr/share/jupyter
runtime:
    /Users/ivm/Library/Jupyter/runtime
```

Choose one of paths under ``data``, which you can write into, e.g. /Users/ivm/.local/share/jupyter

```sh
$ mkdir -p /Users/ivm/.local/share/jupyter/nbconvert/templates
$ cp -R reveal1 /Users/ivm/.local/share/jupyter/nbconvert/templates
```

Use the template:

```sh
$ jupyter nbconvert the_presentation.ipynb --to html --template reveal1
```