# Pyenv

## Introduction to Pyenv

Pyenv is a tool used to work with various versions of Python.
Documentation on the full installation can be found
[here.](https://github.com/pyenv/pyenv)

### Installation

I will show how to install `pyenv` for Ubuntu/Debian systems:

1. First clone the repo into your home directory under a hidden file:

    ```bash
    git clone https://github.com/pyenv/pyenv.git ~/.pyenv
    ```

2. You can also compile this dynamic bash extension to speed up the command.
Don't worry if it does not work though:

    ```bash
    cd ~/.pyenv && src/configure && make -C src
    ```

3. Now add this to your `~/.bashrc`:

    ```bash
    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
    echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
    echo 'eval "$(pyenv init -)"' >> ~/.bashrc
    ```

4. Now if you have either `~/.bash_profile` or `~/.profile` add this:

    ```bash
    # ~/.profile
    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.profile
    echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.profile
    echo 'eval "$(pyenv init -)"' >> ~/.profile
    ```

    ```bash
    # ~/.bash_profile
    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
    echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
    echo 'eval "$(pyenv init -)"' >> ~/.bash_profile
    ```

5. Restart your shell:

    ```bash
    exec "$SHELL"
    ```

    or

    ```bash
    source ~/.bashrc
    ```
