# i2cns-19

[Introduction to Computer and Network Security](https://sites.google.com/view/intro2cns/home?authuser=0) 2019 workshop material.

Exercises are provided as [jupyter](https://jupyter-notebook.readthedocs.io/en/stable/index.html) notebooks. Those who wish to try out the code in their browser without installing anything on their machine may do so. Those who wish to run code on their own machine will find it easier to copy-and-paste it from notebooks than pdf files.

There are several cryptography libraries, with varying degrees of user-friendliness and capabilities - see for instance this [crypto API comparison](https://www.cl.cam.ac.uk/~rja14/shb17/fahl.pdf). We shall use [cryptography.io](https://cryptography.io/en/latest/hazmat/primitives/cryptographic-hashes/).

## jupyter

### Setup on a local linux machine

`apt install python3-pip python3-setuptools python3-venv`

`python3 -m pip install --upgrade pip`

setup a virtual env to install the package (recommended):

`python3 -m venv ./env`

`source ./env/bin/activate`

`python3 -m pip install wheel`

`python3 -m pip install jupyter`

To have the notebook recognize installed python packages, add the path to the packages to your PYTHONPATH os variable, e.g. add something like this to your ~/.profile

`PYTHONPATH="${PYTHONPATH}:/usr/lib/python3/dist-packages/"`

`export PYTHONPATH`

Then either force your current terminal to update with the new changes

`source ~/.profile`

or logout and back in.

### Starting the notebook

`./env/bin/jupyter notebook`

I recommend [jupyterthemes](https://github.com/dunovank/jupyter-themes)

`./env/bin/jupyter jt -t chesterish`
