# Gerenciamento simples para versões de Python : pyenv

Gerenciar várias versões do Python de maneira simples e intuitiva, é a proposta do *pyenv*. Com ele podemos instalar e gerenciar multiplas versões do Python em nossos ambientes de desenvolvimento.

## Instalação

Instalando algumas dependências para o *pyenv*

```
sudo apt-get install -y make build-essential libssl-dev && sudo apt-get install -y zlib1g-dev libbz2-dev libreadline-dev
sudo apt-get install -y libsqlite3-dev wget curl llvm libncurses5-dev libffi-dev git
```
Agora vamos o usar o caminho $HOME/.pyenv para através do git baixar ele.

```
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
```

Hora de definir as variáveis de ambiente.

```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Vamos validar que o pyenv tá instalado e configurado corretamente.

```
pyenv --version
```

## Principais comandos

Listar todas as versões de Python disponíveis para instalação.

```
pyenv install -l
```

Instalando uma versão do Python, vamos instalar a 3.8.13

```
pyenv install 3.8.13
```

Listar todas as versões do Python instaladas.

```
pyenv versions
```

Definindo a versão do Python que vamos utilizar.

```
pyenv global 3.8.13
```







