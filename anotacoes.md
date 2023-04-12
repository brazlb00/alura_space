Ativando a venv

1: virtualenv env
2: source env/bin/activate 

Finalizar a venv
1: deactivate

Instalação Django:
pip3 install django

Verificar dependencias:
pip3 freeze

Criando um .md com as dependências
pip3 freeze > requirements.md

Criando um novo projeto:
django-admin startproject setup .

Rodar o projeto:
python manage.py runserver

Servidor e porta: http://127.0.0.1:8000

Pacote para esconder a secret key: pip install python-dotenv

1: criar um .env em /env
2: definir uma SECRET_KEY com a secret key
3: from dotenv import load_dotenv
4: load_dotenv()
5: apagar a secrevt key de manage.py
6: em manage.py alterar a secret key para = str(os.getenv('SECRET_KEY'))


Criação de apps
1: python manage.gy start app "nome_do_app"
2: Em settings.py, installed_apps inserir o nome do app em aspas simples