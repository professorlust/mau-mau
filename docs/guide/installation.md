# Installation

## Which Python version should I use?

> Short version: Python 2.x is legacy, Python 3.x is the present and future of the language and [3.6 is the new hotness](https://www.python.org/downloads/release/python-361/) and I won't do it below that.

-- [Should I use Python 2 or Python 3 for my development activity?](https://wiki.python.org/moin/Python2orPython3)

... nuff said.

### To be more exact: **Python 3.6**

There are a lot of great additions in [Python 3.6](https://www.python.org/downloads/release/python-361/) - most of them backwards compatible, but I will use at least one backwards incompatible feature in this project: [f-strings](https://www.python.org/dev/peps/pep-0498/) - because I can :D

!!! note
    It might already be installed. Type `python` on the commandline and see if a Python [REPL](https://docs.python.org/3/tutorial/interpreter.html) opens and which version it reports. If the standard python interpreter is still Python2 on your system, try typing `python3` instead and see if you are lucky. If not get it here: [Python3](https://www.python.org/downloads/).

## [In a virtualenv]

!!! note
    The installation of this package in a virtualenv is is not necessary but recommended. It is worth learning to work with virtualenvs as early as possible anyway.

You should really install this in a [virtualenv](https://docs.python.org/3/library/venv.html). This should work out of the box. If not, you might be on Linux and are bitten by [this](https://bugs.launchpad.net/ubuntu/+source/python3.4/+bug/1290847). `sudo apt-get install python3-pip` should solve the problem - otherwise have a look at the [pip documentation](https://pip.pypa.io/en/stable/installing/).

    $ python3.6 -m venv mau-mau-env

Activation of virtualenvs is sadly still one of the things that is not os independent, so you will have to look [here](https://docs.python.org/3/library/venv.html#creating-virtual-environments) how to do that in your os. The most common cases are:

    $ source mau-mau-env/bin/activate  # most linux shells
    $ mau-mau-env\Scripts\activate.bat  # Windows cmd.exe

Deactivate with:

    $ deactivate

## ... from Github

Install the latest code directly from github by typing on the command line:

    $ pip install "git+https://github.com/obestwalter/mau-mau.git#egg=mau-mau"

To install a specific version just replace `master` with the version you want to install (e.g. `1.1.0`). The different versions can be seen in the [release section](https://github.com/obestwalter/mau-mau/releases) of a Github project.

## ... from .zip file

On the [releases page](https://github.com/obestwalter/mau-mau/releases/) you can download zip archives and install them by typing on the command line:

    $ pip install </path/to/downloaded/zip/archive>

## ... from [PyPI](https://pypi.python.org/pypi)

!!! warning "This is not implemented"
    This would mean uploading the package to the official Python Package Index (PyPI -- formerly known as the cheese shop -- documented [here](https://docs.python.org/3/distutils/packageindex.html)) ... it's not hard to do but not necessary for a learning tool like this, so I just mention it here, because that is the official way for "real" software.

If `mau-mau` would be uploaded to PyPI, it could be installed by simply typing:

    $ pip install mau-mau
