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
