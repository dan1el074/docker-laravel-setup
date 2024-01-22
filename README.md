# Setup

Para iniciar a aplicação, baixe o Docker para desktop [nesse link](https://www.docker.com/products/docker-desktop/).

Depois use o seguinte comando no console:
- `docker-compose up -d --build`
- `docker exec setup-php php artisan config:cache`
- `docker exec setup-php composer install`

Para testar o banco escreva:
- `docker exec setup-php php artisan migrate`

Para acessar o projeto, basta entrar em [localhost:8080]()

Para acessar o phpMyAdmin, basta entrar em [localhost:8888]() com as credências:
- usuario: `user`
- senha: `password`


Todos esses passos foram extraídos desse [video](https://www.youtube.com/watch?v=E4-IfMSZCVc&ab_channel=Jo%C3%A3oLucasXavier)!
