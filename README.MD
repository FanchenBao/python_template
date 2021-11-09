# Description

The purpose of this repo is to create a template for Python project that I'd like to follow. This repo will be updated if I find it necessary to include new toolings.

# Pre-installed Packages

These packages are for linting, testing, and git commit safeguarding.

## Linting and Formating
* wemake-python-styleguide
* mypy
* isort
* pyformat

## Testing
* pytest
* pytest-cov

## Git Commit Safeguarding
* pre-commit

# Usage

1. Clone the repo, and **change the folder name** to that of your project
    ```
    git clone https://github.com/FanchenBao/python_template.git
    ```
2. Remove the git history associated with the development of this template and create a new one
    ```
    rm -rf .git && git init
    ```
3. Inside the folder, create a virtual environment (recommended `pyenv`)
4. Inside the virtualenv
    ```bash
    pip install --upgrade pip && pip install -r requirements.txt
    ```
5. `pre-commit install`
6. Add other packages if needed. Adjust the configuration of the strictness of linting as needed (i.e. modify `setup.cfg`).

## Specifics for data science
I prepare my own virtualenv for data science projects. Thus, the following packages must be installed in addition to the ones that come with the template.

```
pip install jupyterlab numpy pandas scipy matplotlib
```

