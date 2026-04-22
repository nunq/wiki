# python

## creating a venv for a python version you dont have locally

i.e. for python 3.13

```sh
uv python pin python3.13
uv run python --version
# create the venv using uv's temp python version
uv run python -m venv .venv
source .venv-linux/bin/activate.fish
python --version
# > Python 3.13.11
pip install -r requirements.txt
```

## misc

links:
* https://www.b-list.org/weblog/2022/dec/19/boring-python-code-quality/
* https://gist.github.com/RobertAKARobin/a1cba47d62c009a378121398cc5477ea

