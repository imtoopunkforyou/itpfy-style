# itpfy-style (づ ◕‿◕ )づ

I use [nitpick](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/usage/integrations/nitpick.html) for sharing my python code style.

- Package manager: [poetry](https://github.com/python-poetry/poetry)
- Linter: [flake8](https://github.com/pycqa/flake8)
- Linter plugin: [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide)
- Static type checker: [mypy](https://github.com/python/mypy)
- Imports sorter: [isort](https://github.com/PyCQA/isort)
- Docstring linter: [darglint](https://github.com/terrencepreilly/darglint)

## Usage
```bash
poetry add --group lint wemake-python-styleguide mypy darglint
```
```bash
poetry add --group dev nitpick ipython
```
Add link to `pyproject.toml`:
```code
[tool.nitpick]
style = "https://raw.githubusercontent.com/imtoopunkforyou/itpfy-style/refs/heads/main/py/imtoopunkforyou.toml"
```
```bash
nitpick fix
```
```bash
flake8 ./ && mypy ./ --no-pretty
```
