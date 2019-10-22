# CONFIGURAÇÃO DO DIRETÓRIO

## Crie um diretório chamado django:
### 1. $ cd
### 2. $ mkdir django
### 3. $ cd django
---------------------------------------------------------------------------------------------------------
# INSTALAÇÃO AMBIENTE VIRTUAL(venv)

## Crie um virtualenv chamado myenv, digitando o seguinte comando no terminal:
### 1. $ python3 -m venv myenv


## Caso receba erro, instale o python3-venv, digitando o seguinte comando no terminal:
### 1. $ sudo apt install python3-venv


## Ative o virtualenv no diretório atual, digitando o seguinte comando no terminal:
### 1.$ source myenv/bin/activate

---------------------------------------------------------------------------------------------------------
# INSTALAÇÃO/ATUALIZAÇÃO PIP

## Garanta que o pip esteja em sua versão mais atual, digitando o seguinte comando no terminal:
### 1. (myvenv) ~$ python -m pip install --upgrade pip


## Instale as dependências do projeto, que estão incluídas no arquivo requirements, utilizando o pip, na pasta django, digitando o seguinte comando no terminal:
### 1. (myvenv) ~$ pip install -r requirements.txt

---------------------------------------------------------------------------------------------------------
# CRIANDO PROJETO DJANGO - SO Linux

## Com o venv ativo, execute o seguinte comando no terminal:
### 1. $ django-admin startproject mysite .
(Obs.: Não esquecer do ponto(.) final, pois referencia o diretório atual).

---------------------------------------------------------------------------------------------------------
# CONFIGURANDO PROJETO COMO LOCALHOST

## 1. Navegue até o diretório django/mysite e abra o arquivo setting.py em formato de texto.

## 2. Procure por DEBUG, defina como true, caso não esteja.

## 3. Procure por ALLOWED_HOSTS, defina como [], caso não esteja.

## Deverá ficar da seguinte forma:

### DEBUG = True

### ALLOWED_HOSTS = []

---------------------------------------------------------------------------------------------------------
# CRIAR BANCO DE DADOS (sqlite3)

## 1. Com o venv ativo, no diretório django, digite o seguinte comando no terminal:
### python manage.py migrate

---------------------------------------------------------------------------------------------------------
# INICIANDO O SERVIDOR WEB

## 1. Com o venv ativo, no diretório django, digite o seguinte comando no terminal:
### python manage.py runserver
