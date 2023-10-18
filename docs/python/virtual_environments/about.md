# About

## Virtual environments

A virtual environment allows an isolated use of
package installation for each and every project.

## Use for virtual environment

As projects require specific versions of certain packages,
a problem can occur when working on multiple projects.
If you were to install version 1.0 of a
package globally for one project but another required version
0.9 this would cause clashs when trying to run projects.

## Specific to Python

There are two main virtual environments for Python:

1. [`Virtualenv`](virtualenv.md) (for pip)
1. [`Conda`](anaconda.md) (for conda)
    1. [`Mamba`](anaconda.md#mamba) (faster but newer implementation of conda)
