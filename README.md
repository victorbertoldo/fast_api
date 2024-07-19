# Starting with Fast API

## Configuring the environment
First thing to do is install pyenv to set the environment.

For ubuntu systems:

```bash
sudo apt update
sudo apt install -y make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncurses5-dev libncursesw5-dev xz-utils tk-dev libffi-dev \
liblzma-dev python-openssl git
```

#### 2\. Install `pyenv`

Run the following commands to install `pyenv`:

bash

Copy code

```bash
curl https://pyenv.run | bash
```
This command will install `pyenv`, `pyenv-virtualenv`, and `pyenv-update`.

For `zsh`:

bash

Copy code
```bash
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init --path)"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.zshrc
source ~/.zshrc` 
```
#### 4\. Verify Installation

To verify that `pyenv` is installed correctly, run:

bash

Copy code

```
pyenv --version
```

You should see the version of `pyenv` displayed in the terminal.


Now for this project we will be using `python 3.12.4`

Run this:

```bash
pyenv update
pyenv install 3.12:latest
```

Now to set the python version as defaut we can run:

```bash
pyenv global 3.12.4
```