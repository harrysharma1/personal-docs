# Anaconda

## Where to find for conclusive and official documentation

Check the official [docs](https://docs.anaconda.com/index.html) for installations.
This mainly covers setup.

## Setting up a virtual environment

You need to have anaconda installed and added to your path on your terminal.
Then you can set it up in your terminal:

```bash
conda create -n example_env
conda activate
```

## Installing packages

Installing packages is relatively simple you just:

```bash
conda install anaconda-docs
```

## Uninstalling packages

Uninstalling packages is similar, you just:

```bash
conda remove anaconda-docs
```

## Removing your virtual environment

Make sure you have deactivated your environment then:

```bash
conda deactivate
conda remove --name example_env --all
```

- The `--name` flag specifies the anaconda environment name
- The `--all` specifies the removal of all packages within that environment
