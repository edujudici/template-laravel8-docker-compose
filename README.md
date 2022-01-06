# Simple laravel docker environment 

Projeto utilizando docker com uma versão simples do laravel 8.x

### Tecnologias

Utiliza-se as seguintes tecnologias para o funcionamento desse sistema:

* [Laravel 8.x] - Framework PHP
* [Docker] - Administrador de containers

### Pré-requisitos
 - Executando o docker na maquina local
 - Executando o docker-compose na maquina local
 - Conhecimento básico em docker e PHP

### Instalação

Assume que atenda aos pré-requisitos informados acima para seguir com os passos abaixo:

Clonando o repositório

```sh
$ git clone https://github.com/edujudici/template-laravel8-docker-compose.git
```

Executar o shell script de instalação

```sh
$ ./install-development.sh
```

Os seguintes passos serão executados para o funcionamento do sistema:
 - Buildar e subir os containers
 - Instalação das depencias do projeto
 - Geração da key para o correto funcionamento do Laravel
 - Execução das migrations no banco de dados
 - Execução dos seeders para preenchimento de informações nas tabelas

### Como acessar

 - Acessando o sistema: [localhost:8000](http://localhost:8000/)
 - Acessando banco de dados [localhost:8001](http://localhost:8001)

### Comandos utéis

 - Start containers
     ```sh
    $ docker-compose up -d
    ```
 - Stop e remove containers
    ```sh
    $ docker-compose down
    ```
  - Instalando depencias
    ```sh
    $ docker-compose exec app composer install
    ```
  - Executando as migrations no banco de dados
    ```sh
    $ docker-compose exec app php artisan migrate
    ```
    
License
----

MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [Laravel 8.x]: <https://laravel.com/docs/8.x>
   [Docker]: <https://www.docker.com/>
