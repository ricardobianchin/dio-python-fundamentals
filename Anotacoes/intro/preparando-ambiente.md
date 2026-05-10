# Preparando o Ambiente de Desenvolvimento

Optei por não instalar o Python no meu computador. Ao invés disso, instalarei ambiente virtual, de formas que possa ter um ambiente isolado para cada projeto, sem me preocupar com conflitos de dependências ou versões e ter uma versão diferente para cada projeto.

## Configurando o Ambiente Virtual

O primeiro passo é instalar o pyenv-win, que vai gerenciar os ambientes virtuais. Abra o PowerShell em modo administrador e execute o comando:

``` powershell
Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
```

Crie a pasta do projeto. Abra o cmd e vá até a pasta raiz dele.

```powershell
pyenv local 3.13.13
pyenv virtualenv 3.13.13 .venv
.venv\Scripts\activate
python --version
python -m pip install --upgrade pip
pip --version
```

O comando `pyenv local 3.13.13` define a versão do Python para o projeto. O comando `pyenv virtualenv 3.13.13 .venv` cria um ambiente virtual usando a versão do Python especificada e o nome do ambiente virtual é `.venv`. O comando `.venv\Scripts\activate` ativa o ambiente virtual, permitindo que você use as dependências instaladas nele. O comando `python --version` verifica a versão do Python ativa, e o comando `python -m pip install --upgrade pip` atualiza o gerenciador de pacotes pip para a versão mais recente. 

Atente sempre para o prompt de comandos que deve iniciar por (.venv) para indicar que o ambiente virtual está ativo.

Enquanto estiver ativo, o comando python e pip se referirão à versão do Python e às dependências instaladas na pasta do seu projeto apenas.

Quando terminar de trabalhar no projeto, você pode desativar o ambiente virtual usando o comando no CMD:

```bash
deactivate
```

Para remover o ambiente virtual, basta excluir a pasta `.venv` do projeto. Certifique-se de que o ambiente virtual esteja desativado antes de excluir a pasta para evitar problemas.

Você nao precisa desativar o ambiente virtual se for mudar para uma pasta de outro projeto que utilize exatamente a mesma versão do Python. Se for de versão diferente, desative o ambiente atual, entre na pasta do outro projeto e ative o ambiente virtual dele.

## Requirements

o seguinte comando no cmd gera o arquivo requirements.txt com tudo que foi instalado no ambiente virtual:

```bash
pip freeze > requirements.txt
```

## instale o vs code

Instale a extensão Python, da Microsoft, que tem suporte para linting, debugging, Jupyter Notebooks e muito mais. Ao instalar esta extensão, outras extensões serão instaladas automaticamente, como o pylance e o python debugger

O VS Code permite executar um script aberto pressionando o botão de play no canto superior direito da janela do editor. Ele também tem um terminal integrado, que pode ser aberto usando o atalho Ctrl + ` (crase). O terminal integrado é útil para executar comandos sem sair do editor, como ativar o ambiente virtual ou executar scripts Python.