# Getting Started with JupyterHub tutorial

Based on a tutorial at PyData London 2016
by Min Ragan-Kelly*, Thomas Kluyver, and Kyle Kelley.

Follow along with [the PDF](./JupyterHub.pdf)
or watch [the video on YouTube](https://www.youtube.com/watch?v=LkgSCjyv75s).

Clone this repo:

    git clone https://github.com/{{ insert repo here }} /srv/jupyterhub

You will need:

- conda with Python 3
- jupyterhub
- root access to a server or VM and/or docker

Quickest way to get jupyterhub is to run in this repo:

    conda env create -f environment.yml

The latter half of the tutorial will use [Docker](https://docs.docker.com).
