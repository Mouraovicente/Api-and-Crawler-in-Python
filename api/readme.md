## Desafio IN8 
#### 05) API Imagine que você ficou responsável por desenvolver o backend do sistema de uma biblioteca. Crie uma API RESTful para o cadastro, edição, listagem e exclusão dos livros (título, autor, edição) e o controle de entradas e saídas.  
A proposta foi feita em Python com [Django](https://www.djangoproject.com/) e [Django Rest Framework](https://www.django-rest-framework.org/)   
  
Requisitos:  
 - Python  
 - Postman  
   
 Para garantir uma facilidade, o projeto já acompanha o `db.sqlite3` para ser executado de maneira mais simples e já possui alguns dados pré-cadastrados. 

> Um [ambiente virtual de python](https://docs.python.org/3/library/venv.html) é recomendado, porem não é obrigatório para os passos abaixo.
> <br> Lembre-se de estar na pasta /api/ ao executar os comandos abaixo:

 1. `pip install -r requirements.txt`   para instalar as dependências 
 2. Defina as variáveis de ambiente (veja `.env.example`; o Django não lê o arquivo `.env` sozinho, exporte no shell). `DJANGO_SECRET_KEY` é obrigatória: sem ela o servidor aborta com `RuntimeError: DJANGO_SECRET_KEY is required...`. Só para desenvolvimento local, `DJANGO_DEBUG=true` libera uma chave insegura de dev. Opcional: `DJANGO_ALLOWED_HOSTS` (padrão `localhost,127.0.0.1`).
 3. `python manage.py migrate` para criar o banco, caso `db.sqlite3` não exista
 4. `python manage.py runserver` para executar o servidor na porta :8000 (endpoints em `/biblioteca/`)

Agora basta importar o Postman [por link](https://www.getpostman.com/collections/ab77ab1737fcf5ec147e) ou por arquivo que esta em `api/Biblioteca.postman_collection.json`


O usuário super criado no banco enviado é: `Login: admin | Senha: admin`
