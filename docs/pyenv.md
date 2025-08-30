# Instalação do pyenv

1. Dependências de compilação

```sh
sudo apt update
sudo apt install -y make build-essential libssl-dev zlib1g-dev \
  libbz2-dev libreadline-dev libsqlite3-dev curl git \
  libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev \
  libffi-dev liblzma-dev
```

2. Instale o pyenv

```sh
curl https://pyenv.run | bash
```

3. Configure o shell (Bash/Zsh):

Acrescente ao final do seu ~/.bashrc ou ~/.zshrc:

```sh
export PYENV_ROOT="$HOME/.pyenv"
command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
```

Recarregue:

```sh
exec $SHELL -l
```

4. Teste

```sh
pyenv --version
```

---

# Instalando versões do python

1. Liste versões disponíveis

```sh
pyenv install -l
```

2. Instale a versão requerida

```sh
pyenv install 3.12.9
```

3. Caso queira definir como versão global


```sh
pyenv global 3.12.6
python --version
which python
```


OBS: atualização do pyenv

```sh
pyenv update
```


