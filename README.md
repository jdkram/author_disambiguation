# Author disambiguation

This is a small sample project intended to help Ollie Wills solve the problem he was facing with trying to disambiguate authors across papers.

## Setup

```bash
git clone this-repo-url
cd this-repo
brew install pipenv
pipenv install --skip-lock
pipenv shell
jupyter lab
```

### ExecutionTime plugin

I discovered the ExecutionTime plugin which improves on the Autotime one I was using. This displays the time a cell was last executed, as well as how long it took to run. To set this up:

Outside pipenv shell:

```bash
pipenv install jupyter-contrib-nbextensions jupyter_nbextensions_configurator
```

Inside pipenv shell:

```bash
jupyter contrib nbextension install --sys-prefix
jupyter nbextensions_configurator enable --user
```

Then config stuff using url/nbextensions.