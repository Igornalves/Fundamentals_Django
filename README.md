# Projeto fundamentos Python com Django 

Projeto com o intuito de desenvolver um API usando o Python com Django que e uma fremework 

- para criar o ambiente virtual
```bash
python -m venv venv 
```

- para roda o ambiente virtual ativado 
```bash 
.\venv\Scripts\activate
```

- para desativar o ambiente virtual do venv 
```bash 
deactivate
```

- agora instale o django com o ambiente virtual ativo
```bash 
pip install django
```

- para saber se o django foi instalado com sucesso 
```bash
django-admin --version
```

- iniciando o projeto com Django 
```bash
django-admin startproject <nome-proejeto> <diretorio-pasta> 

django-admin startproject app .
```

- rodando o projeto Django
```bash
python manage.py runserver
```

- para rodar os arquivos de teste da aplicacao
```bash
python manage.py test
```

- falando de rotas na aplicacao que se localiza no arquivo que fica responsavel por colocar as rotas da aplicacao no projeto
```bash
.\app\urls.py
```

- arquivo de configuracoes estao na raiz
```bash
.\manage.py 
```

- criando uma app para fazer o gerenciamentos de uma parte da aplicacao
```bash
python manage.py startapp cars
```

- para que o django consiga identificar o app criado precisa fazer a alteracao no arquivo 
```bash
.\app\settings.py
```
- que fica mais ou menos assim 
```bash
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'cars',
    '<ADCIONANDO_MAIS_AQUI>',
]
```

# Fundamentals Django

## Configuração no Ubuntu

### 1. Entrar no projeto

```bash
cd ~/Documentos/Projeto\ Vscode/Fundamentals_Django
```

### 2. Instalar o suporte ao `venv`

```bash
sudo apt update
sudo apt install python3.14-venv
```

### 3. Criar o ambiente virtual

```bash
python3 -m venv venv
```

> Se o `venv` tiver sido criado com erro anteriormente:

```bash
rm -rf venv
python3 -m venv venv
```

### 4. Ativar o ambiente virtual

```bash
source venv/bin/activate
```

Se aparecer `(venv)` no terminal, está funcionando.

### 5. Atualizar o pip

```bash
python -m pip install --upgrade pip
```

### 6. Instalar o Django

```bash
pip install django
```

### 7. Verificar

```bash
python --version
django-admin --version
which python
```

O `which python` deve apontar para:

```text
venv/bin/python
```

### 8. Desativar

```bash
deactivate
```

---

## Comandos rápidos

```bash
# Ativar
source venv/bin/activate

# Desativar
deactivate

# Ver Python
python --version

# Ver Django
django-admin --version
```

