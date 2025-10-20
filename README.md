## Caso não tenha sido criado o ambiente
>> python3 -m venv venv

## Ativa o ambiente virtual
>> source venv/bin/activate

## Instale as dependencias do Django
>> pip install django djangorestframework django-cors-headers dj-rest-auth django-allauth djangorestframework-simplejwt python-dotenv

## Criação da estrutura principal do projeto
>> django-admin startproject backend .

### Exemplo de criação de um app
>> python manage.py startapp accounts

## Rode as migrações do sistema 
>> python manage.py makemigrations
>> python manage.py migrate


# Observação
Cada App, precisa de 4 arquivos essenciais para conseguir subir uma instância do projeto:\
  models.py: Arquivo referente a configuração do banco de dados\
  uls.py: Aquivo referente a configuração de rota relacionado com aquele app\
  views.py: Arquivo referente a configuração de como as informações desse app serão apresentadas\
  serializers.py: Arquivo referente a conversão das informações de uma estrutura para outra\

Na falta de um desses, é impossivel subir uma instância de teste
