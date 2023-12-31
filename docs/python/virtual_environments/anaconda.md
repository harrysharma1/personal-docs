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

## Mamba

Mamba is a reimplimentation of Anaconda using C++. This was intended to
speed up resolution speeds compared to Anaconda. This is newer, but if
you do get stuck with Anaconda, you can use this as an alternative.
Documentation on mamba can be found [here.](https://mamba.readthedocs.io/en/latest/)

### Basic usage

Make sure you have deactivated your environment then:

```bash
conda create -n mamba_environment -c conda-forge mamba
conda activate mamba_environment
(mamba_environment) mamba create -n new-environment -c <channel> <packages-to-install>

# Run 'mamba init' to be able to run mamba activate/deactivate
# and start a new shell session. Or use conda to activate/deactivate.

# (mamba_environment) $ mamba init
# (mamba_environment) $ source ~/.bashrc

(mamba_environment) mamba activate new-environment
```
