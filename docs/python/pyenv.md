# Pyenv

## Introduction to Pyenv

Pyenv is a tool used to work with various versions of Python.
Documentation on the full installation can be found
[here.](https://github.com/pyenv/pyenv)

## Installation 

### Installation through Github

I will show how to install `pyenv` for through their [github](https://github.com/pyenv/pyen0v):

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

### Installation through Homebrew

The only prerequisite is that you have [Homebrew:](https://brew.sh)

1. Firstly run:

    ```bash
    brew update
    brew install pyenv
    ```

2. Assuming you have Hombrew you are probably using a Mac so run
(If not check their [github](https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv) for other shell environments):

    ```bash
    echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
    echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
    echo 'eval "$(pyenv init -)"' >> ~/.zshrc
    ```

3. Now run:

    ```bash
    alias brew='env PATH="${PATH//$(pyenv root)\/shims:/}" brew'
    ```

4. Also restart your shell:

    ```bash
    exec "$SHELL"
    ```

    or

    ```bash
    source ~/.zshrc
    ```
