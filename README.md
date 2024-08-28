Aqui está um exemplo de README que cobre os pontos solicitados:

---

# Introdução aos Estudos de Computação Quântica

## Notebooks


1. [Portas Lógicas - Clássica e suas Representações Quânticas](notebooks/01-portas_logicas/Portas%20L%C3%B3gicas.ipynb)

* Neste notebook, discutimos as portas lógicas clássicas, como NOT, AND, OR, e suas correspondentes versões quânticas. O notebook fornece uma introdução prática e teórica sobre como essas portas são implementadas no contexto da computação quântica.

## Configuração do Ambiente

Para garantir que o ambiente de desenvolvimento esteja configurado corretamente, siga as instruções abaixo:

### Instalação do pyenv

**Linux:**

1. Atualize os pacotes e instale as dependências:
    ```bash
    sudo apt update; sudo apt install -y make build-essential libssl-dev zlib1g-dev \
    libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
    libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev \
    libgdbm-dev libnss3-dev libgdbm-compat-dev git
    ```

2. Instale o `pyenv` via curl:
    ```bash
    curl https://pyenv.run | bash
    ```

3. Adicione as seguintes linhas ao seu `~/.bashrc` (ou `~/.zshrc` se usar Zsh):
    ```bash
    export PATH="$HOME/.pyenv/bin:$PATH"
    eval "$(pyenv init --path)"
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"
    ```

4. Reinicie o terminal ou rode `source ~/.bashrc` para aplicar as mudanças.

**Windows:**

1. Instale o `pyenv` usando o [instalador oficial](https://github.com/pyenv-win/pyenv-win#installation):
    ```powershell
    Invoke-WebRequest -Uri https://pyenv.run | Invoke-Expression
    ```

2. Adicione `pyenv` ao seu `Path` e reinicie o terminal.

### Configuração do Ambiente Local

1. Navegue até o diretório do projeto:
    ```bash
    cd /caminho/para/o/projeto
    ```

2. Instale a versão Python 3.11.9 e defina-a localmente:
    ```bash
    pyenv install 3.11.9
    pyenv local 3.11.9
    ```

3. Instale o Poetry:
    ```bash
    curl -sSL https://install.python-poetry.org | python3 -
    ```

4. Instale as dependências do projeto:
    ```bash
    poetry install
    ```