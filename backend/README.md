# Rest API

## Requisitos do cliente
Possuir uma máquina com ambiente python configurável e/ou docker, caso queira executar a aplicação em um container.

## Tecnologias usadas
- API Rest
    + [Flask](https://flask.palletsprojects.com/en/2.2.x/)
    + [Flask-Smorest](https://flask-smorest.readthedocs.io/en/latest/)
- Testes
    + [Pytest](https://coverage.readthedocs.io/)
    + [Testes com Pytest](https://flask.palletsprojects.com/en/2.2.x/tutorial/tests/)
- Implantação
    + [Gunicorn](https://gunicorn.org/)
    + [Implantação com Gunicorn](https://flask.palletsprojects.com/en/2.2.x/deploying/gunicorn/)
    + [Docker](https://www.docker.com/products/docker-desktop/)
    + [Docker Compose](https://docs.docker.com/compose/)

## Iniciar a aplicação

### Iniciar a aplicação  usando Docker Compose
No meu setup foi utilizado o Docker Compose versão v2.15.1
<pre>
docker compose up
</pre>

### Iniciar a aplicação sem docker
`Na pasta raiz`
<pre>pip install -r requirements.txt
gunicorn --bind 0.0.0.0:8080 'pspython:create_app()'
</pre>


## Link para Swagger Docs
`http://localhost:8000/swagger-ui`<br>
[Swagger-docs](http://localhost:8000/swagger-ui)

## Executar testes
`Na pasta raiz, execute o comando:`
<pre>pytest
</pre>