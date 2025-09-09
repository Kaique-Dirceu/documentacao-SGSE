# Links 
MkDocs: https://www.mkdocs.org/

Markdown guia: https://www.markdownguide.org/basic-syntax/ 

# Instalação

Clone o projeto e acesse a pasta:

```bash
$ git clone https://github.com/Kaique-Dirceu/documentacao-SGSE.git
$ cd documentacao-SGSE
```
Certifique-se de ter o Python e o pip instalados:
```bash
python --version
```

A saída esperada deve ser algo como:
```bash
Python 3.12.3
```
Verifique também o pip:
```bash
pip --version
```
A saída esperada deve ser algo como:
```bash
pip 24.0 from /usr/lib/python3/dist-packages/pip (python 3.12)
```


## Criar o ambiente virtual
Primeiro, é necessário criar um ambiente virtual para instalar as dependências do projeto.

> Não é obrigatório seguir exatamente este tutorial. Crie o ambiente da maneira que preferir e depois vá direto para a seção **[Executar o projeto](#executar-o-projeto)**.

## Linux / mac
Rode o comando:
```bash
python3 -m venv venv
```
Ele criará uma pasta chamada `venv` no projeto.

> ⚠️ Caso o python não tenha criado uma pasta `venv` ou se dentro de `venv/bin` não existir o arquivo de activate. Execute:
> ```bash
> sudo apt update
> sudo apt install python3-venv -y
> ```
> Em seguida, rode novamente o comando para criar o ambiente virtual.

Agora, ative o ambiente:

```bash
source venv/bin/activate
```
Se tudo ocorrer corretamente, aparecerá no terminal `(venv)`, indicando que o ambiente está ativado.

## Windows
Rode o comando:

```bash
python -m venv venv
```

Ele criará uma pasta chamada `venv` no projeto.
Agora, ative o ambiente:

Caso esteja usando o **PowerShell**:
```cmd
.\env\Scripts\Activate.ps1
```
Ou caso esteja usando o **CMD**:
```cmd
.\env\Scripts\Activate.bat
```

> ⚠️ Caso houver um erro. 
> 
> Execute o **PowerShell** como administrador e rode:
> ```cmd
> Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
> ```
> Em seguida, digite **S** para aceitar.


# Executar o projeto
Para roda o projeto, primeiro é necessario instalar as dependências.

Execute:
```bash
pip install -r requirements.txt
```

E para iniciar o MkDocs:
```bash
mkdocs serve
```

Pronto! 🎉

A documentação estará disponível em seu localhost.