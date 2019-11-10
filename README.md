# bootcamp-gympoint-rocketseat
API Projeto Gympoint do desafio do bootcamp da Rocketseat

Para rodar a aplicação é necessário ter instalado o node, npm, yarn e o docker.

Para criar o conteiner do banco execute o seguinte comando na raiz do Projeto:
$ docker image build -t db-gympoint:1.0 .
$ docker container run --publish 3306:3306 --detach --name db-gympoint db-gympoint:1.0

Para criar as tabelas no banco execute o comando:
$ yarn sequelize db:migrate

Para dar carga nas seeds de dados execute:
$ yarn sequelize db:seed:all

Para rodar a API execute:
$ yarn dev

A collection do postman se encontra na pasta docs com o nome "Gympoint.postman_collection.json"
