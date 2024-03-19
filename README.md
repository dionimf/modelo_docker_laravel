# modelo_docker_laravel
Modelo de docker-compose para subir um container laravel 11 com php 8.3

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/dionimf/modelo_docker_laravel.git
```
```sh
cd modelo_docker_laravel
```
Suba os containers do projeto
```sh
docker-compose up -d
```


Crie o Arquivo .env
```sh
cp .env.example .env
```

Acesse o container app
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```

Gere a key do projeto Laravel
```sh
php artisan key:generate
```

Rodar as migrations
```sh
php artisan migrate
```

Acesse o projeto
[http://localhost:8000](http://localhost:8000)