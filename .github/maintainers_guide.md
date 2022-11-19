# Maintainers Guide

This project uses [MKdocs](https://www.mkdocs.org/) to render the pages.

## Python

```zsh
brew install pyenv

pyenv install -l

pyenv install 3.10.8

pyenv local 3.10.8

python -m venv env_3.10.8

source env_3.10.8/bin/activate
```

```zsh
pip install -r requirments.txt

./scripts/serve.sh
```

## Add page

1. create a new `.md` file in the `/docs` folder ex: `docs/egg_fried_rice.md`
2. add this page in `mkdocs.yml` file to allow it to appear in the sidebar

```yaml
nav:
    - welcome: index.md
    - egg fried rice: egg_fried_rice.md
```

## deploy

https://dash.cloudflare.com
