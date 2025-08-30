# Instalação do poetry

1. Instale o poetry

```sh
curl -sSL https://install.python-poetry.org | python3 -
```

2. Garanta que o poetry está no PATH

Adicione no seu ~/.bashrc ou ~/.zshrc:

```sh
export PATH="$HOME/.local/bin:$PATH"
```

Recarregue:

```sh
exec $SHELL -l
```

3. Teste:

```sh
poetry --version
```
