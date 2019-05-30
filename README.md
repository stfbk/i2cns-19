# i2cns-19

I2C&amp;NS 2019 workshop material

[Course website](https://sites.google.com/view/intro2cns/home?authuser=0)

## jupyter

### Setup on a local linux machine

apt install python3-pip python3-setuptools python3-venv

python3 -m pip install --upgrade pip

. setup a virtual env to install the package (recommended):

python3 -m venv ./env
source ./env/bin/activate
python3 -m pip install wheel
python3 -m pip install jupyter

To have the notebook recognize installed python packages, add the path to the packages to your PYTHONPATH os variable, e.g. add something like this to your ~/.profile

PYTHONPATH="${PYTHONPATH}:/usr/lib/python3/dist-packages/"
export PYTHONPATH

then source ~/.profile


### Starting the notebook

./env/bin/jupyter notebook


### Links

[jupyter documentation](https://jupyter-notebook.readthedocs.io/en/stable/index.html)

[markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
