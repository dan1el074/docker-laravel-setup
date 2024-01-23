# Setup

Para iniciar a aplicação, baixe o Docker para desktop [nesse link](https://www.docker.com/products/docker-desktop/).

Não esqueça de fornecer as credências do banco de dados nas variáveis de ambiente, nos arquivos .env e docker-compose.yml

Depois use o seguinte comando no console:
- `docker-compose up -d --build`
- `docker exec setup-php composer install`
- `docker exec setup-php php artisan config:cache`

Para testar o banco escreva:
- `docker exec setup-php php artisan migrate`

Para acessar o projeto, basta entrar em [localhost:8080]()

Para acessar o phpMyAdmin, basta entrar em [localhost:8888]()
