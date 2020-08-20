# Ambiente de desenvolvimento laravel 

Contém:
- Nginx
- PHP-FPM
- Redis
- MySQL

Execute o comando abaixo para compilar as imagens e subir o ambiente de desenvolvimento em modo daemon (via docker-compose):

```sh
docker-compose up -d --build
```

Execute o comando abaixo para gerar o build da imagem optimizada:

```sh
docker build -t laravel-optimized -f Dockerfile.prod .
```

Para visualizar a imagem publicada no docker-hub clique [aqui](https://hub.docker.com/r/deividroger/laravel-optimized)


Para realizar o Pull da imagem do docker-hub:

```sh
docker pull deividroger/laravel-optimized:latest
```