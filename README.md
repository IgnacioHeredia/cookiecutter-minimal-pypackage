# Minimal Pypackage Cookiecutter

A minimal [cookiecutter](https://github.com/audreyr/cookiecutter) template for Python packages, forked from [kragniz](https://github.com/kragniz/cookiecutter-pypackage-minimal).

```
pip install cookiecutter
cookiecutter https://github.com/ignacioheredia/cookiecutter-minimal-pypackage.git
```

**Post-generation actions:**
* run `git init` to make the package installable via `pip install -e .`
* check `setup.cfg` to apply to proper [PyPI classifiers](https://pypi.org/classifiers/)
* choose a [license](https://choosealicense.com/) for the project
* remove `tox.ini` and `tests/` if you want to remove tests
* if you don't want automatic releases based on Conventional Commits you can remove using Release Please:
  - `.github/workflows/release-please.yml`
  - `.release-please-manifest.json`
  - `.release-please-config.json`
Otherwise, if you want this feature, create a _fine grained personal access token_ for this repo only with permissions:
  - content: `write`
  - pull-requests: `write`
Then copy the token in this repo SECRETS with the name `MY_RELEASE_PLEASE_TOKEN`.
