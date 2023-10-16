# Virtualenv

## Where to find for conclusive and official documentation

Check the official [docs](https://virtualenv.pypa.io/en/latest/) for installations.
This mainly covers setup.

## Setting up virtual environment

You need to have Python and `virtualenv` set up. Then in your terminal:

```bash
virtualenv venv
source venv/bin/activate
```

## Installing packages

Installing packages is relatively simple you just:

```bash
pip install mkdocs
```

## Uninstalling packages

Uninstalling packages is similar, you just:

```bash
pip uninstall mkdocs
```

## Removing your virtual environment

Make sure to deactivate your environment then:

```bash
deactivate
rm -rf venv
```

- `-rf` removes all files within the `venv` folder recursively and force the removal
