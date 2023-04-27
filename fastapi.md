---
description: >-
  FastAPI framework, high performance, easy to learn, fast to code, ready for
  production
---

# FastAPI

## Installation

{% tabs %}
{% tab title="mac" %}
```bash
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew install openssl readline sqlite3 xz zlib
$ curl https://pyenv.run | zsh

$ vi .zshrc
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv virtualenv-init -)"
$ exec $SHELL
```
{% endtab %}

{% tab title="ubuntu" %}
```bash
$ sudo apt-get install -y make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev \
libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python-openssl

$ curl https://pyenv.run | bash

$ vi .bashrc
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv virtualenv-init -)"
$ exec $SHELL
```
{% endtab %}
{% endtabs %}

## Setup

```bash
$ pyenv update
$ pyenv versions
$ pyenv install --list | grep " 3\."
$ pyenv install 3.11.3

$ pyenv global 3.11.3  # ~/.pyenv/version
$ python -V
# $ pyenv global system
# $ pyenv uninstall 3.11.3

$ pyenv which pip
/Users/joyplug/.pyenv/versions/3.11.3/bin/pip

$ pip -V
pip 22.3.1 from /Users/joyplug/.pyenv/versions/3.11.3/lib/python3.11/site-packages/pip (python 3.11)

$ pyenv local 3.10.3  # .python-version, 현재 디렉토리, App별로 설치
$ pyenv shell 3.10.4  # PYENV_VERSION 환경변수, 첫번째 우선순위
# pyenv shell --unset
```
