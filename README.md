<div style="display: flex; align-items: center;">
  <img src="https://github.com/abraao69/abraao69-portfolio-abraao/blob/master/testinho/portfolio/1679067787215.jpeg" width="70" height="100" style="border-radius: 100%;">
  <img src="https://github.com/abraao69/ApiRestful-teste/blob/main/logo.png" alt="Logo" width="200" height="100">
  <br><br>
</div>

  <img src="https://i.ytimg.com/vi/SzsPe_QX__c/maxresdefault.jpg" alt="Logo" width="1000" height="600" style="border-radius: 100%;">


# Curso Laravel Microservices com RabbitMQ (micro e-mail)
[Saiba Mais Sobre o Curso](https://academy.especializati.com.br/curso/laravel-microservices-micro-emails)

## Requisitos
Este micro e-mail depende do microservice 01, portanto, primeiramente subir o [microservice 01](https://github.com/especializati/laravel-microservice-01)
E também depende do microservice 02, portanto, também subir o [microservice 02](https://github.com/especializati/laravel-microservice-02)

### Instalação
Clonar Projeto
```sh
git clone https://github.com/abraao69/laravel-micro-email.git
```

Acessar o projeto
```sh
cd laravel-micro-email
```

Criar o Arquivo .env
```sh
cp .env.example .env
```

Atualizar as variáveis de ambiente do arquivo .env
```dosini
APP_NAME=EspecializaTi
APP_URL=http://localhost:8005

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```

Subir os containers do projeto
```sh
docker-compose up -d
```

Acessar o container
```sh
docker-compose exec micro_mail bash
```

Instalar as dependências do projeto
```sh
composer install
```

Gerar a key do projeto Laravel
```sh
php artisan key:generate
```

Acessar o projeto
[http://localhost:8005](http://localhost:8005)
