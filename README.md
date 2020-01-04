# Docker Django

Ambiente de desenvolvimento usando Docker Compose. Usa:

* Python 3.8.x
* Django (última versão)

## Instalação

Faça o clone desse repositório.

```shell
git clone https://github.com/simonardejr/dockerdjango.git

cd dockerdjango/
```

## Crie um projeto Django

Para criar o projeto, execute:

```shell
docker-compose run web django-admin.py startproject nome_do_projeto .
```
> IMPORTANTE, não esqueça o "." no final do comando.

Ao ser executado pela primeira vez, o comando vai criar o container, instalar o Django em sua última versão e criar o projeto dentro do diretório `./app`

## Agora é só subir o ambiente de desenvolvimento

Execute
```shell
docker-compose up -d
```
E acesse `http://localhost:8000` no seu navegador ;)
