# Anaconda

## Where to find for conclusive and official documentation

Check the official [docs](https://docs.anaconda.com/index.html) for installations.
This mainly covers setup.

## Setting up a virtual environment

You need to have anaconda installed and added to your path on your terminal.
Then you can set it up:

```bash
user:~$ conda create -n example_env
user:~$ conda activate
(example_env) user:~$ ...
```

## Installing packages

Installing packages is relatively simple you just:

```bash
(example_env) user:~$ conda install anaconda-docs
```

## Uninstalling packages

Uninstalling packages is similar, you just:

```bash
(example_env) user:~$ conda remove anaconda-docs
```

## Removing your virtual environment

Make sure you have deactivated your environment then:

```bash
(example_env) user:~$ conda deactivate
user:~$ conda remove --name example_env --all
```

- The `--name` flag specifies the anaconda environment name
- The `--all` specifies the removal of all packages within that environment
